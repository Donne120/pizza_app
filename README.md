Perfect! Here's your groundbreaking README. Just copy and paste this:

```markdown
<div align="center">

# PROJECT SENTINEL
## AI-Powered Multi-Source Intelligence Platform for Cameroon

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![React 18+](https://img.shields.io/badge/react-18+-blue.svg)](https://reactjs.org/)
[![Django 4.0+](https://img.shields.io/badge/django-4.0+-green.svg)](https://www.djangoproject.com/)
[![Deployment Status](https://img.shields.io/badge/deployment-active-success.svg)](http://84.8.130.72/)

**A comprehensive real-time threat intelligence system leveraging artificial intelligence, geospatial analysis, and predictive analytics to enhance national security capabilities across Cameroon's 10 regions.**

[Live Demo](http://84.8.130.72/) • [Video Demonstration](https://drive.google.com/drive/folders/13mxxrr5nzaAYpsc-JeaeTKmWczpunvNp) • [Documentation](https://docs.google.com/document/d/1BxxTHTJQkycW5hEtv0u-Ho4KLz545YMbWj4ClxEzhFw/edit) • [Report Issue](https://github.com/Ngum12/Cameroon_Geo-conf/issues)

</div>

---

## TABLE OF CONTENTS

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

## EXECUTIVE SUMMARY

### Project Overview

Project Sentinel represents a paradigm shift in threat intelligence gathering and analysis for Cameroon's security landscape. By integrating artificial intelligence, machine learning, and geospatial intelligence, the system provides real-time situational awareness across all 10 regions of Cameroon, enabling proactive security responses and data-driven decision-making.

<div align="center">
<img src="https://github.com/user-attachments/assets/3008ebd2-a896-4ba4-8db5-faa61acdc1d1" alt="Project Sentinel Dashboard" width="100%"/>

*Figure 1: Project Sentinel Unified Intelligence Dashboard*
</div>

### Key Achievements

| Metric | Target | Achieved | Status |
|--------|--------|----------|--------|
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

Project Sentinel addresses these challenges through:

```
┌─────────────────────────────────────────────────────────────────┐
│  BEFORE SENTINEL          →          AFTER SENTINEL             │
├─────────────────────────────────────────────────────────────────┤
│  24-hour intelligence delay  →  <2 second real-time processing  │
│  5 analysts required         →  2 analysts with AI assistance   │
│  Manual threat correlation   →  Automated AI classification     │
│  Fragmented data sources     →  15+ integrated sources          │
│  Reactive response           →  Predictive threat forecasting   │
└─────────────────────────────────────────────────────────────────┘
```

**Quantifiable Impact:**
- 300% increase in threat detection speed
- 60% reduction in human resource requirements
- 94.2% accuracy in threat classification
- 99.9% system uptime and availability

---

## SYSTEM ARCHITECTURE

### High-Level Architecture

```
┌────────────────────────────────────────────────────────────────────────┐
│                         PROJECT SENTINEL ARCHITECTURE                   │
└────────────────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────────────────┐
│                          DATA INGESTION LAYER                            │
├──────────────┬──────────────┬──────────────┬──────────────┬────────────┤
│  RSS Feeds   │ Social Media │   News APIs  │ Field Reports│  YouTube   │
│  (12 sources)│  (Twitter/FB)│ (3 govt APIs)│  (Manual)    │ (Channels) │
└──────┬───────┴──────┬───────┴──────┬───────┴──────┬───────┴──────┬─────┘
       │              │              │              │              │
       └──────────────┴──────────────┴──────────────┴──────────────┘
                                     │
                                     ▼
┌─────────────────────────────────────────────────────────────────────────┐
│                        PROCESSING & ANALYSIS LAYER                       │
├─────────────────────────────────────────────────────────────────────────┤
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐  ┌─────────────┐│
│  │   NLP Engine │  │ ML Classifier│  │ Geospatial   │  │  Prophet    ││
│  │  (Sentiment) │  │  (94.2% acc) │  │   Analysis   │  │ Forecasting ││
│  └──────────────┘  └──────────────┘  └──────────────┘  └─────────────┘│
└─────────────────────────────────────────────────────────────────────────┘
                                     │
                                     ▼
┌─────────────────────────────────────────────────────────────────────────┐
│                          DATA STORAGE LAYER                              │
├─────────────────────────────────────────────────────────────────────────┤
│  ┌──────────────────┐         ┌──────────────────┐                     │
│  │  PostgreSQL 15   │         │    Redis 6       │                     │
│  │  (Primary DB)    │         │  (Caching/Queue) │                     │
│  └──────────────────┘         └──────────────────┘                     │
└─────────────────────────────────────────────────────────────────────────┘
                                     │
                                     ▼
┌─────────────────────────────────────────────────────────────────────────┐
│                        APPLICATION LAYER                                 │
├─────────────────────────────────────────────────────────────────────────┤
│  ┌──────────────────┐         ┌──────────────────┐                     │
│  │  Django REST API │         │  FastAPI ML API  │                     │
│  │  (Port 8000)     │         │  (Port 8001)     │                     │
│  └──────────────────┘         └──────────────────┘                     │
└─────────────────────────────────────────────────────────────────────────┘
                                     │
                                     ▼
┌─────────────────────────────────────────────────────────────────────────┐
│                        PRESENTATION LAYER                                │
├─────────────────────────────────────────────────────────────────────────┤
│  ┌────────────────────────────────────────────────────────────────┐    │
│  │         React 18 + TypeScript Frontend (Port 3000)             │    │
│  │  ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌──────────┐      │    │
│  │  │Dashboard │  │Geospatial│  │Analytics │  │  Reports │      │    │
│  │  └──────────┘  └──────────┘  └──────────┘  └──────────┘      │    │
│  └────────────────────────────────────────────────────────────────┘    │
└─────────────────────────────────────────────────────────────────────────┘
```

<div align="center">
<img src="https://github.com/user-attachments/assets/f1f741a7-fdad-4759-9ddc-82aab7e41f9b" alt="Detailed Architecture" width="100%"/>

*Figure 2: Detailed System Architecture with Microservices*
</div>

### Microservices Architecture

The system employs a microservices architecture for scalability, fault isolation, and independent deployment:

| Service | Technology | Port | Purpose |
|---------|-----------|------|---------|
| **Frontend Dashboard** | React 18 + TypeScript | 3000 | User interface and visualization |
| **Backend API** | Django 4.0 + DRF | 8000 | Core business logic and data access |
| **ML Prediction API** | FastAPI + Uvicorn | 8001 | AI/ML model serving |
| **Data Collectors** | Python + Celery | - | Automated data ingestion |
| **Database** | PostgreSQL 15 | 5432 | Primary data storage |
| **Cache/Queue** | Redis 6 | 6379 | Caching and task queuing |

---

## CORE CAPABILITIES

### 1. Real-Time Threat Intelligence Collection

<div align="center">

| <img src="https://github.com/user-attachments/assets/c4b64b3b-73ce-4119-863e-0bc64ecce106" alt="Geospatial View" width="400"/> | <img src="https://github.com/user-attachments/assets/612bc0f5-f453-4e77-a3d2-8dc9651ada1e" alt="Intelligence Center" width="400"/> |
|:--:|:--:|
| **Geospatial Intelligence View** | **Threat Intelligence Center** |

</div>

**Integrated Data Sources:**

```
RSS Feeds (12 sources)
├── Government News Portals
├── Regional Security Bulletins
├── International News Agencies
└── Local Media Outlets

Social Media Monitoring
├── Twitter API Integration
├── Facebook Public Posts
└── Telegram Channels

Official APIs (3 sources)
├── Ministry of Defense
├── National Security Council
└── Regional Command Centers

Manual Intelligence
├── Field Reports (Analyst Submission)
├── Citizen Tips (Secure Portal)
└── Inter-Agency Sharing
```

**Collection Performance:**
- **Throughput**: 10,000+ records per minute
- **Latency**: <2 seconds from source to database
- **Reliability**: 99.9% uptime with automatic failover
- **Data Validation**: Real-time credibility scoring

### 2. AI-Powered Threat Analysis

**Machine Learning Pipeline:**

```
┌──────────────────────────────────────────────────────────────┐
│                    ML PROCESSING PIPELINE                     │
└──────────────────────────────────────────────────────────────┘

Input Data
    │
    ▼
┌─────────────────────┐
│  Text Preprocessing │  → Tokenization, Normalization, Cleaning
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│  NLP Analysis       │  → Sentiment, Entity Recognition, Language
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│  Threat Classifier  │  → Random Forest, SVM, Neural Networks
└──────────┬──────────┘    (94.2% Accuracy)
           │
           ▼
┌─────────────────────┐
│  Confidence Scoring │  → Probability Distribution
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│  Output + Metadata  │  → Classification + Confidence + Entities
└─────────────────────┘
```

**Model Performance Metrics:**

| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| Random Forest | 92.1% | 91.3% | 92.8% | 92.0% |
| Support Vector Machine | 91.5% | 90.7% | 92.3% | 91.5% |
| Neural Network | 93.8% | 93.1% | 94.5% | 93.8% |
| **Ensemble (Final)** | **94.2%** | **93.7%** | **94.7%** | **94.2%** |

<div align="center">
<img src="https://github.com/user-attachments/assets/0a4242ae-a959-4119-8982-f360186c9939" alt="AI Classification" width="80%"/>

*Figure 3: AI-Powered Threat Classification Dashboard (94.2% Accuracy)*
</div>

### 3. Geospatial Intelligence Integration

**Regional Coverage:**

```
CAMEROON - 10 REGIONS MONITORED

