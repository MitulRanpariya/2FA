# 🔐 Two-Factor Authentication (2FA) System

A secure, full-stack Two-Factor Authentication (2FA) system built with **Spring Boot**, **Spring Security**, **React**, and **TypeScript**. It uses **JWT**, **TOTP-based 2FA**, **Google reCAPTCHA**, and **email verification** to provide robust user authentication.

---

## 🚀 Features

### ✅ Authentication System
- JWT-based login and registration
- Email verification link on registration
- Secure password reset functionality
- Session handling with refresh tokens

### 🔐 Two-Factor Authentication
- TOTP-based authentication (e.g., Google Authenticator)
- QR code-based setup
- Backup codes for account recovery

### 🛡️ Security Measures
- Google reCAPTCHA integration (v2/v3)
- Spring Security for endpoint protection
- Passwords securely hashed with BCrypt

### 📬 Email Service
- Email verification on signup
- Password reset emails with tokenized links

---

## 🧑‍💻 Tech Stack

### Backend (Spring Boot)
- Spring Security
- Java JWT
- Spring Data JPA
- MySQL
- Google Authenticator (TOTP)
- Java Mail Sender

### Frontend (React)
- React + TypeScript
- Material UI
- Axios
- React Router
- Google reCAPTCHA (react-google-recaptcha)

---

## ⚙️ Installation

### Prerequisites
- Java 17+
- Node.js + npm
- MySQL
- Maven

### Backend Setup
```
bash
git clone https://github.com/your-username/2fa-auth-system.git
cd backend
cp .env.example .env # configure DB, mail, and JWT secrets
./mvnw spring-boot:run
```

### Frontend Setup
```
bash
cd frontend
npm install
npm start
```

---

## 🔐 Environment Variables

### Backend `.env`
```
env
DB_URL=jdbc:mysql://localhost:3306/2fa_db
DB_USERNAME=root
DB_PASSWORD=yourpassword

JWT_SECRET=supersecretkey
EMAIL_USERNAME=youremail@example.com
EMAIL_PASSWORD=yourpassword
RECAPTCHA_SECRET=your_recaptcha_secret
```

### Frontend `.env`
```
env
REACT_APP_API_URL=http://localhost:8080
REACT_APP_RECAPTCHA_SITE_KEY=your_recaptcha_site_key
```

---

## 🛠️ Future Enhancements
- WebAuthn (biometric login)
- SMS-based 2FA
- Admin dashboard for user management

---

