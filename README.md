# 🎬 Secure Movie Booking System

A secure web-based movie booking application developed using **Flask** and **SQLite**. The system allows users to register, browse movies, book tickets, and leave comments, while administrators can upload and manage movies. The application follows secure coding practices by implementing password hashing, strong password policies, rate limiting, secure file upload validation, and role-based authorization.

---

## Features

### User Features

* User registration with secure password validation
* Secure login and logout
* Browse all available movies
* Filter movies by category
* View detailed movie information
* Book movie tickets
* Comment on movies
* Session-based authentication

### Administrator Features

* Upload new movies
* Add movie posters
* Set ticket prices
* Categorize movies
* View accumulated ticket profits

---

## Security Features

* Password hashing using **bcrypt**
* Strong password policy enforcement

  * Minimum length
  * Uppercase letters
  * Lowercase letters
  * Numbers
  * Special characters
* Protection against brute-force attacks using **Flask-Limiter**
* Secure session management
* Role-based access control (Admin/User)
* Input validation
* Secure image upload validation

  * Allowed file extensions only
  * Maximum upload size restrictions
* Protection against unauthorized page access

---

## Technologies Used

### Backend

* Python
* Flask

### Database

* SQLite

### Frontend

* HTML
* CSS
* JavaScript
* Jinja2 Templates

### Security Libraries

* bcrypt
* Flask-Limiter

---

## Database

The application stores information for:

* Users
* Movies
* Ticket purchases
* Movie comments

SQLite is used as the backend database.

---

## Project Functionality

### User Authentication

Users create accounts using strong passwords that are securely hashed before being stored in the database.

### Movie Management

Administrators can upload movies with:

* Movie title
* Description
* Ticket price
* Category
* Poster image

### Ticket Booking

Users can:

* View movie details
* Purchase tickets
* See ticket availability

Each successful purchase updates the ticket counter and the movie owner's profit.

### Comments

Registered users can leave comments on movie pages, allowing interaction and discussion.

---

## Security Measures

This project demonstrates several secure web development practices, including:

* Secure password storage using bcrypt
* Password complexity enforcement
* Login request rate limiting
* Session-based authentication
* Authorization checks before accessing protected routes
* File type validation
* File size validation
* Restricted administrator functionality

---

## Installation

1. Clone the repository

```bash
git clone https://github.com/AlaaRabie1/movie-booking-project.git
```

2. Install the required packages

```bash
pip install flask bcrypt flask-limiter
```

3. Run the application

```bash
python app.py
```

4. Open your browser and visit

```
http://127.0.0.1:5000
```

---

## Future Improvements

* Online payment integration
* Email notifications
* Seat selection
* Movie search functionality
* User profiles
* Booking history
* Movie ratings
* Admin dashboard analytics
* Password reset functionality
* CSRF protection
* SQLAlchemy ORM integration

---

## Learning Objectives

This project demonstrates practical implementation of:

* Flask web development
* Authentication and authorization
* Secure password handling
* Session management
* File upload security
* SQLite database operations
* CRUD functionality
* Web application security best practices

---

## Author

**Alaa Rabie**

Developed as an academic project to demonstrate secure web application development using Flask.
