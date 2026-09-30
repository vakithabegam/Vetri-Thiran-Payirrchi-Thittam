# PocketSmart AI

PocketSmart AI is a budget-aware Generative AI recommendation
assistant.

It provides three planning modules:

1. Home Interior Planner
2. Party Budget Planner
3. Jewelry Planner

The application uses:

- FastAPI
- Jinja2
- Vanilla JavaScript
- SQLite
- JWT authentication
- Gemini API
- Optional image input for jewelry recommendations
- Recommendation history
- Marketplace search links


# Project Structure

```text
PocketSmartAI/
│
├── app/
│   ├── __init__.py
│   ├── config.py
│   ├── database.py
│   ├── models.py
│   ├── schemas.py
│   ├── security.py
│   ├── main.py
│   │
│   ├── routers/
│   │   ├── __init__.py
│   │   ├── auth.py
│   │   ├── session.py
│   │   ├── planners.py
│   │   └── pages.py
│   │
│   ├── services/
│   │   ├── __init__.py
│   │   ├── ai_service.py
│   │   ├── marketplace_service.py
│   │   └── recommendation_service.py
│   │
│   ├── static/
│   │   ├── style.css
│   │   └── app.js
│   │
│   └── templates/
│       ├── index.html
│       ├── login.html
│       ├── register.html
│       ├── dashboard.html
│       ├── home_planner.html
│       ├── party_planner.html
│       └── jewelry_planner.html
│
├── tests/
│   ├── __init__.py
│   ├── conftest.py
│   └── test_app.py
│
├── .env.example
├── .gitignore
├── Dockerfile
├── docker-compose.yml
├── README.md
└── requirements.txt