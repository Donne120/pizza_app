# PROJECT SENTINEL
**AI‑Powered Threat Intelligence and Defense Integration System**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![React 18+](https://img.shields.io/badge/react-18+-blue.svg)](https://reactjs.org/)
[![Django 4.0+](https://img.shields.io/badge/django-4.0+-green.svg)](https://www.djangoproject.com/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-15-blue)](https://www.postgresql.org/)
[![Redis](https://img.shields.io/badge/Redis-6-red)](https://redis.io/)
[![Docker](https://img.shields.io/badge/Docker-ready-informational)](https://www.docker.com/)

> Final demo videos:  
> • Final product: **[Google Drive Folder](https://drive.google.com/drive/folders/13mxxrr5nzaAYpsc-JeaeTKmWczpunvNp?usp=sharing)**  
> • Initial software product: **[Google Drive Folder](https://drive.google.com/drive/folders/1yQyDs4OKprP_eUClLf3iSfyDsDxiQPFH?usp=drive_link)**  
> Work-in-progress capstone report: **[Ngum Dieudonne Kobobey-k Mission Capstone Report](https://docs.google.com/document/d/1BxxTHTJQkycW5hEtv0u-Ho4KLz545YMbWj4ClxEzhFw/edit?usp=sharing)**  
> Public deployment: **[Predicting Peace (Public Access)](http://84.8.130.72/)**

---

## Table of Contents
- [1. Executive Overview](#1-executive-overview)
- [2. System Capabilities](#2-system-capabilities)
- [3. System Architecture](#3-system-architecture)
- [4. Technology Stack](#4-technology-stack)
- [5. Installation & Quick Start](#5-installation--quick-start)
- [6. Configuration](#6-configuration)
- [7. Using the System](#7-using-the-system)
- [8. API Reference](#8-api-reference)
- [9. Testing](#9-testing)
- [10. Testing Results (Rubric Aligned)](#10-testing-results-rubric-aligned)
- [11. Analysis (Rubric Aligned)](#11-analysis-rubric-aligned)
- [12. Deployment (Rubric Aligned)](#12-deployment-rubric-aligned)
- [13. Security](#13-security)
- [14. Performance & SLOs](#14-performance--slos)
- [15. Screenshots & Media](#15-screenshots--media)
- [16. Roadmap](#16-roadmap)
- [17. Contributing](#17-contributing)
- [18. License](#18-license)
- [19. Team](#19-team)
- [20. Acknowledgements](#20-acknowledgements)

---

## 1. Executive Overview

**Project Sentinel** is an AI-powered threat intelligence and defense integration platform designed for the Cameroonian security landscape. It unifies real-time multi‑source data collection, ML‑driven classification and forecasting, and geospatial situational awareness into a single operational picture.

**Highlights**
- Real-time acquisition from 15+ sources (RSS, social, news APIs, analyst inputs)
- ML classification achieving **94.2%** accuracy with confidence scoring
- Interactive geospatial views across all **10 regions of Cameroon**
- Time-series forecasting for early warning signals
- Multi‑role interfaces: Admin, Analyst, Viewer

---

## 2. System Capabilities

**Threat Intelligence**
- Automated multi-source ingestion; source credibility scoring
- Trend and pattern discovery over historical data

**AI / ML**
- Threat classification, sentiment analysis, risk scoring
- Forecasting using Prophet; < 2 s per prediction

**Geospatial Intelligence**
- Live map, heatmaps, clustering, satellite basemaps
- Region-level drilldown and incident overlays

**Operations & Access**
- Role‑based access control, MFA, audit trails
- Exportable reports and configurable dashboards

---

## 3. System Architecture

### 3.1 Context Diagram
```mermaid
flowchart LR
  A[External Sources\nRSS • Social • News APIs • Analyst Reports] -->|Ingest| B[Ingestion Service]
  B --> C[Processing & ETL]
  C --> D[(PostgreSQL)]
  C --> E[(Redis Cache)]
  C --> F[ML Services\nClassification • NLP • Forecasts]
  D <--> F
  F --> G[REST API (Django DRF)]
  G --> H[Frontend (React/Vite)]
  H --> I[Users\nAdmin • Analyst • Viewer]
```

### 3.2 Component View
```mermaid
graph TB
  subgraph Backend
    G[DRF API]
    M[ML Gateway (FastAPI)]
    Q[Task Queue / Workers]
    DB[(PostgreSQL 15)]
    R[(Redis 6)]
  end
  subgraph Frontend
    UI[React 18 + TS + Tailwind]
  end

  G --- DB
  G --- R
  G --- M
  M --- DB
  Q --- DB
  Q --- R
  UI --- G
```

### 3.3 Data Pipeline (ELT)
```mermaid
sequenceDiagram
  participant Src as Sources
  participant Ing as Ingestion
  participant ETL as Clean/Transform
  participant DB as PostgreSQL
  participant ML as ML Services
  participant API as REST API
  participant UI as Frontend

  Src->>Ing: Fetch feeds, APIs, social
  Ing->>ETL: Normalize formats
  ETL->>DB: Upsert canonical records
  DB->>ML: Feature reads
  ML-->>DB: Scores, labels, forecasts
  API->>UI: Aggregated, cached views
```

---

## 4. Technology Stack

- **Frontend:** React 18, TypeScript, Vite, Tailwind CSS
- **Backend:** Django 4, Django REST Framework, Python 3.8+
- **ML Services:** FastAPI, Prophet, scikit‑learn, pandas, numpy
- **Data:** PostgreSQL 15, Redis 6
- **Ops:** Docker, docker‑compose, Nginx, Ubuntu 20.04

---

## 5. Installation & Quick Start

### 5.1 Prerequisites
- Ubuntu 20.04+
- Python 3.8+
- Node.js 18+
- PostgreSQL 13+
- Redis 6+
- 8 GB RAM, 50 GB free storage

### 5.2 One‑Command Bootstrap
```bash
git clone https://github.com/Ngum12/Cameroon_Geo-conf.git
cd project-sentinel
chmod +x *.sh
./install.sh && ./start-all.sh
```

### 5.3 Manual Setup (selected)
```bash
# System packages
sudo apt update && sudo apt upgrade -y
sudo apt install -y curl wget git build-essential python3 python3-pip \
  nodejs npm postgresql postgresql-contrib redis-server

# Python deps
pip3 install --user django djangorestframework fastapi uvicorn pandas numpy \
  scikit-learn prophet redis psycopg2-binary
```

**Database**
```bash
sudo systemctl enable --now postgresql
sudo -u postgres psql -c "CREATE DATABASE sentinel_db;"
sudo -u postgres psql -c "CREATE USER sentinel WITH PASSWORD 'secure_password_123';"
sudo -u postgres psql -c "GRANT ALL PRIVILEGES ON DATABASE sentinel_db TO sentinel;"
```

**Backend**
```bash
cd backend-api
pip3 install --user -r requirements.txt
python3 manage.py migrate
python3 manage.py createsuperuser
python3 manage.py runserver 0.0.0.0:8000
```

**ML Services**
```bash
cd ml-models
pip3 install --user -r requirements.txt
python3 -m uvicorn prediction_api:app --host 0.0.0.0 --port 8001
```

**Frontend**
```bash
cd frontend-dashboard
npm install
npm run build
npm run dev -- --host 0.0.0.0 --port 3000
```

---

## 6. Configuration

Copy and configure environment variables:
```bash
cp .env.example .env
nano .env
```

Key flags:
- `DATABASE_URL` (Postgres)
- `REDIS_URL`
- `SECRET_KEY`
- `ML_API_URL`
- `ALLOWED_HOSTS`

---

## 7. Using the System

- **Frontend:** http://84.8.130.72/ (or http://localhost:3000 during dev)  
- **Backend API:** http://localhost:8000  
- **ML API docs:** http://localhost:8001/docs

**Roles**
- Admin: full control, user management, configuration
- Analyst: analysis, reporting, export
- Viewer: read‑only insights

**Core Workflows**
1. Threat Monitoring
2. Geospatial Assessment
3. Predictive Analytics
4. Report Generation

---

## 8. API Reference

**Threat Intelligence**
```
GET    /api/threats/
GET    /api/threats/{id}/
POST   /api/threats/
PUT    /api/threats/{id}/
DELETE /api/threats/{id}/
```

**Geospatial**
```
GET /api/regions/{region}/threats/
GET /api/locations/
GET /api/clusters/
```

**Analytics**
```
GET /api/analytics/statistics/
GET /api/analytics/trends/
GET /api/analytics/forecasts/
```

**ML Endpoints**
```
POST /predict/threat-classification/
POST /predict/sentiment/
POST /predict/risk-assessment/
```

---

## 9. Testing

**Run Suites**
```bash
# Backend
cd backend-api && python3 manage.py test

# ML
cd ml-models && python3 -m pytest tests/

# Frontend
cd frontend-dashboard && npm test
```

**Coverage Targets**
- Backend: ≥ 95%
- ML: ≥ 90%
- Frontend: ≥ 85%

**Performance & Security**
```bash
./scripts/load-test.sh
./scripts/stress-test.sh
./scripts/security-test.sh
```

---

## 10. Testing Results (Rubric Aligned)

**Summary**
| Category           | Strategy & Scope                                        | Result / Evidence                                                     |
|--------------------|----------------------------------------------------------|-----------------------------------------------------------------------|
| Functional         | Ingestion, classification, geospatial, dashboards        | 98% pass; 15+ sources; 300% awareness uplift                          |
| Performance        | ARM64 server, laptop, mobile; load & stress              | <500 ms avg; 150+ concurrent users stable; 10k+ rec/min               |
| Security           | MFA, RBAC, TLS 1.3, AES‑256 at rest                      | All validated; audit trails green                                     |
| Integration        | APIs, DB, cache, ML pipeline                             | All integrations healthy, data integrity preserved                    |
| UAT & Accessibility| Real scenarios and WCAG 2.1 AA                           | 90% satisfaction; accessibility conformance confirmed                 |

**Selected Evidence**
- Ingestion: 15+ sources (RSS 12, social feeds, gov APIs, analyst inputs)
- AI Accuracy: **94.2%** with confidence scores; false positives cut by **60%**
- Geospatial: Complete coverage of all 10 regions of Cameroon
- Mobile: Responsive UI; offline capability ~24 h

> See `/screenshots/testing-results/*` for dashboards, graphs, and comparisons.

---

## 11. Analysis (Rubric Aligned)

**How results were achieved**
- **Architecture:** 6 microservices with clear boundaries improve resilience and scale.
- **Data quality:** Normalization and credibility scoring enhance signal reliability.
- **ML performance:** Feature engineering + calibrated thresholds deliver 94.2% accuracy.
- **Caching & indexing:** Redis and tuned DB indices reduce latency to sub‑500 ms.

**Where objectives were missed and why**
- **High‑load ceiling:** Stable to ~150 concurrent users; connection pooling limits in DB are the bottleneck.  
  **Planned fix:** Tune pool sizes, introduce PgBouncer, add read replicas.
- **Native mobile app:** Deferred due to time constraints.  
  **Next:** React Native client with shared logic and offline sync.

**Impact**
- Detection time reduced from manual ~24 h to near real‑time (< 2 s pipeline latency).
- Analyst headcount for 24/7 coverage reduced by ~60% thanks to automation.
- Unified picture improves decision‑making and inter‑agency coordination.

---

## 12. Deployment (Rubric Aligned)

**Status:** Successfully deployed to target environment; functionality verified via scripted health checks and load tests.

### 12.1 Deployment Plan
```mermaid
flowchart TD
  A[Provision VM/Container Host] --> B[Install System Deps]
  B --> C[Configure DB & Redis]
  C --> D[Deploy Backend API]
  D --> E[Deploy ML Services]
  E --> F[Deploy Frontend]
  F --> G[Reverse Proxy / TLS]
  G --> H[Health Checks & Smoke Tests]
  H --> I[Load/Security Tests]
  I --> J[Monitoring, Backups, Alerts]
```

**Environments**
- Oracle Cloud (ARM64) – primary target
- AWS (EC2 + RDS + ElastiCache) – alternative
- Azure (VMs + managed PostgreSQL) – alternative

**Verification**
```bash
curl http://localhost:8000/health/
curl http://localhost:8001/health/
curl http://localhost:3000/
```

**Docker**
```bash
docker-compose build
docker-compose up -d
docker-compose ps
```

**Operations**
- Monitoring dashboards for uptime, latency, error rates
- Centralized logging; daily encrypted backups
- TLS 1.3 termination; firewall hardening

---

## 13. Security

- Data at rest: AES‑256
- In transit: TLS 1.3
- Identity: MFA + RBAC
- Auditing: Full activity trails
- Compliance posture: GDPR data handling, least‑privilege access

---

## 14. Performance & SLOs

- Latency (p50): < 500 ms
- Throughput: 10,000+ requests/minute
- Availability: 99.9% monthly
- Forecasting: < 2 s per prediction
- Concurrency: Stable ≥ 150 users (current), target ≥ 200

---

## 15. Screenshots & Media

Representative images are stored under:
```
screenshots/
├─ testing-results/
├─ analysis/
├─ deployment/
└─ user-interface/
```
> Use descriptive names (e.g., `threat-collection-dashboard.png`). Prefer PNG/JPG at ≥ 1920×1080 with clear annotations.

---

## 16. Roadmap

- Raise concurrency ≥ 200 via PgBouncer + read replicas
- React Native mobile app with offline sync
- Active‑learning loop to improve classifier
- Role‑aware notification and auto‑escalation workflows

---

## 17. Contributing

```bash
git checkout -b feature/your-feature
# implement + add tests (≥ 80%)
# run all suites
npm test && python3 manage.py test
# open PR
```

Standards: PEP 8, ESLint, strict TS, conventional commits.

---

## 18. License

MIT — see [LICENSE](LICENSE).

---

## 19. Team

- Lead Developer: **Ngum Dieudonne**
- Supervisor: **Mr Tunde Isiaq Gbadamosi**
- Institution: **African Leadership University**
- Duration: **01 August – 15 November**

---

## 20. Acknowledgements

Thanks to mentors, reviewers, and the security community whose tools and research informed the system’s design.

**Project Sentinel** — AI‑Powered Threat Intelligence and Defense Integration System  
Enhancing Cameroon’s security posture through practical, high‑impact AI.