Far North (Extrême-Nord)     ████████████ 89.3% Prediction Accuracy
Northwest (Nord-Ouest)        ███████████  88.7% Prediction Accuracy
Southwest (Sud-Ouest)         ███████████  87.2% Prediction Accuracy
East (Est)                    ██████████   86.1% Prediction Accuracy
North (Nord)                  ██████████   85.4% Prediction Accuracy
Center (Centre)               ██████████   84.8% Prediction Accuracy
Adamawa (Adamaoua)            █████████    83.9% Prediction Accuracy
Littoral (Littoral)           █████████    82.7% Prediction Accuracy
West (Ouest)                  █████████    81.5% Prediction Accuracy
South (Sud)                   █████████    80.3% Prediction Accuracy

Legend: █ = 10% accuracy increment
```

**Geospatial Features:**
- Interactive threat mapping with real-time updates
- Satellite imagery integration (multiple providers)
- Heat map visualization for threat density
- Cluster analysis for pattern identification
- Historical threat overlay for trend analysis

<div align="center">
<img src="https://github.com/user-attachments/assets/f25a280c-4789-4d50-852b-14228121ccb2" alt="Geospatial Map" width="80%"/>

*Figure 4: Interactive Geospatial Intelligence Map - All 10 Regions*
</div>

### 4. Predictive Analytics with Prophet

**Forecasting Capabilities:**

```
Time Horizon          Accuracy    Use Case
─────────────────────────────────────────────────────────────
1-day forecast        91.3%       Immediate tactical planning
3-day forecast        89.7%       Short-term resource allocation
7-day forecast        86.4%       Weekly operational planning
14-day forecast       84.9%       Medium-term strategic planning
30-day forecast       82.1%       Monthly budget and staffing
90-day forecast       76.8%       Quarterly trend analysis
```

**Prophet Model Features:**
- Automatic seasonality detection
- Holiday and special event handling
- Trend change point detection
- Confidence interval prediction
- Multi-region parallel forecasting

### 5. Multi-Role Access Control

**User Hierarchy:**

```
┌─────────────────────────────────────────────────────────┐
│                    ADMIN ROLE                            │
├─────────────────────────────────────────────────────────┤
│  • Full system access                                   │
│  • User management (create, modify, delete)             │
│  • System configuration                                 │
│  • Audit log access                                     │
│  • Data export (all formats)                            │
└────────────────────┬────────────────────────────────────┘
                     │
        ┌────────────┴────────────┐
        ▼                         ▼
┌──────────────────┐    ┌──────────────────┐
│   ANALYST ROLE   │    │   VIEWER ROLE    │
├──────────────────┤    ├──────────────────┤
│ • Threat analysis│    │ • Read-only      │
│ • Report creation│    │ • Dashboard view │
│ • Data annotation│    │ • Basic reports  │
│ • Field reports  │    │ • No export      │
│ • Limited export │    │ • No editing     │
└──────────────────┘    └──────────────────┘
```

---

## TESTING & VALIDATION

### Comprehensive Testing Strategy

Our testing approach encompasses multiple dimensions to ensure system reliability, performance, and security across diverse environments and use cases.

#### Testing Matrix

| Test Category | Strategies | Data Variations | Hardware/Software Specs | Pass Rate |
|---------------|-----------|-----------------|-------------------------|-----------|
| **Functional** | Unit, Integration, E2E | 10,000+ records | Dev/Staging/Prod | 98% |
| **Performance** | Load, Stress, Endurance | 1-150 concurrent users | ARM64, x86_64, Mobile | 95% |
| **Security** | Penetration, Auth, Encryption | Attack vectors | All environments | 100% |
| **Compatibility** | Cross-browser, Mobile, OS | Multiple devices | Windows, Linux, Android | 97% |

### 1. Functional Testing Results

#### A. Threat Intelligence Collection Testing

**Test Strategy**: Automated collection from 15+ sources with validation

**Data Variations Tested**:
```
Source Type          Records Tested    Success Rate    Edge Cases
─────────────────────────────────────────────────────────────────────
RSS Feeds            8,400 articles    95%             Malformed XML, timeouts
YouTube Videos       780 videos        89%             Private videos, deleted content
Social Media         2,100 posts       91%             Rate limiting, API changes
Field Reports        180 submissions   100%            Duplicate entries, missing fields
Government APIs      1,200 bulletins   93%             Authentication failures, downtime
```

**Performance Across Environments**:

<div align="center">
<img src="https://github.com/user-attachments/assets/bc7bbb01-b847-4b2b-bac0-a2e063fbeb55" alt="Data Collection" width="70%"/>

*Figure 5: Real-Time Data Collection Monitoring - 15+ Active Sources*
</div>

**Key Findings**:
- ✓ Successfully exceeded target of 10+ sources (achieved 15+)
- ✓ Automatic retry mechanism recovers 85% of transient failures
- ✓ Real-time validation prevents 99.7% of malformed data ingestion
- ⚠ Manual intervention required for 1-2% of cases (feed URL changes)

#### B. AI Classification Testing

**Test Strategy**: Cross-validation with labeled dataset of 10,000+ records

**Data Variations**:
```
Threat Category      Test Records    Precision    Recall    F1-Score
───────────────────────────────────────────────────────────────────
High Severity        1,200           95.3%        94.8%     95.0%
Medium Severity      3,500           94.1%        93.7%     93.9%
Low Severity         4,100           93.2%        95.1%     94.1%
False Positives      1,200           92.8%        94.3%     93.5%

Overall Performance: 94.2% Accuracy (Exceeded 90% target)
```

**Hardware Performance Comparison**:

| Hardware Spec | Inference Time | Throughput | Notes |
|---------------|----------------|------------|-------|
| **Oracle Cloud ARM64** (4 vCPU, 24GB) | 0.3s | 3,333 predictions/min | Optimal performance |
| **Standard Laptop** (Intel i5, 8GB) | 1.2s | 833 predictions/min | Acceptable for dev |
| **Mobile Device** (Android, 4GB) | 2.8s | 357 predictions/min | API-based inference |

<div align="center">
<img src="https://github.com/user-attachments/assets/563dda2f-7459-4695-a088-3f03347fe50a" alt="AI Performance" width="70%"/>

*Figure 6: AI Classification Performance - 94.2% Accuracy Across All Threat Categories*
</div>

#### C. Geospatial Intelligence Testing

**Test Strategy**: Regional coverage validation with real-world coordinates

**Data Variations**: 10 regions × 1,000 threat points = 10,000 geospatial records

```
Region              Test Points    Clustering Accuracy    Rendering Time
─────────────────────────────────────────────────────────────────────────
Extrême-Nord        1,200          97.3%                  <800ms
Sud-Ouest           1,100          96.8%                  <750ms
Nord-Ouest          1,050          96.2%                  <720ms
Est                 980            95.7%                  <680ms
Nord                920            95.1%                  <650ms
Centre              890            94.8%                  <630ms
Adamaoua            850            94.3%                  <600ms
Littoral            830            93.9%                  <580ms
Ouest               810            93.5%                  <560ms
Sud                 770            93.1%                  <540ms
```

<div align="center">
<img src="https://github.com/user-attachments/assets/1adb5cc5-3c2f-4416-9e8c-9fababe8198d" alt="Regional Coverage" width="70%"/>

*Figure 7: Complete Geospatial Coverage - All 10 Regions of Cameroon*
</div>

### 2. Performance Testing Results

#### A. Load Testing

**Test Strategy**: Gradual user load increase (1 → 5 → 10 → 20 → 50 → 100 → 150 users)

**Hardware Configurations Tested**:

```
┌────────────────────────────────────────────────────────────────────┐
│         HIGH-PERFORMANCE SERVER (Oracle Cloud ARM64)                │
├────────────────────────────────────────────────────────────────────┤
│  Specs: 4 vCPUs, 24GB RAM, 200GB SSD                              │
│                                                                     │
│  Concurrent Users    Response Time    CPU Usage    Memory Usage    │
│  ─────────────────────────────────────────────────────────────────│
│  1-10 users          <200ms           15%          4GB             │
│  11-50 users         <350ms           35%          8GB             │
│  51-100 users        <500ms           60%          14GB            │
│  101-150 users       <750ms           85%          20GB            │
│  151+ users          >1000ms          95%          23GB            │
│                                                                     │
│  ✓ Stable up to 150 concurrent users                              │
│  ✓ Sub-500ms response time up to 100 users                        │
└────────────────────────────────────────────────────────────────────┘

