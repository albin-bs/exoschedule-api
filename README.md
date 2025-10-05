# ExoSchedule API

Backend API for ExoSchedule – an intelligent, AI-powered exoplanet observation scheduler built for the NASA Space Apps Challenge.

## 🌌 Overview

ExoSchedule API serves as the backend system for scheduling and optimizing ground-based telescope follow-ups of exoplanet candidates discovered by missions like TESS. The API employs active learning, Gaussian Process regression, and information theory to recommend the most valuable next observations, maximizing discovery efficiency.

**Key Features:**
- RESTful FastAPI service
- Integrates with NASA Exoplanet Archive and TESS data
- Intelligent Bayesian scheduling and prioritization
- Real-time updating of TOI (TESS Objects of Interest) status and observation plans
- Designed for seamless connection to lightweight web frontends

---

## 🚀 Quick Start

### Prerequisites
- Python 3.11+
- pip

### Setup Instructions
API will be running at flowbound.me

---

## 🧑‍💻 API Endpoints

| Path                         | Description                         |
|------------------------------|-------------------------------------|
| `/api/health`                | API health check                    |
| `/api/v1/toi/active`         | Current active TESS Objects         |
| `/api/v1/schedule/next?n=10` | Next N recommended observation slots|
| `/docs`                      | Interactive API docs (Swagger UI)   |

---

## ⚙️ Deployment

### Docker


