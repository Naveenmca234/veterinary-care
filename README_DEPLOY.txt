# Veterinary Care Django Project - Render Deployment

This folder is prepared for deploying the Django project on Render.

## Render settings

Build Command:
./build.sh

Start Command:
gunicorn hospitalmanagement.wsgi:application

Environment Variables:
PYTHON_VERSION = 3.8.18
DEBUG = False
ALLOWED_HOSTS = *

## Notes

- This is a Django backend project, so do not deploy it on Netlify as a static site.
- The project includes db.sqlite3 for demo data.
- For college demo/submission this is okay.
- For real production, move the database to PostgreSQL because SQLite data can be lost on free hosting redeploy/restart.
