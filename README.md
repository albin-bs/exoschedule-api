# ExoSchedule API

Backend API for ExoSchedule – an intelligent, AI-powered exoplanet observation scheduler built for the NASA Space Apps Challenge.

## 🌌 Overview

ExoSchedule API powers the backend scheduling and scoring engine for astronomers to optimize ground-based follow-up of exoplanet candidates, automating recommendations using NASA data and machine learning. This API connects to the ExoSchedule frontend at [https://flowbound.me](https://flowbound.me).

**Key Features:**
- RESTful FastAPI service
- Integrates NASA Exoplanet Archive and TESS data
- Intelligent Bayesian scheduling and prioritization
- Real-time updating of TOI (TESS Objects of Interest) status and observation plans
- Designed for seamless connection to lightweight web frontends

---

## 🚀 Quick Start

**Prerequisites:**  
- Python 3.11+  
- pip

**Install and Run:**
git clone https://github.com/albin-bs/exoschedule-api.git
cd exoschedule-api
python -m venv .venv
source .venv/bin/activate # (Windows: .venv\Scripts\activate)
pip install -r requirements.txt
uvicorn app.main:app --reload --port 8000

API will now be running at http://localhost:8000

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

**Docker:**
docker build -t exoschedule-api .
docker run -p 8000:8000 exoschedule-api


**Cloud:**  
Deployable to [Render](https://render.com), [Railway](https://railway.app), or any Docker host.

---

## 🛰️ NASA Data & Challenge

This solution addresses the Space Apps Challenge:  
**A World Away: Hunting for Exoplanets with AI**.  
It uses these core NASA resources:
- [NASA Exoplanet Archive](https://exoplanetarchive.ipac.caltech.edu/)
- [TESS MAST Portal](https://mast.stsci.edu/portal/Mashup/Clients/Mast/Portal.html)

---

## 🤖 Technologies Used

FastAPI, Uvicorn, Numpy, Pandas, Scikit-learn, Astropy, Docker

---

## 💡 License

MIT

---

## 👩‍🚀 Acknowledgments

- NASA Space Apps Challenge
- NASA Exoplanet Science Institute
- TESS Project and MIT MAST Archive

---

## 📫 Project Contact

For questions, raise an issue or contact [albin-bs](https://github.com/albin-bs).