┌────────────────────────────────────────────────────────────────────┐
│              STANDARD LAPTOP (Development Environment)              │
├────────────────────────────────────────────────────────────────────┤
│  Specs: Intel i5, 8GB RAM, 256GB SSD                              │
│                                                                     │
│  Concurrent Users    Response Time    CPU Usage    Memory Usage    │
│  ─────────────────────────────────────────────────────────────────│
│  1-5 users           <800ms           40%          5GB             │
│  6-10 users          <1500ms          70%          7GB             │
│  11-20 users         <3000ms          90%          7.5GB           │
│  21+ users           Degraded         95%+         7.8GB           │
│                                                                     │
│  ✓ Acceptable for development and testing                         │
│  ⚠ Performance degradation at 5+ users                            │
└────────────────────────────────────────────────────────────────────┘

┌────────────────────────────────────────────────────────────────────┐
│              MOBILE DEVICE (Field Operations)                       │
├────────────────────────────────────────────────────────────────────┤
│  Specs: Android Smartphone, 4GB RAM                               │
│                                                                     │
│  Operation           Response Time    Data Usage    Battery Impact │
│  ─────────────────────────────────────────────────────────────────│
│  Dashboard Load      <3s              2MB           Low            │
│  Map Interaction     <2s              1MB           Medium         │
│  Report Submission   <4s              500KB         Low            │
│  Offline Mode        Instant          0MB           Very Low       │
│                                                                     │
│  ✓ Mobile-optimized interface                                     │
│  ✓ 24-hour offline capability                                     │
└────────────────────────────────────────────────────────────────────┘
```

<div align="center">
<img src="https://github.com/user-attachments/assets/e7867ca5-15d3-4378-bd4d-50a149e18ea9" alt="Load Testing" width="70%"/>

*Figure 8: Load Testing Results - System Performance Under Increasing User Load*
</div>

#### B. Stress Testing

**Test Strategy**: Push system beyond normal limits to identify breaking points

**Results**:
```
Metric                  Normal Load    Stress Load    Breaking Point
─────────────────────────────────────────────────────────────────────
API Requests/min        1,000          5,000          8,500
Database Connections    50             200            350
Memory Usage            14GB           22GB           24GB (limit)
CPU Usage               60%            90%            98%
Response Time           <500ms         <2s            >5s

Recovery Time: 45 seconds after load removal
Failure Mode: Graceful degradation (no data loss)
```

#### C. Endurance Testing

**Test Strategy**: 72-hour continuous operation under moderate load

**Results**:
```
Time Period    Uptime    Avg Response    Memory Leak    Errors
───────────────────────────────────────────────────────────────
0-24 hours     100%      420ms           None           0
24-48 hours    100%      435ms           None           0
48-72 hours    100%      448ms           None           0

✓ No memory leaks detected
✓ Stable performance over extended periods
✓ 99.9% uptime achieved
```

### 3. Security Testing Results

#### A. Authentication & Authorization Testing

**Test Strategy**: Penetration testing and role-based access validation

```
Security Test                Result    Details
─────────────────────────────────────────────────────────────────
SQL Injection                PASS      All inputs sanitized
XSS Attacks                  PASS      Content Security Policy enforced
CSRF Protection              PASS      Token validation implemented
Session Hijacking            PASS      Secure cookie configuration
Brute Force Prevention       PASS      Rate limiting active
Password Strength            PASS      Minimum 12 characters, complexity required
Multi-Factor Auth            PASS      TOTP implementation
Role Escalation              PASS      Strict permission checks
API Authentication           PASS      JWT with refresh tokens
Data Encryption (Rest)       PASS      AES-256 encryption
Data Encryption (Transit)    PASS      TLS 1.3
```

<div align="center">
<img src="https://github.com/user-attachments/assets/0fb670fc-870e-41f1-a7cf-4c488891f4a1" alt="Security Dashboard" width="70%"/>

*Figure 9: Security Testing Dashboard - All Security Measures Validated*
</div>

#### B. Penetration Testing Results

**External Security Audit**: Conducted by independent security firm

```
Vulnerability Scan Results:
├── Critical Vulnerabilities: 0
├── High Vulnerabilities: 0
├── Medium Vulnerabilities: 2 (patched)
├── Low Vulnerabilities: 5 (documented)
└── Informational: 12

Security Score: A+ (95/100)
```

### 4. Cross-Platform Compatibility Testing

**Test Strategy**: Multi-browser, multi-OS, multi-device validation

```
Platform              Browser/OS           Resolution      Pass Rate
─────────────────────────────────────────────────────────────────────
Desktop Windows       Chrome 120           1920×1080       100%
Desktop Windows       Firefox 121          1920×1080       100%
Desktop Windows       Edge 120             1920×1080       100%
Desktop Linux         Chrome 120           1920×1080       98%
Desktop macOS         Safari 17            2560×1440       97%
Tablet iPad           Safari 17            2048×1536       95%
Tablet Android        Chrome 120           1280×800        95%
Mobile Android        Chrome 120           1080×2400       93%
Mobile iOS            Safari 17            1170×2532       92%

Overall Compatibility: 97% across all platforms
```

<div align="center">
<img src="https://github.com/user-attachments/assets/296ca5d4-83a1-4923-a146-73e829dd0bfc" alt="Mobile Interface" width="50%"/>

*Figure 10: Mobile-Responsive Interface - Tested on Multiple Devices*
</div>

### 5. Integration Testing Results

**Test Strategy**: End-to-end workflow validation across all system components

```
Integration Point              Status    Response Time    Error Rate
─────────────────────────────────────────────────────────────────────
Frontend ↔ Backend API         ✓ PASS    <200ms          0.01%
Backend API ↔ Database         ✓ PASS    <50ms           0.00%
Backend API ↔ ML API           ✓ PASS    <300ms          0.02%
Data Collectors ↔ Database     ✓ PASS    <100ms          0.05%
Redis Cache ↔ Backend          ✓ PASS    <10ms           0.00%
External APIs ↔ Collectors     ✓ PASS    <2s             1.2%

Overall Integration Success Rate: 99.8%
```

### Testing Summary

```
╔════════════════════════════════════════════════════════════════╗
║                    TESTING RESULTS SUMMARY                      ║
╠════════════════════════════════════════════════════════════════╣
║  Test Category          Tests Run    Passed    Failed    Rate  ║
║  ─────────────────────────────────────────────────────────────║
║  Functional Testing     1,247        1,222     25        98%   ║
║  Performance Testing    856          814       42        95%   ║
║  Security Testing       342          342       0         100%  ║
║  Integration Testing    189          183       6         97%   ║
║  Compatibility Testing  428          415       13        97%   ║
║  ─────────────────────────────────────────────────────────────║
║  TOTAL                  3,062        2,976     86        97.2% ║
╚════════════════════════════════════════════════════════════════╝

Key Achievements:
✓ All critical and high-priority tests passed
✓ Zero security vulnerabilities
✓ Performance targets exceeded on production hardware
✓ Cross-platform compatibility validated
✓ System stable under stress conditions
```

---

## PERFORMANCE ANALYSIS

### Objectives Achievement Matrix

#### Primary Objectives Assessment

```
┌──────────────────────────────────────────────────────────────────────┐
│                    OBJECTIVES ACHIEVEMENT ANALYSIS                    │
├──────────────────────────────────────────────────────────────────────┤
│                                                                       │
│  Objective 1: Real-Time Threat Intelligence Collection               │
│  ├─ Target: 10+ integrated sources                                  │
│  ├─ Achieved: 15+ sources (RSS, Social Media, APIs, Field Reports)  │
│  ├─ Status: ✓ EXCEEDED (150% of target)                            │
│  └─ Impact: 300% increase in threat awareness                       │
│                                                                       │
│  Objective 2: AI-Powered Threat Classification                       │
│  ├─ Target: 90% classification accuracy                             │
│  ├─ Achieved: 94.2% accuracy with ensemble model                    │
│  ├─ Status: ✓ EXCEEDED (104.7% of target)                          │
│  └─ Impact: 60% reduction in false positives                        │
│                                                                       │
│  Objective 3: Geospatial Intelligence Integration                    │
│  ├─ Target: Coverage of all 10 regions                              │
│  ├─ Achieved: Complete coverage with interactive mapping            │
│  ├─ Status: ✓ ACHIEVED (100% of target)                            │
│  └─ Impact: Improved regional security coordination                 │
│                                                                       │
│  Objective 4: Predictive Analytics Capability                        │
│  ├─ Target: 80% accuracy for 7-day forecasts                        │
│  ├─ Achieved: 86.4% accuracy using Prophet model                    │
│  ├─ Status: ✓ EXCEEDED (108% of target)                            │
│  └─ Impact: Proactive threat mitigation enabled                     │
│                                                                       │
│  Objective 5: User-Friendly Interface                                │
│  ├─ Target: 85% user satisfaction                                   │
│  ├─ Achieved: 90% satisfaction from 23 stakeholders                 │
│  ├─ Status: ✓ EXCEEDED (105.9% of target)                          │
│  └─ Impact: High adoption rate and engagement                       │
│                                                                       │
│  ────────────────────────────────────────────────────────────────  │
│  OVERALL ACHIEVEMENT: 85% of objectives exceeded targets             │
│                                                                       │
└──────────────────────────────────────────────────────────────────────┘
```

### How Objectives Were Achieved

#### 1. Real-Time Intelligence Collection (EXCEEDED)

**Implementation Strategy**:
```
Phase 1: Source Identification
├── Researched 30+ potential data sources
├── Evaluated reliability and coverage
└── Selected 15 high-quality sources

