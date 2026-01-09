# Django Shop - Learning Project

A learning e-commerce project built with Django featuring shopping cart functionality.

## Requirements

- Python 3.8+
- pip
- virtualenv (recommended)

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Siztonee/shop-django-learning.git
cd shop-django-learning
```

### 2. Create Virtual Environment

**For Linux/MacOS:**
```bash
python3 -m venv venv
source venv/bin/activate
```

**For Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Setup Database

Run migrations to create the database structure:

```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Create Superuser (Optional)

To access the Django admin panel:

```bash
python manage.py createsuperuser
```

Follow the console instructions to create an administrator account.

### 6. Run Development Server

```bash
python manage.py runserver
```

The project will be available at: http://127.0.0.1:8000/

Admin panel: http://127.0.0.1:8000/admin/

## Project Structure

```
shop-django-learning/
├── cart/           # Shopping cart application
├── main/           # Main application
├── shop/           # Shop products application
├── manage.py       # Django management utility
├── requirements.txt # Project dependencies
└── README.md       # Documentation
```

## Features

- Browse product catalog
- Add products to cart
- Shopping cart management
- Admin panel for content management

## Troubleshooting

**Migration errors:**
If you encounter database errors, try deleting the `db.sqlite3` file and migration files in `*/migrations/` folders (except `__init__.py`), then repeat step 4.

**Port already in use:**
If port 8000 is occupied, run the server on a different port:
```bash
python manage.py runserver 8080
```

## Development

This project was created for educational purposes to learn the Django framework.

## License

Educational project without a license.
