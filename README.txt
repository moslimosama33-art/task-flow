# TaskFlow - Flask + SQLAlchemy

## Run

1. Open this folder in VS Code.
2. Open Terminal.
3. Install packages:

    pip install -r requirements.txt

4. Run:

    python app.py

5. Open:

    http://127.0.0.1:5000

The SQLite database `taskflow.db` is created automatically.

## Database relationship

User 1 ---- Many Task

User:
- id (PK)
- username
- password

Task:
- id (PK)
- title
- description
- priority
- due_date
- done
- user_id (FK -> User.id)

Passwords are stored as hashes, not plain text.