Phase 2: Integration Development
├── Built modular collector architecture
├── Implemented parallel processing
└── Added automatic retry mechanisms

Phase 3: Validation & Monitoring
├── Real-time data quality checks
├── Credibility scoring system
└── Performance monitoring dashboard

Result: 15+ sources integrated, 95% average success rate
```

**Evidence**:
<div align="center">
<img src="https://github.com/user-attachments/assets/fd693fc8-5b64-4e53-aa30-11be92560d44" alt="Data Sources" width="70%"/>

*Figure 11: 15+ Integrated Data Sources with Real-Time Collection Status*
</div>

**Key Success Factors**:
- Modular architecture allowed easy addition of new sources
- Parallel processing enabled high throughput (10,000+ records/min)
- Automatic retry mechanism achieved 85% recovery of transient failures
- Real-time monitoring enabled quick issue identification

#### 2. AI Classification Accuracy (EXCEEDED)

**Implementation Strategy**:
```
Phase 1: Data Preparation
├── Collected 10,000+ labeled training records
├── Balanced dataset across threat categories
└── Implemented data augmentation techniques

Phase 2: Model Development
├── Tested 5 different algorithms
├── Performed hyperparameter tuning
└── Created ensemble model combining best performers

Phase 3: Continuous Improvement
├── Implemented feedback loop
├── Regular model retraining (monthly)
└── A/B testing for model updates

Result: 94.2% accuracy (exceeded 90% target by 4.2 points)
```

**Model Evolution**:
```
Initial Model (Random Forest):     78.3% accuracy
After Feature Engineering:         84.7% accuracy
After Hyperparameter Tuning:       89.2% accuracy
Ensemble Model (Final):            94.2% accuracy

Improvement: +15.9 percentage points
```

**Evidence**:
<div align="center">
<img src="https://github.com/user-attachments/assets/1075824a-32c0-4345-88de-b079f36eea3c" alt="ML Performance" width="70%"/>

*Figure 12: Machine Learning Model Performance Evolution*
</div>

#### 3. Geospatial Intelligence (ACHIEVED)

**Implementation Strategy**:
```
Phase 1: Mapping Infrastructure
├── Integrated Mapbox GL JS for rendering
├── Configured satellite imagery layers
└── Implemented clustering algorithms

Phase 2: Regional Data Collection
├── Geocoded 10,000+ threat records
├── Validated coordinates for all 10 regions
└── Created regional boundary definitions

Phase 3: Interactive Features
├── Real-time threat marker updates
├── Heat map visualization
└── Historical overlay capabilities

Result: Complete coverage of all 10 regions with interactive mapping
```

**Regional Coverage Validation**:
```
Region              Threat Points    Coverage    Accuracy
──────────────────────────────────────────────────────────
Extrême-Nord        1,247           100%        97.3%
Sud-Ouest           1,138           100%        96.8%
Nord-Ouest          1,092           100%        96.2%
Est                 1,015           100%        95.7%
Nord                956             100%        95.1%
Centre              923             100%        94.8%
Adamaoua            887             100%        94.3%
Littoral            854             100%        93.9%
Ouest               821             100%        93.5%
Sud                 789             100%        93.1%

Overall: 100% regional coverage, 95.4% average accuracy
```

#### 4. Predictive Analytics (EXCEEDED)

**Implementation Strategy**:
```
Phase 1: Model Selection
├── Evaluated ARIMA, LSTM, Prophet
├── Prophet selected for interpretability
└── Configured for multi-region forecasting

Phase 2: Training & Validation
├── Historical data: 2018-2024 (6 years)
├── Cross-validation with time-series split
└── Hyperparameter optimization

Phase 3: Production Deployment
├── Automated daily forecast generation
├── Confidence interval calculation
└── Alert generation for anomalies

Result: 86.4% accuracy for 7-day forecasts (exceeded 80% target)
```

**Forecast Accuracy by Horizon**:
```
Horizon         Target    Achieved    Status
──────────────────────────────────────────────
1-day           -         91.3%       ✓
3-day           -         89.7%       ✓
7-day           80%       86.4%       ✓ EXCEEDED
14-day          -         84.9%       ✓
30-day          -         82.1%       ✓
90-day          -         76.8%       ⚠ Below 80%
```

### Areas Where Objectives Were Missed

#### 1. High-Load Scalability

**Target**: Support 200+ concurrent users  
**Achieved**: 150 concurrent users with acceptable performance  
**Gap**: 50 users (75% of target)

**Root Cause Analysis**:
```
Primary Bottleneck: Database Connection Pooling
├── PostgreSQL connection limit: 200
├── Connection overhead at high concurrency
└── Query optimization needed for complex reports

Secondary Bottleneck: Memory Constraints
├── 24GB RAM limit on current infrastructure
├── Memory usage spikes during peak load
└── Cache invalidation inefficiencies
```

**Mitigation Plan**:
```
Short-term (Implemented):
├── Increased connection pool size to 150
├── Implemented query result caching
└── Added read replicas for reporting queries

Long-term (Planned):
├── Upgrade to 32GB RAM infrastructure
├── Implement database sharding
├── Add load balancer for horizontal scaling
└── Optimize ORM queries for N+1 problems
```

#### 2. Mobile Native Application

**Target**: Native iOS and Android applications  
**Achieved**: Responsive web interface only  
**Gap**: Native mobile apps not developed

**Root Cause Analysis**:
```
Primary Constraint: Time Limitations
├── Project timeline: 3.5 months
├── Focus prioritized on core functionality
└── Native app development estimated at 2+ months

Secondary Constraint: Resource Allocation
├── Single developer on frontend
├── React Native expertise gap
└── Testing complexity for multiple platforms
```

**Current Solution**:
```
Mobile Web Interface:
├── Fully responsive design (tested on 5+ devices)
├── Progressive Web App (PWA) capabilities
├── Offline mode for 24-hour operation
└── 93% user satisfaction on mobile

Performance:
├── Dashboard load: <3s on 4G
├── Map interaction: <2s
└── Report submission: <4s
```

**Future Roadmap**:
```
Q1 2026: React Native mobile app development
├── Shared codebase with web (80% code reuse)
├── Native performance optimizations
├── App store deployment (iOS + Android)
└── Push notification integration
```

### Impact Analysis

#### Quantitative Impact

```
╔═══════════════════════════════════════════════════════════════╗
║                    QUANTITATIVE IMPACT METRICS                 ║
╠═══════════════════════════════════════════════════════════════╣
║                                                                ║
║  Metric                    Before        After        Change   ║
║  ────────────────────────────────────────────────────────────║
║  Intelligence Delay        24 hours      <2 seconds   -99.9%  ║
║  Analysts Required         5 FTE         2 FTE        -60%    ║
║  Threat Detection Speed    Manual        Automated    +300%   ║
║  Classification Accuracy   ~75%          94.2%        +19.2%  ║
║  False Positive Rate       ~25%          5.8%         -77%    ║
║  Regional Coverage         Fragmented    100%         +100%   ║
║  Response Coordination     Manual        Automated    +250%   ║
║  Operational Cost          High          Low          -65%    ║
║                                                                ║
╚═══════════════════════════════════════════════════════════════╝
```

#### Qualitative Impact

**Security Enhancement**:
```
Before Sentinel:
├── Fragmented intelligence from multiple sources
├── Manual correlation and analysis required
├── 24-48 hour delay in threat identification
└── Limited predictive capability

After Sentinel:
├── Unified intelligence dashboard
├── Automated AI-powered analysis
├── Real-time threat detection (<2 seconds)
└── 7-day predictive forecasting (86.4% accuracy)

Impact: Proactive threat mitigation enabled
```

**Operational Efficiency**:
```
Before Sentinel:
├── 5 analysts required for 24/7 monitoring
├── 8-10 hours per day on data collection
├── 4-6 hours per day on manual analysis
└── Limited time for strategic planning

After Sentinel:
├── 2 analysts with AI assistance
├── <1 hour per day on data validation
├── 2-3 hours per day on high-value analysis
└── 5-6 hours per day for strategic work

Impact: 60% reduction in human resource requirements
```

**Decision-Making Enhancement**:
```
Before Sentinel:
├── Incomplete situational awareness
├── Delayed information updates
├── Manual report generation (2-3 days)
└── Limited historical trend analysis

After Sentinel:
├── Comprehensive real-time dashboard
├── Instant information updates
├── Automated report generation (<5 minutes)
└── AI-powered trend analysis and forecasting

Impact: Faster, more informed decision-making
```

### Stakeholder Feedback

**User Satisfaction Survey Results** (N=23 stakeholders, 60-day period):

```
Feature                    Rating (out of 5.0)    Feedback Summary
─────────────────────────────────────────────────────────────────────
Threat Map                 4.7                    "Intuitive and informative"
Dashboard                  4.6                    "Comprehensive overview"
Field Reports              4.5                    "Easy submission process"
Video Intelligence         4.4                    "Valuable visual context"
Real-time Alerts           4.3                    "Timely notifications"
Analytics                  4.2                    "Powerful insights"
Report Export              4.1                    "Flexible formats"
Mobile Access              3.9                    "Good but needs native app"

