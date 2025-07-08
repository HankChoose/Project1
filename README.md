# 📚 CS50W Wiki Project

This is my submission for the CS50 Web Programming with Python and JavaScript course — Project 1: **Wiki**.

The project is a Wikipedia-like online encyclopedia built with Django. Entries are stored in Markdown format and rendered into HTML.

---

## ✅ Features

- Create, edit, and delete encyclopedia entries
- Search for entries (exact or partial match)
- Display random entries
- Markdown to HTML rendering using `markdown2`
- Fully responsive with Bootstrap

---

## 🖥️ How to Run Locally (for Grading)

### 1. Clone this repository

```bash
git clone https://github.com/YOUR_USERNAME/cs50w-wiki.git
cd cs50w-wiki
```

### 2. (Optional) Create and activate a virtual environment

```bash
python3 -m venv venv
source venv/bin/activate        # macOS/Linux
# venv\Scripts\activate.bat     # Windows
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Django development server

```bash
python manage.py runserver
```

Then open your browser and go to:  
**http://127.0.0.1:8000/**

---

## 📁 Project Structure

```
wiki/
├── manage.py
├── encyclopedia/        # Django app
├── entries/             # Markdown content
├── wiki/                # Project settings
├── requirements.txt     # Python dependencies
├── README.md            # You're reading it!
├── Dockerfile           # (Optional) Docker support
├── docker-compose.yml   # (Optional) Dev environment
└── nginx/
    └── nginx.conf       # (Optional) Nginx config
```

---

## 🐳 Optional: Run with Docker (Advanced)

This project also includes Docker support for development or deployment.

### 1. Build and start containers

```bash
docker-compose up --build
```

### 2. Visit your site

```
http://localhost/
```

This runs:
- Django app in one container
- Nginx as a reverse proxy

### Live Demo (Optional)

You can view a live version deployed at:  
🌐 https://raybeststar.com

---

## 📦 Dependencies

See `requirements.txt`, but mainly:

- Django >= 4.0
- markdown2

---

## ✅ Notes

- No login is required — this is a single-user system
- All data is stored in `.md` files under `/entries/`
- Docker and deployment are optional and **not required for grading**

---

## 📧 Contact

Feel free to reach out via GitHub or email if you have questions!
