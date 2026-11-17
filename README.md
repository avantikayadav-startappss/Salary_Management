# ACME Salary Management

Web app for the HR Manager to manage salaries of 10,000 employees across countries
and answer "how do we pay people" questions.

## Stack
Django + DRF, SQLite, React (Vite) + Ant Design

## Setup
Backend:
    python -m venv env
    env\Scripts\activate
    pip install -r requirements.txt
    python manage.py migrate
    python manage.py seed_employees
    python manage.py runserver

Frontend:
    cd frontend
    npm install
    npm run dev

Open http://localhost:5173

## Tests
    python manage.py test

## API
- GET/POST /api/employees/ (supports ?search=, ?country=, ?job_title=, ?page=)
- GET/PUT/DELETE /api/employees/<id>/
- GET /api/insights/by-country/
- GET /api/insights/by-job-title/

## Design decisions
See docs/REQUIREMENTS.md and docs/AI_NOTES.md