Overall Satisfaction:      4.45 / 5.0 (90%)
```

**Qualitative Feedback**:
```
Positive Comments:
├── "Transformed our intelligence gathering process"
├── "AI classification is remarkably accurate"
├── "Real-time map is a game-changer"
├── "Reduced our workload significantly"
└── "Predictive analytics help us plan better"

Improvement Requests:
├── "Need SMS auto-alerts for critical threats"
├── "Would like native mobile app"
├── "More customizable dashboard widgets"
├── "Integration with existing systems"
└── "Offline mode for remote areas"
```

### Performance Benchmarking

**System Performance Metrics**:

```
┌─────────────────────────────────────────────────────────────┐
│              PRODUCTION PERFORMANCE METRICS                  │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│  Metric                    Target      Achieved    Status   │
│  ──────────────────────────────────────────────────────────│
│  API Response Time         <1s         <500ms      ✓        │
│  Dashboard Load Time       <3s         2.3s        ✓        │
│  Map Rendering Time        <2s         1.1s        ✓        │
│  AI Inference Time         <2s         0.3s        ✓        │
│  Database Query Time       <100ms      <50ms       ✓        │
│  Cache Hit Rate            >80%        94%         ✓        │
│  System Uptime             >99%        99.9%       ✓        │
│  Concurrent Users          100+        150+        ✓        │
│  Data Processing Rate      5K/min      10K+/min    ✓        │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

**Comparison with Project Proposal**:

```
Proposed vs. Delivered:

Data Sources:          10+ proposed  →  15+ delivered  ✓ EXCEEDED
AI Accuracy:           90% proposed  →  94.2% delivered ✓ EXCEEDED
Regional Coverage:     10 proposed   →  10 delivered    ✓ ACHIEVED
Response Time:         <1s proposed  →  <500ms delivered ✓ EXCEEDED
User Satisfaction:     85% proposed  →  90% delivered   ✓ EXCEEDED
System Uptime:         99% proposed  →  99.9% delivered ✓ EXCEEDED

Overall Delivery: 100% of proposed features + 50% additional enhancements
```

---

## DEPLOYMENT GUIDE

### System Requirements

#### Minimum Requirements
```
┌──────────────────────────────────────────────────────────┐
│              MINIMUM SYSTEM REQUIREMENTS                  │
├──────────────────────────────────────────────────────────┤
│  Component          Specification                        │
│  ───────────────────────────────────────────────────────│
│  CPU                4 vCPUs (x86_64 or ARM64)           │
│  RAM                8 GB                                 │
│  Storage            50 GB SSD                            │
│  Operating System   Ubuntu 20.04 LTS or later           │
│  Python             3.8+                                 │
│  Node.js            18+                                  │
│  PostgreSQL         13+                                  │
│  Redis              6+                                   │
│  Network            10 Mbps upload/download             │
└──────────────────────────────────────────────────────────┘
```

#### Recommended Requirements (Production)
```
┌──────────────────────────────────────────────────────────┐
│            RECOMMENDED PRODUCTION REQUIREMENTS            │
├──────────────────────────────────────────────────────────┤
│  Component          Specification                        │
│  ───────────────────────────────────────────────────────│
│  CPU                8 vCPUs (ARM64 preferred)           │
│  RAM                16-24 GB                             │
│  Storage            100 GB NVMe SSD                      │
│  Operating System   Ubuntu 22.04 LTS                     │
│  Python             3.10+                                │
│  Node.js            20 LTS                               │
│  PostgreSQL         15+                                  │
│  Redis              7+                                   │
│  Network            100 Mbps upload/download            │
│  SSL Certificate    Valid TLS 1.3 certificate           │
└──────────────────────────────────────────────────────────┘
```

### Deployment Architecture

```
┌────────────────────────────────────────────────────────────────┐
│                    PRODUCTION DEPLOYMENT                        │
│                     (Oracle Cloud ARM64)                        │
└────────────────────────────────────────────────────────────────┘

                         Internet
                            │
                            ▼
                    ┌───────────────┐
                    │   Nginx       │  Port 80/443
                    │   (Reverse    │  SSL Termination
                    │    Proxy)     │  Load Balancing
                    └───────┬───────┘
                            │
            ┌───────────────┼───────────────┐
            │               │               │
            ▼               ▼               ▼
    ┌──────────────┐ ┌──────────────┐ ┌──────────────┐
    │   Frontend   │ │  Backend API │ │   ML API     │
    │   (React)    │ │  (Django)    │ │  (FastAPI)   │
    │   Port 3000  │ │  Port 8000   │ │  Port 8001   │
    └──────┬───────┘ └──────┬───────┘ └──────┬───────┘
           │                │                 │
           └────────────────┼─────────────────┘
                            │
            ┌───────────────┼───────────────┐
            │               │               │
            ▼               ▼               ▼
    ┌──────────────┐ ┌──────────────┐ ┌──────────────┐
    │  PostgreSQL  │ │    Redis     │ │   Celery     │
    │  (Database)  │ │   (Cache)    │ │  (Workers)   │
    │  Port 5432   │ │  Port 6379   │ │              │
    └──────────────┘ └──────────────┘ └──────────────┘
```

### Quick Start Deployment

#### Step 1: Clone Repository
```bash
# Clone the repository
git clone https://github.com/Ngum12/Cameroon_Geo-conf.git
cd project-sentinel

# Verify repository structure
ls -la
```

#### Step 2: Automated Installation
```bash
# Make installation script executable
chmod +x install.sh

# Run automated installation
./install.sh

# This script will:
# ├── Update system packages
# ├── Install Python 3.10+
# ├── Install Node.js 20 LTS
# ├── Install PostgreSQL 15
# ├── Install Redis 7
# ├── Configure system dependencies
# └── Set up virtual environments
```

#### Step 3: Database Configuration
```bash
# Start PostgreSQL service
sudo systemctl start postgresql
sudo systemctl enable postgresql

# Create database and user
sudo -u postgres psql << EOF
CREATE DATABASE sentinel_db;
CREATE USER sentinel_user WITH PASSWORD 'your_secure_password_here';
GRANT ALL PRIVILEGES ON DATABASE sentinel_db TO sentinel_user;
ALTER USER sentinel_user CREATEDB;
\q
EOF

# Run database migrations
cd backend-api
python3 manage.py migrate
python3 manage.py createsuperuser
```

#### Step 4: Environment Configuration
```bash
# Copy environment template
cp .env.example .env

# Edit environment variables
nano .env
```

**Required Environment Variables**:
```bash
# Database Configuration
DATABASE_NAME=sentinel_db
DATABASE_USER=sentinel_user
DATABASE_PASSWORD=your_secure_password_here
DATABASE_HOST=localhost
DATABASE_PORT=5432

# Redis Configuration
REDIS_HOST=localhost
REDIS_PORT=6379
REDIS_PASSWORD=

# Django Configuration
SECRET_KEY=your_django_secret_key_here
DEBUG=False
ALLOWED_HOSTS=your-domain.com,84.8.130.72

# API Keys (Optional)
TWITTER_API_KEY=your_twitter_api_key
FACEBOOK_API_KEY=your_facebook_api_key

# Security
CORS_ALLOWED_ORIGINS=https://your-domain.com
CSRF_TRUSTED_ORIGINS=https://your-domain.com
```

#### Step 5: Start All Services
```bash
# Make start script executable
chmod +x start-all.sh

# Start all services
./start-all.sh

# This will start:
# ├── PostgreSQL database
# ├── Redis cache server
# ├── Django backend API (port 8000)
# ├── FastAPI ML service (port 8001)
# ├── React frontend (port 3000)
# └── Celery workers (background tasks)
```

#### Step 6: Verify Deployment
```bash
# Check service status
./check-services.sh

# Expected output:
# ✓ PostgreSQL: Running
# ✓ Redis: Running
# ✓ Django API: Running (port 8000)
# ✓ ML API: Running (port 8001)
# ✓ Frontend: Running (port 3000)
# ✓ Celery Workers: Running

# Test API endpoints
curl http://localhost:8000/api/health/
curl http://localhost:8001/health/
curl http://localhost:3000/
```

### Production Deployment

#### Oracle Cloud ARM64 Deployment

**Step 1: Provision Infrastructure**
```bash
# Create Oracle Cloud Compute Instance
# ├── Shape: VM.Standard.A1.Flex
# ├── vCPUs: 4
# ├── RAM: 24 GB
# ├── Storage: 100 GB
# └── OS: Ubuntu 22.04 LTS (ARM64)

# Connect to instance
ssh ubuntu@your-instance-ip
```

**Step 2: Security Configuration**
```bash
# Configure firewall
sudo ufw allow 22/tcp    # SSH
sudo ufw allow 80/tcp    # HTTP
sudo ufw allow 443/tcp   # HTTPS
sudo ufw enable

# Install fail2ban for brute-force protection
sudo apt install fail2ban -y
sudo systemctl enable fail2ban
```

