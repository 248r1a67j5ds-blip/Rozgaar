# GigShield

Runnable VS Code starter for the unified gig-worker logistics platform described in the supplied specification.

## Stack
- Frontend: React + TypeScript + Vite
- Backend: Python 3.11 + FastAPI + SQLAlchemy 2
- Database: SQLite by default for zero-setup local development; PostgreSQL/PostGIS supported through Docker
- Docker Compose included

## Run locally

### Backend
```bash
cd backend
python -m venv .venv
# Windows:
.venv\Scripts\activate
# macOS/Linux:
# source .venv/bin/activate

pip install -r requirements.txt
uvicorn app.main:app --reload
```

Backend: http://127.0.0.1:8000
Swagger: http://127.0.0.1:8000/docs

### Frontend
Open another terminal:
```bash
cd frontend
npm install
npm run dev
```

Frontend: http://localhost:5173

The frontend expects the backend at `http://127.0.0.1:8000`.
