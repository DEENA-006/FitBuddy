# FitBuddy - AI Fitness Plan Generator (FastAPI + Gemini)

Personalised 7-day workout plans (Gemini Pro), nutrition tips (Gemini Flash),
feedback-based plan updates, SQLite storage and an admin dashboard.

## Quick start (Windows / VS Code)
```powershell
python -m venv venv
venv\Scripts\activate            # macOS/Linux: source venv/bin/activate
pip install -r requirements.txt
copy .env.example .env           # macOS/Linux: cp .env.example .env
# edit .env and paste your GOOGLE_API_KEY from https://aistudio.google.com/app/apikey
uvicorn app.main:app --reload
```
Open http://127.0.0.1:8000  (API docs: http://127.0.0.1:8000/docs)

## Tests (no API key needed - Gemini is mocked)
```powershell
pip install -r requirements-dev.txt
pytest -v
```
