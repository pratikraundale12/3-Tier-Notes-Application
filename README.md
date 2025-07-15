# 📝 Django Notes Application

A simple Notes application built with **Django** and optionally React, containerized using **Docker Compose** for seamless development and deployment.

---

## 📦 Requirements

- Python 3.9
- Node.js (optional, if using frontend)
- Docker
- Docker Compose

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/django-notes-app.git
cd django-notes-app
2. Run with Docker Compose
bash
Copy
Edit
docker-compose up --build
Visit the app at: http://localhost:8000

🗂️ Project Structure
bash
Copy
Edit
django-notes-app/
├── api/                     # Django app for notes
├── django-notes-app/        # Django project folder
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
├── .env                     # Environment variables
└── README.md
⚙️ Environment Setup
Create a .env file in the root directory with:

env
Copy
Edit
DB_NAME=test_db
DB_USER=root
DB_PASSWORD=root
DB_HOST=127.0.0.1
DB_PORT=3306
🐳 Docker Commands
Build and start the containers:

bash
Copy
Edit
docker-compose up --build
Stop the containers:

bash
Copy
Edit
docker-compose down
🧪 Migrations & Admin
Run database migrations (inside container):

bash
Copy
Edit
docker-compose exec web python manage.py makemigrations
docker-compose exec web python manage.py migrate
Create superuser (optional):

bash
Copy
Edit
docker-compose exec web python manage.py createsuperuser
💻 Run Locally (without Docker)
bash
Copy
Edit
cd django-notes-app
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
