# Django HTMX WebSockets

A lightweight Django starter project demonstrating how to combine Django, HTMX, and websocket-style real-time interactions in a minimal, approachable codebase. This repository is designed as a practical foundation for apps that want the feel of a modern interactive frontend without introducing a large JavaScript framework.

## Overview

This project includes:

- Django project setup using the default SQLite configuration
- A small `core` app for the homepage and app structure
- HTMX-friendly templates and routing
- Custom user model support
- Authentication integration via `django-allauth`
- A clean starter layout for expanding into real-time interactive features

The repository is intentionally simple and readable, making it a good base for experimentation, learning, and extending with websocket functionality such as Django Channels.

## Features

- Django 4.1 application structure
- HTMX-ready frontend foundation
- Custom `User` model extending `AbstractUser`
- Allauth integration for login and account routes
- SQLite database by default for quick development
- Minimal but extensible project organization

## Tech Stack

- Python
- Django 4.1.6
- HTMX
- django-allauth
- django-extensions
- SQLite

## Project Structure

```text
.
├── core/
│   ├── templates/
│   │   └── core/
│   │       ├── base.html
│   │       └── index.html
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   └── views.py
├── htmx_websockets/
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── manage.py
├── requirements.txt
├── .gitignore
├── db.sqlite3
└── README.md
```

## Getting Started

### Prerequisites

- Python 3.10+
- pip
- virtualenv (recommended)

### Installation

1. Clone the repository:

```bash
git clone https://github.com/Chill119/django-htmx-websockets.git
cd django-htmx-websockets
```

2. Create and activate a virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate
```

On Windows:

```bash
python -m venv .venv
.venv\Scripts\activate
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

### Database Setup

Run the migrations:

```bash
python manage.py migrate
```

### Run the App

Start the development server:

```bash
python manage.py runserver
```

Then open:

```text
http://127.0.0.1:8000/
```

## Authentication

The project includes `django-allauth` and a custom user model. Authentication routes are mounted under `/accounts/`, and the app is configured to redirect to the home page after login.

## Development Notes

This starter is intentionally minimal and serves as a base for adding:

- real-time websocket functionality with Django Channels
- HTMX-driven interactions and partial page updates
- forms, CRUD flows, and user dashboards
- event-driven UI patterns with minimal JavaScript

## License

This repository does not currently include an explicit license file, so it is not yet formally licensed for broader reuse beyond the default GitHub terms unless a license is added later.

## Contributing

Contributions are welcome. If you'd like to improve the project, feel free to open an issue or submit a pull request.
