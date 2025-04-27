# SDEV_220_Final_Project_Group5

# SDEV_220_Final_Project_Group5

## Installation and Running Guide for Inventory Management System

### Project Structure

/
├── inventory/                    # Main app for warehouse management
│   ├── migrations/               # Database migration files
│   │   └── __init__.py
│   ├── templates/                # HTML templates
│   │   └── inventory/
│   │       ├── base.html         # Base template
│   │       ├── supply_list.html  # Supply list page
│   │       ├── supply_form.html  # Supply add/edit form
│   │       ├── location_list.html # Location list page
│   │       ├── location_form.html # Location add/edit form
│   │       ├── user_list.html    # User list page
│   │       ├── user_form.html    # User add/edit form
│   │       └── alert_list.html   # Alerts list page
│   ├── static/                   # Static files
│   │   ├── css/                  # CSS files
│   │   ├── js/                   # JavaScript files
│   │   └── images/               # Image files
│   ├── models.py                 # Application models
│   ├── views.py                  # Application views (business logic)
│   ├── urls.py                   # URL patterns
│   ├── admin.py                  # Admin site configuration
│   ├── forms.py                  # Django forms
│   ├── tests.py                  # Unit tests
│   └── __init__.py               # Package initializer
├── inventory_management/         # Project settings
│   ├── settings.py               # Project configuration
│   ├── urls.py                   # Root URL configuration
│   ├── wsgi.py                   # WSGI configuration
│   ├── asgi.py                   # ASGI configuration
│   └── __init__.py               # Package initializer
├── manage.py                     # Django management script
├── requirements.txt              # Required packages list
├── README.md                     # Project documentation
├── .gitignore                    # Git ignore rules
└── db.sqlite3                    # SQLite database file

## Detailed description of components

### 1. Directory repository/
- **migrations/**: Contains migration files to manage database changes
- **templates/**: Contains HTML templates
- `base.html`: Base template with common layout
- `supply_list.html`: Displays product list
- `supply_form.html`: Product add/edit template
- `location_list.html`: Displays location list
- `location_form.html`: Add/edit form location
- `user_list.html`: Displays user list
- `user_form.html`: Add/edit user form
- `alert_list.html`: Displays alert list

- **static/**: Contains static files
- `css/`: CSS files
- `js/`: JavaScript Files

- `images/`: Image image files

- **models.py**: Model definitions

- Provisioning source: Product model

- Location: Model location

- User: Model user

- Alerts: Alert model

- **views.py**: Logic processing
- CRUD operations for models
- Processing forms
- Access checks
- Alert handling

- **urls.py**: URL template definitions
- URLs for views
- URLs for API endpoints

- **admin.py**: Admin interface configuration
- Model registration
- Custom screens

- **forms.py**: Form definitions
- Provisioning templates
- Location forms
- User forms

- **tests.py**: Unit tests
- Test models
- Test views
- Forms test

### 2. Inventory_management/ directory
- **settings.py**: Project settings
- Database configuration
- Installed applications
- Middleware
- Templates
- Static files
- Security settings

- **urls.py**: Main template URL
- Includes application URLs
- Admin URLs
- API URLs

- **wsgi.py**: WSGI configuration
- **asgi.py**: ASGI configuration

### 3. Other files
- **manage.py**: Django management scripts
- **requirements.txt**: Dependency list
- **README.md**: Project documentation
- **.gitignore**: Git ignore rules
- **db.sqlite3**: SQLite database file

## System requirements
- Python 3.8 or later
- pip (Package Manager) Python)
- Virtual Environment (recommended)

## Installation Steps

1. **Install Virtual Environment (Virtual Environment)**
``` bash
# Create Virtual Environment
python -m venv venv

# Activate Virtual Environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
```

2. **Install Required Packages**
``` bash
pip install -r require.txt
```

3. **Configure Database**
``` bash
# Create Tables in Database
python manage migrate with python
python manage.py migrate
```

4. **Create Superuser (Administrator)**
``` bash
python manage.py createsuperuser
```

5. **Run the server**
``` bash
python server management run.py
```

##Instructions for use

1. **Login**
- Access http://localhost:8000/admin/
- Created login information with superuser account

2. **Manage products (Supplies)**
- View product list: http://localhost:8000/inventory/supplies/
- Add new product: Click “Add new supply”
- Edit product information: Click edit icon
- Delete product: Click delete icon
- Filter out-of-stock products: Use the checkbox "Only show out-of-stock products"
- Search for products: Use the search box

3. **Manage locations (Location)**
- View location list: http://localhost:8000/inventory/locations/
- Add new location: Click on “Add new location”
- Edit location information: Click on the edit icon
- Delete location: Click on the delete icon

4. **User management (User management)**
- View user list: http://localhost:8000/inventory/users/
- Add new user: Click on "Add new user"
- Edit user information: Click on the edit icon
- Delete user: Click on the delete icon

5. **Alert management (Alerts)**
- View alert list: http://localhost:8000/inventory/alerts/
- Mark as read: Click on "Mark as read"
- Delete alert: Click on the delete icon

##Key features
- Manage products with detailed information
- Manage warehouse locations
- Manage users and permissions
- Automatic warning when products are running out of stock
- Search and filter products quickly
