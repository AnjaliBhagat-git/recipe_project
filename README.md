# Acme Recipes - GraphQL Backend (Runnable)

## Quick start (local)

1. Create and activate a virtualenv, then install requirements:
```bash
python -m venv venv
source venv/bin/activate   # on Windows: venv\Scripts\activate
pip install -r requirements.txt
```

2. Run migrations and create a superuser:
```bash
python manage.py migrate
python manage.py createsuperuser
```

3. Start the server:
```bash
python manage.py runserver
```

4. Obtain JWT token (optional):
POST to `/api/token/` with JSON body `{ "username": "<youruser>", "password": "<yourpass>" }`.
Use returned `access` token in GraphQL requests as header:
`Authorization: Bearer <access>`

5. Open GraphiQL at: `http://127.0.0.1:8000/graphql/` (requires authentication via admin session or Bearer token).

## Notes
- This project uses SQLite and is configured for development convenience.
- The GraphQL endpoint enforces authentication: either a logged-in admin session or a valid JWT Bearer token.
