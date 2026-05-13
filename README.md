# 📝 iCoder - Blog Web App

> A full-featured blog web application built with **Python & Django**, featuring user authentication, post management, categories, and a clean responsive UI.

---

## 📋 Table of Contents

- [About](#about)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Usage](#usage)

---

## About

**iCoder** is a Django-based blogging platform where users can create accounts, write and publish posts, browse content by category, and interact through a clean web interface. It was built as a hands-on Django learning project, covering the full web development cycle from models and views to templates and URL routing.

---

## Features

- 🔐 **User Authentication** — Register, login, and logout functionality
- ✍️ **Post Management** — Create, read, update, and delete blog posts
- 🗂️ **Categories** — Organize posts by topic/category
- 👤 **User Profiles** — Each author has their own profile page
- 🔍 **Browse Posts** — View all posts or filter by category/author
- 🛡️ **Admin Panel** — Django admin interface for full content management
- 📱 **Responsive Design** — HTML templates styled for clean, readable layout

---

## Tech Stack

| Layer | Technology |
|---|---|
| Backend | Python, Django |
| Frontend | HTML, CSS, Django Templates |
| Database | SQLite (default) |
| Admin | Django Admin Panel |

---

## Project Structure

```
iCoder/
└── django blog/
    └── icoder/
        ├── manage.py               # Django management CLI
        ├── icoder/                 # Project config
        │   ├── settings.py         # App settings & config
        │   ├── urls.py             # Root URL routing
        │   └── wsgi.py             # WSGI entry point
        ├── blog/                   # Main blog app
        │   ├── models.py           # Post, Category, Author models
        │   ├── views.py            # View logic
        │   ├── urls.py             # Blog URL patterns
        │   ├── admin.py            # Admin panel config
        │   └── templates/          # HTML templates
        └── db.sqlite3              # SQLite database
```

---

## Getting Started

### Prerequisites

Make sure you have the following installed:

- Python 3.x
- pip

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/sb-0709/iCoder.git
cd iCoder/django\ blog/icoder
```

**2. Create a virtual environment**

```bash
python -m venv venv

# Activate it:
# On macOS/Linux:
source venv/bin/activate

# On Windows:
venv\Scripts\activate
```

**3. Install dependencies**

```bash
pip install django
```

> If a `requirements.txt` exists, use: `pip install -r requirements.txt`

**4. Apply migrations**

```bash
python manage.py makemigrations
python manage.py migrate
```

**5. Create a superuser (admin account)**

```bash
python manage.py createsuperuser
```

**6. Run the development server**

```bash
python manage.py runserver
```

**7. Open in your browser**

```
http://127.0.0.1:8000/
```

---

## Usage

Once the server is running:

- **Register** a new account or log in with your superuser credentials
- **Create posts** from the dashboard or admin panel
- **Browse posts** on the homepage, filter by category
- **Manage content** via the Django admin at `/admin/`

---
