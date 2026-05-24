# Little Lemon API
Backend API for the Little Lemon restaurant project built with Django and Django REST Framework.
This project was developed as part of the Meta Backend Developer Capstone and implements a restaurant menu and booking system with authentication, permissions, API endpoints, and unit testing.
---

## Features

- Restaurant menu management API
- Table booking system
- Django REST Framework integration
- Token-based authentication
- Protected endpoints with permissions
- Django admin panel
- Unit tests
- ViewSets and Generic API Views
- Djoser authentication support
---

## Tech Stack

- Python
- Django
- Django REST Framework
- MySQL
- Djoser
- DRF Token Authentication

---

## Installation

Clone repository:

```bash
git clone <repository-url>
cd LittleLemon
```

Create virtual environment:

```bash
python -m venv venv
```

Activate virtual environment:

Mac/Linux:

```bash
source venv/bin/activate
```

Windows:

```bash
venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Apply migrations:

```bash
python manage.py migrate
```

Create superuser:

```bash
python manage.py createsuperuser
```

Run server:

```bash
python manage.py runserver
```

---

## API Endpoints

### Menu API

```text
GET      /api/menu-items/
POST     /api/menu-items/

GET      /api/menu-items/<id>
PUT      /api/menu-items/<id>
DELETE   /api/menu-items/<id>
```

### Booking API

```text
GET      /api/booking/
POST     /api/booking/

GET      /api/booking/<id>
PUT      /api/booking/<id>
DELETE   /api/booking/<id>
```

### Authentication
POST     /auth/token/login/
POST     /api/api-token-auth/


### Admin Panel
http://127.0.0.1:8000/admin/
---

## Testing

Run tests:

```bash
python manage.py test
```

Current status:
Ran 3 tests
OK

---

## Project Structure
LittleLemon/
│
├── LittleLemon/
├── LittleLemonAPI/
├── tests/
├── manage.py
├── requirements.txt
└── README.md
```

---

## Authentication and Security Notes

This project includes:

- Token Authentication
- Protected API endpoints
- Permission classes
- Djoser authentication integration

This application was created according to Meta/Coursera capstone project requirements.

Some configuration choices follow the educational implementation used in the course.

For production environments:

- secrets should be stored in environment variables
- sensitive credentials should never be committed
- authentication tokens should be secured appropriately

This repository is intended for educational and portfolio purposes.

---

## Author

Mersaid Zhaxybayev

Meta Backend Developer Capstone Project