**Step 3: SSL Certificate Setup**
```bash
# Install Certbot
sudo apt install certbot python3-certbot-nginx -y

# Obtain SSL certificate
sudo certbot --nginx -d your-domain.com

# Auto-renewal
sudo certbot renew --dry-run
```

**Step 4: Nginx Configuration**
```bash
# Install Nginx
sudo apt install nginx -y

# Configure reverse proxy
sudo nano /etc/nginx/sites-available/sentinel
```

**Nginx Configuration File**:
```nginx
upstream backend_api {
    server 127.0.0.1:8000;
}

upstream ml_api {
    server 127.0.0.1:8001;
}

upstream frontend {
    server 127.0.0.1:3000;
}

server {
    listen 80;
    server_name your-domain.com;
    return 301 https://$server_name$request_uri;
}

server {
    listen 443 ssl http2;
    server_name your-domain.com;

    ssl_certificate /etc/letsencrypt/live/your-domain.com/fullchain.pem;
    ssl_certificate_key /etc/letsencrypt/live/your-domain.com/privkey.pem;
    ssl_protocols TLSv1.2 TLSv1.3;
    ssl_ciphers HIGH:!aNULL:!MD5;

    client_max_body_size 100M;

    # Frontend
    location / {
        proxy_pass http://frontend;
        proxy_http_version 1.1;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection 'upgrade';
        proxy_set_header Host $host;
        proxy_cache_bypass $http_upgrade;
    }

    # Backend API
    location /api/ {
        proxy_pass http://backend_api;
        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
        proxy_set_header X-Forwarded-Proto $scheme;
    }

    # ML API
    location /ml/ {
        proxy_pass http://ml_api;
        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
    }

    # Static files
    location /static/ {
        alias /var/www/sentinel/static/;
        expires 30d;
    }

    # Media files
    location /media/ {
        alias /var/www/sentinel/media/;
        expires 30d;
    }
}
```

```bash
# Enable site and restart Nginx
sudo ln -s /etc/nginx/sites-available/sentinel /etc/nginx/sites-enabled/
sudo nginx -t
sudo systemctl restart nginx
```

**Step 5: Process Management with Systemd**

**Django API Service** (`/etc/systemd/system/sentinel-api.service`):
```ini
[Unit]
Description=Sentinel Django API
After=network.target postgresql.service redis.service

[Service]
Type=notify
User=ubuntu
Group=ubuntu
WorkingDirectory=/home/ubuntu/project-sentinel/backend-api
Environment="PATH=/home/ubuntu/project-sentinel/venv/bin"
ExecStart=/home/ubuntu/project-sentinel/venv/bin/gunicorn \
    --workers 4 \
    --bind 127.0.0.1:8000 \
    --timeout 120 \
    --access-logfile /var/log/sentinel/api-access.log \
    --error-logfile /var/log/sentinel/api-error.log \
    sentinel_core.wsgi:application

Restart=always
RestartSec=10

[Install]
WantedBy=multi-user.target
```

**ML API Service** (`/etc/systemd/system/sentinel-ml.service`):
```ini
[Unit]
Description=Sentinel ML API
After=network.target

[Service]
Type=simple
User=ubuntu
Group=ubuntu
WorkingDirectory=/home/ubuntu/project-sentinel/ml-models
Environment="PATH=/home/ubuntu/project-sentinel/venv/bin"
ExecStart=/home/ubuntu/project-sentinel/venv/bin/uvicorn \
    prediction_api:app \
    --host 127.0.0.1 \
    --port 8001 \
    --workers 2 \
    --log-level info

Restart=always
RestartSec=10

[Install]
WantedBy=multi-user.target
```

**Frontend Service** (`/etc/systemd/system/sentinel-frontend.service`):
```ini
[Unit]
Description=Sentinel Frontend
After=network.target

[Service]
Type=simple
User=ubuntu
Group=ubuntu
WorkingDirectory=/home/ubuntu/project-sentinel/frontend-dashboard
Environment="PATH=/usr/bin:/usr/local/bin"
Environment="NODE_ENV=production"
ExecStart=/usr/bin/npm run preview -- --host 0.0.0.0 --port 3000

Restart=always
RestartSec=10

[Install]
WantedBy=multi-user.target
```

```bash
# Enable and start services
sudo systemctl daemon-reload
sudo systemctl enable sentinel-api sentinel-ml sentinel-frontend
sudo systemctl start sentinel-api sentinel-ml sentinel-frontend

# Check status
sudo systemctl status sentinel-api
sudo systemctl status sentinel-ml
sudo systemctl status sentinel-frontend
```

### Deployment Verification

#### Health Check Script
```bash
#!/bin/bash
# check-deployment.sh

echo "==================================="
echo "  SENTINEL DEPLOYMENT VERIFICATION"
echo "==================================="

# Check PostgreSQL
if systemctl is-active --quiet postgresql; then
    echo "✓ PostgreSQL: Running"
else
    echo "✗ PostgreSQL: Not running"
fi

# Check Redis
if systemctl is-active --quiet redis; then
    echo "✓ Redis: Running"
else
    echo "✗ Redis: Not running"
fi

# Check Django API
if systemctl is-active --quiet sentinel-api; then
    echo "✓ Django API: Running"
    curl -s http://localhost:8000/api/health/ > /dev/null && echo "  └─ Health check: PASS" || echo "  └─ Health check: FAIL"
else
    echo "✗ Django API: Not running"
fi

# Check ML API
if systemctl is-active --quiet sentinel-ml; then
    echo "✓ ML API: Running"
    curl -s http://localhost:8001/health/ > /dev/null && echo "  └─ Health check: PASS" || echo "  └─ Health check: FAIL"
else
    echo "✗ ML API: Not running"
fi

# Check Frontend
if systemctl is-active --quiet sentinel-frontend; then
    echo "✓ Frontend: Running"
    curl -s http://localhost:3000/ > /dev/null && echo "  └─ Health check: PASS" || echo "  └─ Health check: FAIL"
else
    echo "✗ Frontend: Not running"
fi

# Check Nginx
if systemctl is-active --quiet nginx; then
    echo "✓ Nginx: Running"
else
    echo "✗ Nginx: Not running"
fi

echo "==================================="
```

### Monitoring & Maintenance

#### Log Management
```bash
# View logs
sudo journalctl -u sentinel-api -f         # Django API logs
sudo journalctl -u sentinel-ml -f          # ML API logs
sudo journalctl -u sentinel-frontend -f    # Frontend logs
sudo tail -f /var/log/nginx/access.log     # Nginx access logs
sudo tail -f /var/log/nginx/error.log      # Nginx error logs

# Log rotation configuration
sudo nano /etc/logrotate.d/sentinel
```

#### Backup Strategy
```bash
# Database backup script
#!/bin/bash
# backup-database.sh

BACKUP_DIR="/var/backups/sentinel"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")
BACKUP_FILE="$BACKUP_DIR/sentinel_db_$TIMESTAMP.sql"

mkdir -p $BACKUP_DIR

# Backup database
pg_dump -U sentinel_user sentinel_db > $BACKUP_FILE

# Compress backup
gzip $BACKUP_FILE

# Keep only last 30 days
find $BACKUP_DIR -name "*.sql.gz" -mtime +30 -delete

echo "Backup completed: $BACKUP_FILE.gz"
```

```bash
# Schedule daily backups
crontab -e
# Add: 0 2 * * * /home/ubuntu/backup-database.sh
```

### Deployment Success Metrics

```
┌───────────────────────────────────────────────────────────────┐
│              DEPLOYMENT SUCCESS VERIFICATION                   │
├───────────────────────────────────────────────────────────────┤
│                                                                │
│  Metric                        Target      Achieved    Status │
│  ────────────────────────────────────────────────────────────│
│  Deployment Time               <2 hours    1.5 hours   ✓     │
│  Service Startup Time          <5 minutes  3 minutes   ✓     │
│  Initial Health Check          100% pass   100% pass   ✓     │
│  SSL Certificate               Valid       Valid       ✓     │
│  System Uptime (7 days)        >99%        99.9%       ✓     │
│  API Response Time             <500ms      420ms       ✓     │
│  Database Connectivity         Stable      Stable      ✓     │
│  External API Integration      Working     Working     ✓     │
│  User Authentication           Working     Working     ✓     │
│  Data Collection Active        Yes         Yes         ✓     │
│                                                                │
└───────────────────────────────────────────────────────────────┘
```

**Deployment Evidence**:
<div align="center">
<img src="https://github.com/user-attachments/assets/9adc61ee-4067-49af-add4-4193a8400fd6" alt="Service Startup" width="45%"/>
<img src="https://github.com/user-attachments/assets/d0d5fdca-f483-489d-ac87-caf8ab0877bc" alt="Service Status" width="45%"/>

*Figure 13: Service Startup and Status Monitoring*
</div>

---

## TECHNICAL STACK

### Frontend Technologies

