# Flask Authentication API with MySQL & Swagger
A simple Flask-based authentication system featuring **user registration, login, logout**, backed by **MySQL**.

## Features
    - User Registration
    - User Login & Logout
    - Session-based Authentication
    - MySQL Database Integration
    - Environment Variable Configuration (`.env`)

## Tech Stack
    - **Backend:** Flask (Python)
    - **Database:** MySQL
    - **ORM/Connector:** flask-mysqldb
    - **API Docs:** Swagger (Flasgger)
    - **Config:** python-dotenv


## Project Structure
    flask-login/
    ├── app.py
    ├── .env
    ├── requirements.txt
    └── README.md


## Installation & Setup

###  Clone the Repository
    https://github.com/aayushmapokhrel/Flask-Authentication.git
    
    python -m venv venv
    venv\Scripts\activate      # Windows
    source venv/bin/activate   # Linux/Mac

### Install Dependencies
    pip install -r requirements.txt

### Environment Variables
    SECRET_KEY=''
    MYSQL_HOST=''
    MYSQL_USER=''
    MYSQL_DB=''

### Database Setup
#### Example
    CREATE DATABASE database_name;
    
    CREATE TABLE table_name (
        id INT AUTO_INCREMENT PRIMARY KEY,
        username VARCHAR(100) NOT NULL UNIQUE,
        password VARCHAR(255) NOT NULL,
        email VARCHAR(100) NOT NULL
    );

### Run the Application
    python app.py
    http://127.0.0.1:5000

### API Endpoints
    | Method | Endpoint    | Description       |
    | ------ | ----------- | ----------------- |
    | GET    | `/`         | check             |
    | POST   | `/login`    | User login        |
    | POST   | `/register` | User registration |
    | GET    | `/logout`   | User logout       |



