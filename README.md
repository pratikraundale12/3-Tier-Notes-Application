# 📝 Django Notes Application

A simple Notes application built with **Django** and optionally React, containerized using **Docker Compose** for seamless development and deployment.

## 📦 Requirements

- Python 3.9
- Node.js (optional, if using frontend)
- Docker
- Docker Compose

## 🚀 Getting Started

### ▶️ Using Docker Compose

```bash
git clone https://github.com/your-username/django-notes-app.git
cd django-notes-app
docker-compose up --build
```

### ▶️ Running Locally without Docker

```bash
cd django-notes-app
python -m venv venv
venv\Scripts\activate      # On Windows
# source venv/bin/activate  # On macOS/Linux
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

**Visit:** http://127.0.0.1:8000
