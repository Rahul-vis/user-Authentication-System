# Flask Authentication System

A simple Flask Authentication System that provides user registration, login, logout, password hashing, session management, and a protected dashboard.

## Features

* User Registration
* User Login
* User Logout
* Password Hashing using Werkzeug
* Session Management
* Protected Dashboard
* SQLite Database Integration
* Responsive UI with HTML, CSS, and Flask Templates

## Technologies Used

* Python
* Flask
* Flask-SQLAlchemy
* SQLite
* HTML5
* CSS3
* Jinja2 Templates

## Project Structure

```text
flask_auth_app/
│
├── app.py
├── database.db
│
├── static/
│   └── style.css
│
└── templates/
    ├── register.html
    ├── login.html
    └── dashboard.html
```

## Installation

### 1. Clone Repository

```bash
git clone https://github.com/your-username/flask-auth-app.git
cd flask-auth-app
```

### 2. Create Virtual Environment

```bash
python -m venv venv
```

### 3. Activate Virtual Environment

Windows:

```bash
venv\Scripts\activate
```

Linux/Mac:

```bash
source venv/bin/activate
```

### 4. Install Dependencies

```bash
pip install flask flask_sqlalchemy
```

### 5. Run Application

```bash
python app.py
```

### 6. Open Browser

```text
http://127.0.0.1:5000
```

## Authentication Flow

### Registration

* User enters username and password.
* Password is hashed before storing in the database.
* User account is created successfully.

### Login

* User enters credentials.
* Password hash is verified.
* Session is created for authenticated user.

### Dashboard

* Only logged-in users can access the dashboard.
* Unauthorized users are redirected to the login page.

### Logout

* Session data is removed.
* User is redirected to the login page.

## Security Features

* Password Hashing
* Session-Based Authentication
* Protected Routes
* Input Validation

## Future Improvements

* Email Verification
* Forgot Password Functionality
* User Profile Management
* Role-Based Authentication
* REST API Integration

## Author

Rahul Vishwakarma

## License

This project is created for educational and internship purposes.
