# Flask Login Authentication System-

A simple Flask-based authentication application with registration and login pages, using SQLAlchemy and WTForms for database and form validation.

## Features-

- User registration with username, email, and password
- Password hashing using Werkzeug security
- Login with username and password
- Input validation for required fields, email format, and unique username/email
- Responsive HTML templates with CSS styling

## Project Structure

- `app.py` - Main Flask application with routes, database models, and forms
- `templates/` - Jinja2 templates for pages
  - `home.html` - Home page with links to login and registration
  - `login.html` - Login form template
  - `registration.html` - Registration form template
- `static/style.css` - Basic styles for the app
- `users.db` - SQLite database file created automatically when the app runs

## Requirements

- Python 3.8+ (recommended)
- Flask
- Flask-WTF
- Flask-SQLAlchemy
- WTForms
- Werkzeug

## Installation

1. Create and activate a virtual environment (recommended):

   ```bash
   python -m venv venv
   .\venv\Scripts\activate
   ```

2. Install dependencies:
   ```bash
   pip install Flask Flask-WTF Flask-SQLAlchemy WTForms
   ```

## Running the App

1. Start the application:

   ```bash
   python app.py
   ```

2. Open your browser and go to:

   ```
   http://127.0.0.1:5000/
   ```

3. Use the registration page to create a new user, then log in with the credentials.

## Notes

- The app uses an SQLite database file at `users.db`.
- `SECRET_KEY` is hardcoded in `app.py` for development; use a secure environment variable in production.
- The login route redirects to the home page on successful sign-in, but does not maintain persistent user sessions.

## Improvements

- Add session management with `flask_login`
- Add logout functionality
- Add email verification or password reset
- Secure the secret key and database configuration for production

##Created By--
Nikhil Gupta
