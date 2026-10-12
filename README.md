# Student Management — Flask CRUD Demo

A small Python/Flask application for adding, listing and deleting student records using Flask-SQLAlchemy and SQLite.

## Local setup

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python app.py
```

Visit http://127.0.0.1:5000. The application requires its existing `templates/index.html` template.

## Deployment considerations

**Not suitable for unrestricted public write access as-is.** The current routes allow unauthenticated additions and deletions. Before production hosting, add authentication, authorization, CSRF protection, form validation and a persistent managed database. SQLite stored on an ephemeral cloud filesystem may lose records on restart.

This is an educational Flask project. Do not upload real student personal information into an open demo.

Maintainer: [Mohsin Pathan](https://github.com/Mohsinpathan17).
