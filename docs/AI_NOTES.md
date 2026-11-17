# How I used AI

## Prompts
- Asked AI to explain the assessment and break it into steps
- Asked for requirements doc, Django model, seed script, API, insights, tests, React UI

## What I verified myself
- Ran the seed script and checked the count is 10,000
- Ran all tests (6 pass)
- Fixed the CORS error by checking settings.py
- Fixed the missing import in views.py by reading the traceback

## Decisions I made
- Insights grouped by currency to avoid mixing INR and USD
- Aggregates in the DB, median in Python (SQLite has no median)
- Left out auth, payroll, currency conversion (see REQUIREMENTS.md)