# Task 3 – Advanced Security, Logging & Finalization

## 🎯 Objective
To perform basic penetration testing, implement logging with Winston, and document key web security best practices.

## 🧪 Environment
- Kali Linux (VMware)
- Node.js + Express
- Terminal-based tools

## 🛠️ Tools & Libraries Used
- **Nmap** – Port scanning and service fingerprinting
- **Winston** – Logging for activity tracking
- **Helmet** – HTTP header protection
- **curl** – API testing

---

## ✅ Tasks Completed

### 1. **Penetration Testing (Nmap)**
- Ran port scan:
  ```bash
  nmap -sV -p 3000 localhost
  Verified:

Port 3000 is open

Helmet headers are applied in HTTP response



2. Winston Logging

Winston configured to:

Log app startup

Log login attempts

Save logs to security.log file


Example:

const winston = require('winston');
const logger = winston.createLogger({
  transports: [
    new winston.transports.Console(),
    new winston.transports.File({ filename: 'security.log' })
  ]
});
logger.info('Application started');


3. Security Checklist

Created security_checklist.txt with:

Input validation (validator.js)

Password hashing (bcrypt)

Authentication (JWT)

Helmet protection

Logging with Winston

Nmap scan

Best practice suggestions (HTTPS, .env, rate limiting)



---

📂 Files Included

index.js – Final secured application code

security.log – Logged activities

security_checklist.txt – Checklist of applied practices

---

📌 Conclusion

Completed final stage of the internship project with:

Port scan validation

Proper activity logging

Documentation of secure practices


All files are verified and ready for review.