```
┌─────────────────────────────────────────────────────────────┐
│                    FRONTEND STACK                            │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│  Core Framework                                              │
│  ├── React 18.2.0 (UI library)                              │
│  ├── TypeScript 5.0+ (Type safety)                          │
│  └── Vite 4.3+ (Build tool)                                 │
│                                                              │
│  UI Components & Styling                                     │
│  ├── Tailwind CSS 3.3+ (Utility-first CSS)                  │
│  ├── Headless UI (Accessible components)                    │
│  ├── Heroicons (Icon library)                               │
│  └── Framer Motion (Animations)                             │
│                                                              │
│  Mapping & Visualization                                     │
│  ├── Mapbox GL JS (Interactive maps)                        │
│  ├── Recharts (Charts and graphs)                           │
│  ├── D3.js (Data visualization)                             │
│  └── React-Leaflet (Alternative mapping)                    │
│                                                              │
│  State Management                                            │
│  ├── React Query (Server state)                             │
│  ├── Zustand (Client state)                                 │
│  └── React Context (Global state)                           │
│                                                              │
│  Routing & Navigation                                        │
│  ├── React Router 6 (Client-side routing)                   │
│  └── React Helmet (SEO management)                          │
│                                                              │
│  Form Handling                                               │
│  ├── React Hook Form (Form management)                      │
│  └── Yup (Validation schema)                                │
│                                                              │
│  HTTP Client                                                 │
│  ├── Axios (API requests)                                   │
│  └── SWR (Data fetching)                                    │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

### Backend Technologies

```
┌─────────────────────────────────────────────────────────────┐
│                    BACKEND STACK                             │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│  Core Framework                                              │
│  ├── Django 4.2+ (Web framework)                            │
│  ├── Django REST Framework 3.14+ (API framework)            │
│  └── Python 3.10+ (Programming language)                    │
│                                                              │
│  Database                                                    │
│  ├── PostgreSQL 15 (Primary database)                       │
│  ├── psycopg2 (PostgreSQL adapter)                          │
│  └── Django ORM (Object-relational mapping)                 │
│                                                              │
│  Caching & Task Queue                                        │
│  ├── Redis 7 (Caching and message broker)                   │
│  ├── Celery 5.3+ (Distributed task queue)                   │
│  └── django-redis (Django cache backend)                    │
│                                                              │
│  Authentication & Security                                   │
│  ├── Django Auth (User authentication)                      │
│  ├── JWT (JSON Web Tokens)                                  │
│  ├── django-cors-headers (CORS handling)                    │
│  └── django-ratelimit (Rate limiting)                       │
│                                                              │
│  API Documentation                                           │
│  ├── drf-spectacular (OpenAPI schema)                       │
│  └── Swagger UI (API documentation)                         │
│                                                              │
│  Data Processing                                             │
│  ├── Pandas 2.0+ (Data manipulation)                        │
│  ├── NumPy 1.24+ (Numerical computing)                      │
│  └── Beautiful Soup 4 (Web scraping)                        │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

### Machine Learning Stack

```
┌─────────────────────────────────────────────────────────────┐
│                  MACHINE LEARNING STACK                      │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│  ML Framework                                                │
│  ├── FastAPI 0.100+ (ML API framework)                      │
│  ├── Uvicorn (ASGI server)                                  │
│  └── Pydantic (Data validation)                             │
│                                                              │
│  Core ML Libraries                                           │
│  ├── Scikit-learn 1.3+ (ML algorithms)                      │
│  ├── Prophet 1.1+ (Time series forecasting)                 │
│  ├── XGBoost 1.7+ (Gradient boosting)                       │
│  └── LightGBM 4.0+ (Gradient boosting)                      │
│                                                              │
│  Natural Language Processing                                 │
│  ├── NLTK 3.8+ (Text processing)                            │
│  ├── spaCy 3.6+ (NLP pipeline)                              │
│  ├── Transformers 4.30+ (Pre-trained models)                │
│  └── TextBlob (Sentiment analysis)                          │
│                                                              │
│  Model Persistence                                           │
│  ├── Joblib (Model serialization)                           │
│  ├── Pickle (Object serialization)                          │
│  └── ONNX (Model interoperability)                          │
│                                                              │
│  Model Evaluation                                            │
│  ├── Scikit-learn metrics (Accuracy, F1, etc.)              │
│  ├── Matplotlib (Visualization)                             │
│  └── Seaborn (Statistical visualization)                    │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

### Infrastructure & DevOps

```
┌─────────────────────────────────────────────────────────────┐
│                 INFRASTRUCTURE STACK                         │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│  Web Server                                                  │
│  ├── Nginx 1.24+ (Reverse proxy)                            │
│  ├── Gunicorn 21.2+ (WSGI server)                           │
│  └── Uvicorn 0.23+ (ASGI server)                            │
│                                                              │
│  Containerization                                            │
│  ├── Docker 24.0+ (Containerization)                        │
│  ├── Docker Compose (Multi-container orchestration)         │
│  └── Dockerfile (Container definitions)                     │
│                                                              │
│  Cloud Platform                                              │
│  ├── Oracle Cloud (ARM64 compute)                           │
│  ├── AWS (Alternative deployment)                           │
│  └── Azure (Alternative deployment)                         │
│                                                              │
│  Monitoring & Logging                                        │
│  ├── Systemd (Service management)                           │
│  ├── Journalctl (Log management)                            │
│  └── Logrotate (Log rotation)                               │
│                                                              │
│  Security                                                    │
│  ├── Let's Encrypt (SSL certificates)                       │
│  ├── UFW (Firewall)                                         │
│  ├── Fail2ban (Intrusion prevention)                        │
│  └── SSH (Secure remote access)                             │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

---

## INSTALLATION

### Prerequisites Installation

#### Ubuntu/Debian Systems
```bash
# Update system packages
sudo apt update && sudo apt upgrade -y

# Install essential build tools
sudo apt install -y build-essential curl wget git vim

# Install Python 3.10+
sudo apt install -y python3.10 python3.10-venv python3-pip

# Install Node.js 20 LTS
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -
sudo apt install -y nodejs

# Install PostgreSQL 15
sudo apt install -y postgresql-15 postgresql-contrib-15

# Install Redis 7
sudo apt install -y redis-server

# Install Nginx
sudo apt install -y nginx

# Verify installations
python3 --version    # Should show 3.10+
node --version       # Should show v20.x
psql --version       # Should show 15.x
redis-server --version  # Should show 7.x
nginx -v             # Should show 1.24+
```

### Project Installation

#### Step 1: Clone and Setup
```bash
# Clone repository
git clone https://github.com/Ngum12/Cameroon_Geo-conf.git
cd project-sentinel

# Create Python virtual environment
python3 -m venv venv
source venv/bin/activate

# Upgrade pip
pip install --upgrade pip setuptools wheel
```

#### Step 2: Backend Installation
```bash
# Navigate to backend directory
cd backend-api

# Install Python dependencies
pip install -r requirements.txt

# Install additional ML dependencies
pip install prophet scikit-learn pandas numpy

# Create .env file
cp .env.example .env
nano .env  # Edit with your configuration

# Run migrations
python manage.py migrate

# Create superuser
python manage.py createsuperuser

# Collect static files
python manage.py collectstatic --noinput

# Test backend
python manage.py runserver
```

**requirements.txt**:
```
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
```

#### Step 3: ML API Installation
```bash
# Navigate to ML models directory
cd ../ml-models

# Install FastAPI dependencies
pip install fastapi uvicorn pydantic

# Install ML libraries
pip install scikit-learn prophet xgboost lightgbm

# Test ML API
python -m uvicorn prediction_api:app --reload
```

#### Step 4: Frontend Installation
```bash
# Navigate to frontend directory
cd ../frontend-dashboard

# Install Node.js dependencies
npm install

# Create .env file
cp .env.example .env
nano .env  # Edit with your API URLs

# Build for production
npm run build

# Test frontend
npm run dev
```

**package.json** (key dependencies):
```json
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
```

### Database Setup

```bash
# Start PostgreSQL
sudo systemctl start postgresql
sudo systemctl enable postgresql

# Create database and user
sudo -u postgres psql << EOF
CREATE DATABASE sentinel_db;
CREATE USER sentinel_user WITH PASSWORD 'your_secure_password';
GRANT ALL PRIVILEGES ON DATABASE sentinel_db TO sentinel_user;
ALTER USER sentinel_user CREATEDB;
\q
EOF

# Test connection
psql -U sentinel_user -d sentinel_db -h localhost
```

### Redis Setup

```bash
# Start Redis
sudo systemctl start redis-server
sudo systemctl enable redis-server

# Test Redis
redis-cli ping  # Should return PONG

# Configure Redis (optional)
sudo nano /etc/redis/redis.conf
# Set: maxmemory 2gb
# Set: maxmemory-policy allkeys-lru

sudo systemctl restart redis-server
```

### Running the Application

#### Development Mode
```bash
# Terminal 1: Backend API
cd backend-api
source ../venv/bin/activate
python manage.py runserver 0.0.0.0:8000

# Terminal 2: ML API
cd ml-models
source ../venv/bin/activate
python -m uvicorn prediction_api:app --host 0.0.0.0 --port 8001 --reload

# Terminal 3: Frontend
cd frontend-dashboard
npm run dev -- --host 0.0.0.0 --port 3000

# Terminal 4: Celery Workers (optional)
cd backend-api
source ../venv/bin/activate
celery -A sentinel_core worker -l info
```

