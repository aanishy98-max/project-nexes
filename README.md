# CampusOS Prototype

Dual-surface prototype (web + mobile) with a real ML inference layer (TF-IDF + Logistic Regression) synced via a FastAPI backend.

## Structure
- backend/ - FastAPI + ML model
- web/ - Static web UI (e-commerce inspired)
- mobile/ - React Native UI (Expo ready)
- docs/ - Architecture

## Backend
```bash
cd backend
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
uvicorn app.main:app --reload --port 8000
```

## Web
Open `web/index.html` directly in a browser or serve with any static server.

## Mobile
```bash
cd mobile
# Create an Expo app in this folder and replace App.js if needed
```

## Key API Endpoints
- POST `/pulse/summary`
- POST `/exchange/score-listing`
- POST `/exchange/travel-match`
- POST `/sync/event`
