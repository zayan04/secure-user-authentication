# Secure User Authentication System

A secure and beginner-friendly user authentication web application built using **Python Flask**. This project provides essential authentication features with a focus on password security, session management, and access control.

## Features

- 📝 **User Registration** – Create a new account.
- 🔑 **Secure Login** – Authenticate users with their credentials.
- 🔒 **Password Hashing** – Store passwords securely using password hashing.
- 🚪 **Logout** – End the authenticated session.
- 🛡️ **CSRF Protection** – Protect forms against Cross-Site Request Forgery.
- 👤 **Session Management** – Manage user sessions with a configured lifetime.
- 🔐 **Protected Dashboard** – Restrict dashboard access to logged-in users.
- ⚙️ **Role-Based Access Control** – Restrict admin-only routes based on user roles.
- 🗄️ **SQLite Database** – Store user account information.

## Technologies Used

- Python
- Flask
- Flask-SQLAlchemy
- Flask-WTF
- SQLite
- HTML & CSS
- Git & GitHub

## Project Structure

```text
secure-user-authentication/
│
├── app.py
├── requirements.txt
├── .gitignore
│
├── static/
│   └── style.css
│
└── templates/
    ├── login.html
    ├── register.html
    └── dashboard.html
```

##  Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/zayan04/secure-user-authentication.git
```

### 2. Open the Project Folder

```bash
cd secure-user-authentication
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

### 4. Activate the Virtual Environment

**Windows PowerShell:**

```powershell
.\venv\Scripts\Activate.ps1
```

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

### 6. Configure Environment Variables

Create a `.env` file in the project root and add a strong secret key:

```env
SECRET_KEY=your-own-random-secret-key
```

Replace the example value with a securely generated random secret key. Never upload your actual `.env` file to GitHub.

### 7. Run the Application

```bash
python app.py
```

Open your browser and visit:

http://127.0.0.1:5000

## 🔐 Security Practices

- Passwords are hashed instead of being stored as plain text.
- CSRF protection is enabled for form submissions.
- Protected routes require authentication.
- Admin-only routes check user roles.
- Session cookies use HTTPOnly and SameSite settings.
- Secret configuration is kept in environment variables.

**Note:** For production deployment, use HTTPS, enable secure cookies, and configure production-grade secret management and database settings.

## Project Objective

The objective of this project is to understand and implement fundamental web application security practices, including user authentication, password protection, session handling, and role-based authorization.

##  Author

**Zayan**

GitHub: [@zayan04](https://github.com/zayan04)

---

If you find this project useful, consider giving the repository a star!