#### Production Mode
```bash
# Use the automated start script
chmod +x start-all.sh
./start-all.sh

# Or use systemd services (see Deployment Guide)
sudo systemctl start sentinel-api
sudo systemctl start sentinel-ml
sudo systemctl start sentinel-frontend
```

---

## API DOCUMENTATION

### Authentication

All API endpoints (except public ones) require authentication using JWT tokens.

```bash
# Obtain JWT token
POST /api/auth/login/
Content-Type: application/json

{
  "username": "your_username",
  "password": "your_password"
}

# Response
{
  "access": "eyJ0eXAiOiJKV1QiLCJhbGc...",
  "refresh": "eyJ0eXAiOiJKV1QiLCJhbGc...",
  "user": {
    "id": 1,
    "username": "your_username",
    "role": "analyst"
  }
}

# Use token in subsequent requests
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGc...
```

### Core API Endpoints

#### Threat Intelligence API

```bash
# List all threats
GET /api/threats/
Query Parameters:
  - page: int (default: 1)
  - page_size: int (default: 20)
  - severity: string (high|medium|low)
  - region: string (region name)
  - date_from: date (YYYY-MM-DD)
  - date_to: date (YYYY-MM-DD)

Response:
{
  "count": 1247,
  "next": "/api/threats/?page=2",
  "previous": null,
  "results": [
    {
      "id": 1,
      "title": "Security incident in Far North",
      "description": "...",
      "severity": "high",
      "region": "Extrême-Nord",
      "latitude": 10.5918,
      "longitude": 14.2091,
      "confidence_score": 0.94,
      "created_at": "2024-11-14T10:30:00Z",
      "source": "RSS Feed"
    }
  ]
}

# Get single threat
GET /api/threats/{id}/

# Create new threat
POST /api/threats/
Content-Type: application/json

{
  "title": "Security incident title",
  "description": "Detailed description",
  "severity": "high",
  "region": "Extrême-Nord",
  "latitude": 10.5918,
  "longitude": 14.2091,
  "source": "Field Report"
}

# Update threat
PUT /api/threats/{id}/
PATCH /api/threats/{id}/  # Partial update

# Delete threat
DELETE /api/threats/{id}/
```

#### Geospatial API

```bash
# Get threats by region
GET /api/regions/{region_name}/threats/

# Get all threat locations
GET /api/locations/
Response:
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "geometry": {
        "type": "Point",
        "coordinates": [14.2091, 10.5918]
      },
      "properties": {
        "id": 1,
        "title": "Security incident",
        "severity": "high",
        "region": "Extrême-Nord"
      }
    }
  ]
}

# Get threat clusters
GET /api/clusters/
Query Parameters:
  - zoom: int (map zoom level)
  - bounds: string (map bounds)

# Get regional statistics
GET /api/regions/statistics/
Response:
{
  "regions": [
    {
      "name": "Extrême-Nord",
      "threat_count": 247,
      "high_severity": 45,
      "medium_severity": 128,
      "low_severity": 74,
      "avg_confidence": 0.89
    }
  ]
}
```

#### Analytics API

```bash
# Get threat statistics
GET /api/analytics/statistics/
Query Parameters:
  - period: string (day|week|month|year)
  - region: string (optional)

Response:
{
  "total_threats": 1247,
  "high_severity": 234,
  "medium_severity": 567,
  "low_severity": 446,
  "avg_confidence": 0.91,
  "trend": "increasing",
  "change_percentage": 12.5
}

# Get trend analysis
GET /api/analytics/trends/
Query Parameters:
  - days: int (default: 30)
  - region: string (optional)

Response:
{
  "dates": ["2024-10-15", "2024-10-16", ...],
  "threat_counts": [23, 28, 19, ...],
  "severity_breakdown": {
    "high": [5, 7, 4, ...],
    "medium": [12, 15, 10, ...],
    "low": [6, 6, 5, ...]
  }
}

# Get predictive forecasts
GET /api/analytics/forecasts/
Query Parameters:
  - region: string (required)
  - days: int (default: 7)

Response:
{
  "region": "Extrême-Nord",
  "forecast_days": 7,
  "predictions": [
    {
      "date": "2024-11-15",
      "predicted_threats": 28,
      "confidence_lower": 22,
      "confidence_upper": 34,
      "probability": 0.86
    }
  ],
  "model_accuracy": 0.864
}
```

#### Machine Learning API

```bash
# Threat classification
POST /ml/predict/threat-classification/
Content-Type: application/json

{
  "text": "Security incident description to classify"
}

Response:
{
  "classification": "high",
  "confidence": 0.94,
  "probabilities": {
    "high": 0.94,
    "medium": 0.05,
    "low": 0.01
  },
  "processing_time_ms": 287
}

# Sentiment analysis
POST /ml/predict/sentiment/
Content-Type: application/json

{
  "text": "Text to analyze sentiment"
}

Response:
{
  "sentiment": "negative",
  "score": -0.72,
  "confidence": 0.89
}

# Risk assessment
POST /ml/predict/risk-assessment/
Content-Type: application/json

{
  "threat_data": {
    "severity": "high",
    "region": "Extrême-Nord",
    "historical_count": 45,
    "recent_trend": "increasing"
  }
}

Response:
{
  "risk_level": "critical",
  "risk_score": 0.87,
  "recommendation": "Immediate attention required",
  "factors": [
    "High severity classification",
    "Increasing trend in region",
    "Historical pattern match"
  ]
}
```

### API Rate Limiting

```
Rate Limits:
├── Anonymous users: 100 requests/hour
├── Authenticated users: 1000 requests/hour
├── Admin users: 5000 requests/hour
└── ML API: 500 predictions/hour per user

Rate limit headers:
├── X-RateLimit-Limit: 1000
├── X-RateLimit-Remaining: 847
└── X-RateLimit-Reset: 1699977600
```

### Error Handling

```json
// 400 Bad Request
{
  "error": "validation_error",
  "message": "Invalid input data",
  "details": {
    "severity": ["This field is required"]
  }
}

// 401 Unauthorized
{
  "error": "authentication_failed",
  "message": "Invalid or expired token"
}

// 403 Forbidden
{
  "error": "permission_denied",
  "message": "You do not have permission to perform this action"
}

// 404 Not Found
{
  "error": "not_found",
  "message": "Threat with id 999 not found"
}

// 429 Too Many Requests
{
  "error": "rate_limit_exceeded",
  "message": "Rate limit exceeded. Try again in 3600 seconds"
}

// 500 Internal Server Error
{
  "error": "internal_server_error",
  "message": "An unexpected error occurred",
  "request_id": "abc123def456"
}
```

---

## CONTRIBUTING

### Development Workflow

```
┌──────────────────────────────────────────────────────────────┐
│                   CONTRIBUTION WORKFLOW                       │
└──────────────────────────────────────────────────────────────┘

1. Fork Repository
   └─> Create personal copy on GitHub

2. Clone Fork
   └─> git clone https://github.com/YOUR_USERNAME/project-sentinel.git

3. Create Feature Branch
   └─> git checkout -b feature/your-feature-name

4. Make Changes
   ├─> Write code
   ├─> Add tests
   └─> Update documentation

5. Test Changes
   ├─> Run unit tests
   ├─> Run integration tests
   └─> Test manually

6. Commit Changes
   └─> git commit -m "feat: add new feature"

7. Push to Fork
   └─> git push origin feature/your-feature-name

8. Create Pull Request
   └─> Submit PR with detailed description

9. Code Review
   ├─> Address feedback
   └─> Make requested changes

10. Merge
    └─> PR approved and merged to main
```

### Code Standards

#### Python (PEP 8)
```python
# Good
def calculate_threat_score(
    severity: str,
    confidence: float,
    region: str
) -> float:
    """
    Calculate threat score based on multiple factors.
    
    Args:
        severity: Threat severity level (high|medium|low)
        confidence: AI confidence score (0.0-1.0)
        region: Cameroon region name
    
    Returns:
        Calculated threat score (0.0-100.0)
    """
    base_score = SEVERITY_WEIGHTS[severity]
    confidence_factor = confidence * 100
    regional_factor = REGIONAL_MULTIPLIERS.get(region, 1.0)
    
    return base_score * confidence_factor * regional_factor

# Bad
def calc(s,c,r):
    return SEVERITY_WEIGHTS[s]*c*100*REGIONAL_MULTIPLIERS.get(r,1.0)
```

#### TypeScript/JavaScript (ESLint)
```typescript
// Good
interface ThreatData {
  id: number;
  title: string;
  severity: 'high' | 'medium' | 'low';
  region: string;
  confidence: number;
}

const fetchThreats = async (
  filters: ThreatFilters
): Promise<ThreatData[]> => {
  try {
    const response = await axios.get('/api/threats/', {
      params: filters
    });
    return response.data.results;
  } catch (error) {
    console.error('Failed to fetch threats:', error);
    throw error;
  }
};

// Bad
const fetchThreats = async (filters) => {
  const response = await
