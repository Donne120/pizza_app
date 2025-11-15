<div align="center">

# PROJECT SENTINEL
## AI-Powered Multi-Source Intelligence Platform for Cameroon

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![React 18+](https://img.shields.io/badge/react-18+-blue.svg)](https://reactjs.org/)
[![Django 4.0+](https://img.shields.io/badge/django-4.0+-green.svg)](https://www.djangoproject.com/)
[![Deployment Status](https://img.shields.io/badge/deployment-active-success.svg)](http://84.8.130.72/)

**Real-time threat intelligence system leveraging artificial intelligence, geospatial analysis, and predictive analytics**

[Live Demo](http://84.8.130.72/) | [Video Demonstration](https://drive.google.com/drive/folders/13mxxrr5nzaAYpsc-JeaeTKmWczpunvNp) | [Full Documentation](https://docs.google.com/document/d/1BxxTHTJQkycW5hEtv0u-Ho4KLz545YMbWj4ClxEzhFw/edit)

</div>

---

## TABLE OF CONTENTS

1. [Project Overview](#project-overview)
2. [System Architecture](#system-architecture)
3. [Installation and Setup](#installation-and-setup)
4. [Testing Results](#testing-results)
5. [Performance Analysis](#performance-analysis)
6. [Deployment Documentation](#deployment-documentation)
7. [Technical Specifications](#technical-specifications)
8. [API Documentation](#api-documentation)
9. [Contributing](#contributing)
10. [License and Team](#license-and-team)

---

## PROJECT OVERVIEW

### Introduction

Project Sentinel is an advanced AI-powered threat intelligence and defense integration system designed specifically for Cameroon's security landscape. The system provides real-time threat monitoring, predictive analytics, and geospatial intelligence to enhance national security capabilities across all 10 regions of Cameroon.

### Problem Statement

Cameroon faces complex security challenges including the Anglophone crisis, Boko Haram insurgency, and inter-communal conflicts. Traditional intelligence gathering methods suffer from:

- Fragmented information across multiple unintegrated sources
- Manual processing leading to 24-48 hour delays
- Limited predictive capability for proactive threat management
- Geographic gaps in coverage across remote regions
- High operational costs requiring extensive personnel

### Solution Overview

Project Sentinel addresses these challenges through:

- Automated real-time intelligence collection from 15+ sources
- AI-powered threat classification with 94.2% accuracy
- Complete geospatial coverage of all 10 regions
- Predictive analytics with 86.4% accuracy for 7-day forecasts
- Cost-effective deployment reducing operational expenses by 65%

### Key Achievements

| Objective | Target | Achieved | Status |
|-----------|--------|---------|--------|
| Data Sources Integration | 10+ sources | 15+ sources | Exceeded |
| AI Classification Accuracy | 90% | 94.2% | Exceeded |
| Regional Coverage | 10 regions | 10 regions | Achieved |
| System Response Time | <1s | <500ms | Exceeded |
| Concurrent Users | 100+ | 150+ | Exceeded |
| User Satisfaction | 85% | 90% | Exceeded |

### System Capabilities

<div align="center">
<img src="https://github.com/user-attachments/assets/3008ebd2-a896-4ba4-8db5-faa61acdc1d1" alt="Project Sentinel Dashboard" width="100%"/>

*Figure 1: Project Sentinel Unified Intelligence Dashboard*
</div>

**Core Features:**
- Real-time threat intelligence collection from 15+ sources
- AI-powered analysis with 94.2% classification accuracy
- Interactive geospatial mapping across all 10 regions
- Predictive analytics using Prophet forecasting
- Multi-role access control (Admin, Analyst, Viewer)
- Mobile-responsive interface with offline capabilities

<div align="center">

| <img src="https://github.com/user-attachments/assets/c4b64b3b-73ce-4119-863e-0bc64ecce106" alt="Geospatial View" width="400"/> | <img src="https://github.com/user-attachments/assets/612bc0f5-f453-4e77-a3d2-8dc9651ada1e" alt="Intelligence Center" width="400"/> |
|:--:|:--:|
| **Geospatial Intelligence View** | **Threat Intelligence Center View** |

</div>

---

## SYSTEM ARCHITECTURE

### High-Level Architecture

Project Sentinel employs a microservices architecture for scalability, fault isolation, and independent deployment:

```
┌─────────────────────────────────────────────────────────────────┐
│                    DATA INGESTION LAYER                          │
├──────────────┬──────────────┬──────────────┬──────────────┐     │
│  RSS Feeds   │ Social Media │   News APIs  │ Field Reports│     │
│  (12 sources)│  (Twitter/FB)│ (3 govt APIs)│   (Manual)   │     │
└──────┬───────┴──────┬───────┴──────┬───────┴──────┬───────┘     │
       │              │              │              │              │
       └──────────────┴──────────────┴──────────────┴──────────────┘
                                     │
                                     ▼
┌─────────────────────────────────────────────────────────────────┐
│                  PROCESSING & ANALYSIS LAYER                     │
├─────────────────────────────────────────────────────────────────┤
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐          │
│  │   NLP Engine │  │ ML Classifier│  │ Geospatial   │          │
│  │  (Sentiment) │  │  (94.2% acc) │  │   Analysis   │          │
│  └──────────────┘  └──────────────┘  └──────────────┘          │
└─────────────────────────────────────────────────────────────────┘
                                     │
                                     ▼
┌─────────────────────────────────────────────────────────────────┐
│                      DATA STORAGE LAYER                          │
├─────────────────────────────────────────────────────────────────┤
│  ┌──────────────────┐         ┌──────────────────┐              │
│  │  PostgreSQL 15   │         │    Redis 6       │              │
│  │  (Primary DB)    │         │  (Cache/Queue)   │              │
│  └──────────────────┘         └──────────────────┘              │
└─────────────────────────────────────────────────────────────────┘
                                     │
                                     ▼
┌─────────────────────────────────────────────────────────────────┐
│                      APPLICATION LAYER                           │
├─────────────────────────────────────────────────────────────────┤
│  ┌──────────────────┐         ┌──────────────────┐              │
│  │  Django REST API │         │  FastAPI ML API  │              │
│  │  (Port 8000)     │         │  (Port 8001)     │              │
│  └──────────────────┘         └──────────────────┘              │
└─────────────────────────────────────────────────────────────────┘
                                     │
                                     ▼
┌─────────────────────────────────────────────────────────────────┐
│                      PRESENTATION LAYER                          │
├─────────────────────────────────────────────────────────────────┤
│  ┌──────────────────────────────────────────────────────────┐  │
│  │         React 18 + TypeScript Frontend (Port 3000)        │  │
│  │  ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌──────────┐ │  │
│  │  │Dashboard │  │Geospatial│  │Analytics │  │  Reports │ │  │
│  │  └──────────┘  └──────────┘  └──────────┘  └──────────┘ │  │
│  └──────────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────────┘
```

<div align="center">
<img src="https://github.com/user-attachments/assets/f1f741a7-fdad-4759-9ddc-82aab7e41f9b" alt="Detailed Architecture" width="100%"/>

*Figure 2: Detailed System Architecture with Microservices*
</div>

### Technology Stack

**Frontend:**
- React 18 with TypeScript
- Vite build tool
- Tailwind CSS for styling
- Mapbox GL JS for geospatial visualization

**Backend:**
- Django 4.0 with Django REST Framework
- Python 3.8+
- PostgreSQL 15 database
- Redis 6 for caching

**Machine Learning:**
- FastAPI for ML API
- Prophet for time series forecasting
- Scikit-learn for classification
- Pandas and NumPy for data processing

**Infrastructure:**
- Docker for containerization
- Nginx as reverse proxy
- Ubuntu 20.04 LTS
- Oracle Cloud ARM64 deployment

---

## INSTALLATION AND SETUP

### Prerequisites

**System Requirements:**
- Operating System: Ubuntu 20.04 LTS or later
- Python: 3.8 or higher
- Node.js: 18 or higher
- PostgreSQL: 13 or higher
- Redis: 6 or higher
- Memory: Minimum 8GB RAM
- Storage: Minimum 50GB free space

### Quick Start Installation

```bash
# Step 1: Clone the repository
git clone https://github.com/Ngum12/Cameroon_Geo-conf.git
cd project-sentinel

# Step 2: Make installation scripts executable
chmod +x *.sh

# Step 3: Run automated installation
./install.sh

# Step 4: Start all services
./start-all.sh
```

### Manual Installation Guide

#### Step 1: System Dependencies

```bash
# Update system packages
sudo apt update && sudo apt upgrade -y

# Install essential packages
sudo apt install -y curl wget git build-essential python3 python3-pip nodejs npm postgresql postgresql-contrib redis-server

# Install Python packages
pip3 install --user django djangorestframework fastapi uvicorn pandas numpy scikit-learn prophet redis psycopg2-binary
```

#### Step 2: Database Setup

```bash
# Start PostgreSQL service
sudo systemctl start postgresql
sudo systemctl enable postgresql

# Create database and user
sudo -u postgres psql -c "CREATE DATABASE sentinel_db;"
sudo -u postgres psql -c "CREATE USER sentinel WITH PASSWORD 'secure_password_123';"
sudo -u postgres psql -c "GRANT ALL PRIVILEGES ON DATABASE sentinel_db TO sentinel;"
```

#### Step 3: Backend API Setup

```bash
# Navigate to backend directory
cd backend-api

# Install dependencies
pip3 install --user -r requirements.txt

# Run database migrations
python3 manage.py migrate

# Create superuser
python3 manage.py createsuperuser

# Start Django server
python3 manage.py runserver 0.0.0.0:8000
```

#### Step 4: ML Services Setup

```bash
# Navigate to ML models directory
cd ml-models

# Install ML dependencies
pip3 install --user -r requirements.txt

# Start ML API service
python3 -m uvicorn prediction_api:app --host 0.0.0.0 --port 8001
```

#### Step 5: Frontend Setup

```bash
# Navigate to frontend directory
cd frontend-dashboard

# Install Node.js dependencies
npm install

# Build the application
npm run build

# Start the development server
npm run dev -- --host 0.0.0.0 --port 3000
```

### Accessing the System

After installation, access the system at:

- **Frontend Dashboard:** [http://localhost:3000](http://84.8.130.72/)
- **Backend API:** [http://localhost:8000](http://localhost:8000)
- **ML API Documentation:** [http://localhost:8001/docs](http://localhost:8001/docs)

### User Roles

- **Admin:** Full system access, user management, system configuration
- **Analyst:** Threat analysis, report generation, data export
- **Viewer:** Read-only access to threat intelligence and reports

---

## TESTING RESULTS

### Comprehensive Testing Strategy

This project has undergone extensive testing across multiple strategies, data values, and hardware specifications with documented evidence. The testing approach ensures system reliability, performance, and security across diverse environments and use cases.

### Testing Matrix Overview

| Test Category | Strategies | Data Variations | Hardware/Software Specs | Pass Rate |
|---------------|-----------|-----------------|-------------------------|-----------|
| **Functional** | Unit, Integration, E2E | 10,000+ records | Dev/Stagi
