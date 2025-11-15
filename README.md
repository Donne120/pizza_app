# PROJECT SENTINEL
### AI-Powered Multi-Source Intelligence Platform for Cameroon

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![React 18+](https://img.shields.io/badge/react-18+-blue.svg)](https://reactjs.org/)
[![Django 4.0+](https://img.shields.io/badge/django-4.0+-green.svg)](https://www.djangoproject.com/)
[![Deployment Status](https://img.shields.io/badge/deployment-active-success.svg)](http://84.8.130.72/)

**A comprehensive real-time threat intelligence system leveraging artificial intelligence, geospatial analysis, and predictive analytics to enhance national security capabilities across Cameroon's 10 regions.**

**Live Demo:** http://84.8.130.72/ • **Video Demonstration:** https://drive.google.com/drive/folders/13mxxrr5nzaAYpsc-JeaeTKmWczpunvNp • **Documentation:** https://docs.google.com/document/d/1BxxTHTJQkycW5hEtv0u-Ho4KLz545YMbWj4ClxEzhFw/edit • **Report Issue:** https://github.com/Ngum12/Cameroon_Geo-conf/issues

---

## 📑 Table of Contents

1. [Executive Summary](#executive-summary)
2. [System Architecture](#system-architecture)
3. [Core Capabilities](#core-capabilities)
4. [Testing & Validation](#testing--validation)
5. [Performance Analysis](#performance-analysis)
6. [Deployment Guide](#deployment-guide)
7. [Technical Stack](#technical-stack)
8. [Installation](#installation)
9. [API Documentation](#api-documentation)
10. [Contributing](#contributing)

---

## Executive Summary

### Project Overview

Project Sentinel represents a paradigm shift in threat intelligence gathering and analysis for Cameroon's security landscape. By integrating artificial intelligence, machine learning, and geospatial intelligence, the system provides real-time situational awareness across all 10 regions of Cameroon, enabling proactive security responses and data-driven decision-making.

![Project Sentinel Dashboard](https://github.com/user-attachments/assets/3008ebd2-a896-4ba4-8db5-faa61acdc1d1)
*Figure 1: Project Sentinel Unified Intelligence Dashboard*

### Key Achievements

| Metric | Target | Achieved | Status |
|---|---|---|---|
| **Data Sources Integration** | 10+ sources | 15+ sources | ✓ Exceeded |
| **AI Classification Accuracy** | 90% | 94.2% | ✓ Exceeded |
| **Regional Coverage** | 10 regions | 10 regions | ✓ Achieved |
| **System Response Time** | <1s | <500ms | ✓ Exceeded |
| **Concurrent Users** | 100+ | 150+ | ✓ Exceeded |
| **User Satisfaction** | 85% | 90% | ✓ Exceeded |

### Problem Statement

Cameroon faces complex security challenges including the Anglophone crisis, Boko Haram insurgency, and inter-communal conflicts. Traditional intelligence gathering methods suffer from:

- **Fragmented Information**: Data scattered across multiple unintegrated sources  
- **Manual Processing**: Time-intensive analysis leading to delayed responses  
- **Limited Predictive Capability**: Reactive rather than proactive threat management  
- **Geographic Gaps**: Inconsistent coverage across remote regions  
- **Resource Constraints**: High operational costs and personnel requirements  

### Solution Impact

┌─────────────────────────────────────────────────────────────────┐
│ BEFORE SENTINEL → AFTER SENTINEL │
├─────────────────────────────────────────────────────────────────┤
│ 24-hour intelligence delay → <2 second real-time processing │
│ 5 analysts required → 2 analysts with AI assistance │
│ Manual threat correlation → Automated AI classification │
│ Fragmented data sources → 15+ integrated sources │
│ Reactive response → Predictive threat forecasting │
└─────────────────────────────────────────────────────────────────┘

yaml
Copy code

**Quantifiable Impact**
- 300% increase in threat detection speed  
- 60% reduction in human resource requirements  
- 94.2% accuracy in threat classification  
- 99.9% system uptime and availability  

---

## System Architecture

### High-Level Architecture (ASCII)

┌────────────────────────────────────────────────────────────────────────┐
│ PROJECT SENTINEL ARCHITECTURE │
└────────────────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────────────────┐
│ DATA INGESTION LAYER │
├──────────────┬──────────────┬──────────────┬──────────────┬────────────┤
│ RSS Feeds │ Social Media │ News APIs │ Field Reports│ YouTube │
│ (12 sources) │ (Twitter/FB) │ (3 govt APIs)│ (Manual) │ (Channels) │
└──────┬───────┴──────┬───────┴──────┬───────┴──────┬───────┴──────┬─────┘
│ │ │ │ │
└──────────────┴──────────────┴──────────────┴──────────────┘
│
▼
┌─────────────────────────────────────────────────────────────────────────┐
│ PROCESSING & ANALYSIS LAYER │
├─────────────────────────────────────────────────────────────────────────┤
│ NLP Engine | ML Classifier (94.2%) | Geospatial Analysis | Prophet │
└─────────────────────────────────────────────────────────────────────────┘
│
▼
┌─────────────────────────────────────────────────────────────────────────┐
│ DATA STORAGE LAYER │
├─────────────────────────────────────────────────────────────────────────┤
│ PostgreSQL 15 (Primary DB) | Redis 6 (Cache/Queue) │
└─────────────────────────────────────────────────────────────────────────┘
│
▼
┌─────────────────────────────────────────────────────────────────────────┐
│ APPLICATION LAYER │
├─────────────────────────────────────────────────────────────────────────┤
│ Django REST API (8000) | FastAPI ML (8001) │
└─────────────────────────────────────────────────────────────────────────┘
│
▼
┌─────────────────────────────────────────────────────────────────────────┐
│ PRESENTATION LAYER │
├─────────────────────────────────────────────────────────────────────────┤
│ React 18 + TypeScript (3000): Dashboard | Geospatial | Analytics │
└─────────────────────────────────────────────────────────────────────────┘

yaml
Copy code

![Detailed Architecture](https://github.com/user-attachments/assets/f1f741a7-fdad-4759-9ddc-82aab7e41f9b)
*Figure 2: Detailed System Architecture with Microservices*

### Microservices Overview

| Service | Technology | Port | Purpose |
|---|---|---|---|
| **Frontend Dashboard** | React 18 + TypeScript | 3000 | UI & visualization |
| **Backend API** | Django 4.0 + DRF | 8000 | Core business logic & data access |
| **ML Prediction API** | FastAPI + Uvicorn | 8001 | AI/ML model serving |
| **Data Collectors** | Python + Celery | - | Automated data ingestion |
| **Database** | PostgreSQL 15 | 5432 | Primary storage |
| **Cache/Queue** | Redis 6 | 6379 | Caching & task queue |

---

## Core Capabilities

### 1) Real-Time Threat Intelligence Collection

| ![Geospatial View](https://github.com/user-attachments/assets/c4b64b3b-73ce-4119-863e-0bc64ecce106) | ![Intelligence Center](https://github.com/user-attachments/assets/612bc0f5-f453-4e77-a3d2-8dc9651ada1e) |
|---|---|
| **Geospatial Intelligence View** | **Threat Intelligence Center** |

**Integrated Data Sources**

RSS Feeds (12 sources)
├─ Government Portals
├─ Regional Bulletins
├─ International Agencies
└─ Local Media

Social Media
├─ Twitter API
├─ Facebook Public Posts
└─ Telegram Channels

Official APIs (3)
├─ Ministry of Defense
├─ National Security Council
└─ Regional Command Centers

Manual Intelligence
├─ Field Reports (Analyst)
├─ Citizen Tips (Secure Portal)
└─ Inter-Agency Sharing

markdown
Copy code

**Collection Performance**
- Throughput: **10,000+** records/min  
- Latency: **<2s** source → DB  
- Reliability: **99.9%** uptime  
- Data Validation: Real-time credibility scoring  

### 2) AI-Powered Threat Analysis

Input → Preprocess → NLP (Sentiment/NER/Language) → Classifier (RF/SVM/NN)
→ Confidence Scoring → Output + Metadata

ruby
Copy code

**Model Performance**

| Model | Accuracy | Precision | Recall | F1 |
|---|---:|---:|---:|---:|
| Random Forest | 92.1% | 91.3% | 92.8% | 92.0% |
| SVM | 91.5% | 90.7% | 92.3% | 91.5% |
| Neural Network | 93.8% | 93.1% | 94.5% | 93.8% |
| **Ensemble (Final)** | **94.2%** | **93.7%** | **94.7%** | **94.2%** |

![AI Classification](https://github.com/user-attachments/assets/0a4242ae-a959-4119-8982-f360186c9939)
*Figure 3: Classification Dashboard (94.2% Accuracy)*

### 3) Geospatial Intelligence Integration

CAMEROON - 10 REGIONS MONITORED

Far North (Extrême-Nord) ████████████ 89.3%
Northwest (Nord-Ouest) ███████████ 88.7%
Southwest (Sud-Ouest) ███████████ 87.2%
East (Est) ██████████ 86.1%
North (Nord) ██████████ 85.4%
Center (Centre) ██████████ 84.8%
Adamawa (Adamaoua) █████████ 83.9%
Littoral (Littoral) █████████ 82.7%
West (Ouest) █████████ 81.5%
South (Sud) █████████ 80.3%

Legend: █ = 10% accuracy increment

markdown
Copy code

- Interactive realtime map, satellite imagery, heatmaps, clustering, history overlays

![Geospatial Map](https://github.com/user-attachments/assets/f25a280c-4789-4d50-852b-14228121ccb2)
*Figure 4: Interactive Map – All 10 Regions*

### 4) Predictive Analytics with Prophet

Horizon Accuracy Use Case
1-day 91.3% Immediate planning
3-day 89.7% Short-term allocation
7-day 86.4% Weekly planning
14-day 84.9% Mid-term strategy
30-day 82.1% Monthly budgeting
90-day 76.8% Quarterly trends

makefile
Copy code

Features: seasonality, holidays, change points, confidence intervals, multi-region.

### 5) Multi-Role Access Control

ADMIN
├─ Full access, users, config, audit, export
└─ ANALYST
├─ Threat analysis, reports, annotations, field reports
└─ VIEWER
├─ Read-only dashboards, basic reports

markdown
Copy code

---

## Testing & Validation

### Testing Matrix

| Category | Strategies | Data | Environments | Pass |
|---|---|---|---|---|
| Functional | Unit/Integration/E2E | 10k+ records | Dev/Staging/Prod | 98% |
| Performance | Load/Stress/Endurance | 1–150 users | ARM/x86/Mobile | 95% |
| Security | Penetration/Auth/Enc | Attack vectors | All | 100% |
| Compatibility | Cross-browser/OS | Multi-device | Win/Linux/Android | 97% |

**Threat Collection (15+ sources)**  
Edge handling: malformed XML, timeouts, rate limits, auth failures  
- Auto-retry recovers **85%** transient failures  
- Real-time validation blocks **99.7%** malformed data

![Data Collection](https://github.com/user-attachments/assets/bc7bbb01-b847-4b2b-bac0-a2e063fbeb55)
*Figure 5: Real-Time Data Collection Monitoring*

**Classification Testing** (10k+ labeled)

Hardware comparison:  
- Oracle ARM64 (4 vCPU, 24GB): **0.3s** / 3,333 pred/min  
- Laptop i5, 8GB: **1.2s** / 833 pred/min  
- Android 4GB: **2.8s** / 357 pred/min

![AI Performance](https://github.com/user-attachments/assets/563dda2f-7459-4695-a088-3f03347fe50a)
*Figure 6: AI Performance*

**Geospatial Validation** (10k points) – clustering ≥93%, rendering <800ms

![Regional Coverage](https://github.com/user-attachments/assets/1adb5cc5-3c2f-4416-9e8c-9fababe8198d)
*Figure 7: Geospatial Coverage*

### Performance Testing

**Load** (1 → 150 users): Sub-500ms up to 100 users on ARM64.  
**Stress**: Graceful degradation; recovery time 45s.  
**Endurance**: 72h run; 99.9% uptime; no leaks.

![Load Testing](https://github.com/user-attachments/assets/e7867ca5-15d3-4378-bd4d-50a149e18ea9)
*Figure 8: Load Testing Results*

### Security Testing

All major vectors **PASS**: SQLi, XSS, CSRF, session hardening, rate limiting, MFA (TOTP), JWT, AES-256 (at rest), TLS 1.3 (in transit).

![Security](https://github.com/user-attachments/assets/0fb670fc-870e-41f1-a7cf-4c488891f4a1)
*Figure 9: Security Dashboard*

External audit: **A+ (95/100)**; 0 critical/high; medium patched; lows documented.

### Compatibility

97% cross-platform pass (Chrome/Firefox/Edge/Safari; Desktop/Mobile).

![Mobile UI](https://github.com/user-attachments/assets/296ca5d4-83a1-4923-a146-73e829dd0bfc)
*Figure 10: Mobile-Responsive Interface*

### Integration

Frontend↔Backend <200ms; Backend↔DB <50ms; Backend↔ML <300ms; overall **99.8%** success.

**Testing Summary**

TOTAL TESTS: 3,062 | PASSED: 2,976 | FAILED: 86 | RATE: 97.2%

markdown
Copy code

---

## Performance Analysis

**Objectives Achievement**: 85% exceeded; remaining achieved.

Highlights:
- **Sources**: 15+ (150% of target)
- **Accuracy**: 94.2% (↑4.2 pts over target)
- **Forecasts**: 7-day @ 86.4% (exceeds 80%)
- **Satisfaction**: 90% (↑5% over target)

**Gaps**
- High-load scalability (target 200; achieved 150).  
  - Short-term: bigger pools, caching, read replicas  
  - Long-term: 32GB RAM, sharding, LB, ORM optimizations
- Native mobile apps pending; PWA used in interim.

---

## Deployment Guide

### Requirements

**Minimum**
- 4 vCPU, 8GB RAM, 50GB SSD, Ubuntu 20.04+
- Python 3.8+, Node 18+, PostgreSQL 13+, Redis 6+

**Production (Recommended)**
- 8 vCPU (ARM64), 16–24GB RAM, 100GB NVMe
- Ubuntu 22.04, Python 3.10+, Node 20 LTS, Postgres 15+, Redis 7+
- TLS 1.3 cert

### Architecture (Prod)

Nginx (SSL/Reverse Proxy) → Frontend (3000) / Backend (8000) / ML (8001) → Postgres/Redis/Celery

![Deployment Evidence](https://github.com/user-attachments/assets/9adc61ee-4067-49af-add4-4193a8400fd6)
![Service Status](https://github.com/user-attachments/assets/d0d5fdca-f483-489d-ac87-caf8ab0877bc)
*Figure 13: Startup & Status*

### Quick Start

```bash
git clone https://github.com/Ngum12/Cameroon_Geo-conf.git
cd project-sentinel

chmod +x install.sh && ./install.sh
Postgres

bash
Copy code
sudo systemctl start postgresql && sudo systemctl enable postgresql
sudo -u postgres psql << 'EOF'
CREATE DATABASE sentinel_db;
CREATE USER sentinel_user WITH PASSWORD 'your_secure_password_here';
GRANT ALL PRIVILEGES ON DATABASE sentinel_db TO sentinel_user;
ALTER USER sentinel_user CREATEDB;
\q
EOF
Django

bash
Copy code
cd backend-api
python3 manage.py migrate
python3 manage.py createsuperuser
Env

bash
Copy code
cp .env.example .env && nano .env
Start All

bash
Copy code
chmod +x start-all.sh && ./start-all.sh
./check-services.sh
Nginx + SSL (snippet)

nginx
Copy code
# 80 -> 443 redirect + reverse proxies to 3000/8000/8001
Systemd services provided for Django, ML, Frontend.

Backup (cron)

bash
Copy code
# backup-database.sh (pg_dump + gzip + rotate 30d)
Technical Stack
Frontend
React 18, TypeScript 5, Vite 4, Tailwind, Headless UI, Heroicons, Framer Motion, Mapbox GL, Recharts, D3, React-Leaflet, React Query, Zustand, React Router, React Helmet, React Hook Form, Yup, Axios/SWR.

Backend
Django 4.2, DRF 3.14, Python 3.10, PostgreSQL 15, psycopg2, Redis 7, Celery 5.3, django-redis, CORS, JWT, ratelimit, drf-spectacular, Swagger UI, Pandas, NumPy, BS4, Requests, Gunicorn.

ML
FastAPI, Uvicorn, Pydantic, scikit-learn, Prophet, XGBoost, LightGBM, NLTK, spaCy, Transformers, TextBlob, Joblib, Pickle, ONNX, Matplotlib/Seaborn.

Infra & DevOps
Nginx, Gunicorn, Uvicorn, Docker & Compose, Oracle Cloud/AWS/Azure, systemd, journalctl, logrotate, Let’s Encrypt, UFW, Fail2ban, SSH.

Installation
Prereqs (Ubuntu/Debian)
bash
Copy code
sudo apt update && sudo apt upgrade -y
sudo apt install -y build-essential curl wget git vim
sudo apt install -y python3.10 python3.10-venv python3-pip
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -
sudo apt install -y nodejs
sudo apt install -y postgresql-15 postgresql-contrib-15
sudo apt install -y redis-server nginx
Project Setup
bash
Copy code
git clone https://github.com/Ngum12/Cameroon_Geo-conf.git
cd project-sentinel
python3 -m venv venv && source venv/bin/activate
pip install --upgrade pip setuptools wheel
Backend

bash
Copy code
cd backend-api
pip install -r requirements.txt
pip install prophet scikit-learn pandas numpy
cp .env.example .env && nano .env
python manage.py migrate
python manage.py createsuperuser
python manage.py collectstatic --noinput
python manage.py runserver
requirements.txt

ini
Copy code
Django==4.2.5
djangorestframework==3.14.0
psycopg2-binary==2.9.7
redis==5.0.0
celery==5.3.1
django-cors-headers==4.2.0
django-redis==5.3.0
gunicorn==21.2.0
pandas==2.1.0
numpy==1.25.2
scikit-learn==1.3.0
prophet==1.1.4
beautifulsoup4==4.12.2
requests==2.31.0
python-dotenv==1.0.0
Pillow==10.0.0
ML API

bash
Copy code
cd ../ml-models
pip install fastapi uvicorn pydantic
pip install scikit-learn prophet xgboost lightgbm
python -m uvicorn prediction_api:app --reload
Frontend

bash
Copy code
cd ../frontend-dashboard
npm install
cp .env.example .env && nano .env
npm run build
npm run dev
package.json (key deps)

json
Copy code
{
  "dependencies": {
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "react-router-dom": "^6.15.0",
    "typescript": "^5.2.2",
    "tailwindcss": "^3.3.3",
    "mapbox-gl": "^2.15.0",
    "recharts": "^2.8.0",
    "axios": "^1.5.0",
    "zustand": "^4.4.1",
    "@tanstack/react-query": "^4.35.0"
  },
  "devDependencies": {
    "vite": "^4.4.9",
    "@vitejs/plugin-react": "^4.0.4"
  }
}
Redis

bash
Copy code
sudo systemctl start redis-server && sudo systemctl enable redis-server
redis-cli ping
Dev Mode (multi-terminals)

bash
Copy code
# Backend
cd backend-api && source ../venv/bin/activate && python manage.py runserver 0.0.0.0:8000

# ML
cd ml-models && source ../venv/bin/activate && uvicorn prediction_api:app --host 0.0.0.0 --port 8001 --reload

# Frontend
cd frontend-dashboard && npm run dev -- --host 0.0.0.0 --port 3000

# Celery (optional)
cd backend-api && source ../venv/bin/activate && celery -A sentinel_core worker -l info
API Documentation
Auth (JWT)
http
Copy code
POST /api/auth/login/
Content-Type: application/json
{
  "username": "your_username",
  "password": "your_password"
}
Use: Authorization: Bearer <access>.

Threat Intelligence
http
Copy code
GET /api/threats/?page=1&page_size=20&severity=high&region=Extrême-Nord&date_from=YYYY-MM-DD&date_to=YYYY-MM-DD
GET /api/threats/{id}/
POST /api/threats/
PUT/PATCH/DELETE /api/threats/{id}/
Geospatial
http
Copy code
GET /api/regions/{region_name}/threats/
GET /api/locations/
GET /api/clusters/?zoom=...&bounds=...
GET /api/regions/statistics/
Analytics
http
Copy code
GET /api/analytics/statistics/?period=day|week|month|year&region=...
GET /api/analytics/trends/?days=30&region=...
GET /api/analytics/forecasts/?region=Extrême-Nord&days=7
ML
http
Copy code
POST /ml/predict/threat-classification/
POST /ml/predict/sentiment/
POST /ml/predict/risk-assessment/
Rate Limits
Anonymous: 100/hr

Authenticated: 1000/hr

Admin: 5000/hr

ML API: 500 predictions/hr/user

Error Examples
json
Copy code
{"error":"validation_error","message":"Invalid input data","details":{"severity":["This field is required"]}}
{"error":"authentication_failed","message":"Invalid or expired token"}
{"error":"permission_denied","message":"You do not have permission to perform this action"}
{"error":"not_found","message":"Threat with id 999 not found"}
{"error":"rate_limit_exceeded","message":"Rate limit exceeded. Try again in 3600 seconds"}
{"error":"internal_server_error","message":"An unexpected error occurred","request_id":"abc123def456"}
Contributing
Workflow
Fork → 2. Clone → 3. Branch → 4. Code + Tests + Docs → 5. Test → 6. Commit
→ 7. Push → 8. PR → 9. Review → 10. Merge

Code Standards
Python (PEP8)

python
Copy code
def calculate_threat_score(severity: str, confidence: float, region: str) -> float:
    """Calculate threat score based on severity, confidence, and region."""
    base_score = SEVERITY_WEIGHTS[severity]
    confidence_factor = confidence * 100
    regional_factor = REGIONAL_MULTIPLIERS.get(region, 1.0)
    return base_score * confidence_factor * regional_factor
TypeScript (ESLint)

ts
Copy code
interface ThreatData {
  id: number;
  title: string;
  severity: 'high' | 'medium' | 'low';
  region: string;
  confidence: number;
}

const fetchThreats = async (filters: ThreatFilters): Promise<ThreatData[]> => {
  const response = await axios.get('/api/threats/', { params: filters });
  return response.data.results;
};
pgsql
Copy code

Want me to also generate a **compact version** for GitHub’s mobile view (shorter images, smaller tables), or keep this full version as your default?

