---
title: "EasyDoc – Appointment & User Management System"
excerpt: "A secure Django web app for patient appointments, user registration with email verification, and JWT-based authentication."
layout: single
author_profile: true
read_time: true
share: true
related: true
permalink: /projects/easydoc/
header:
  image: /assets/images/lunch-app-thumbnail.jpg
  teaser: /assets/images/easy_doc/easydoc.jpg
---

## 📝 Project Overview

**EasyDoc** is a Django-powered medical appointment and user management system. It allows patients to book appointments, notifies administrators, and handles user authentication with email verification and JWT tokens — all within a secure web interface.

---

## 🧱 Tech Stack

- **Backend:** Django, Django REST Framework  
- **Templating:** Django Templates (HTML/CSS)  
- **Database:** PostgreSQL  
- **Authentication:** JWT (via `rest_framework_simplejwt`)  
- **Email:** SMTP via `EmailMessage` and `send_mail`  
- **Token Handling:** JSON Web Tokens (JWT) with expiration and payload signing  
- **Validation:** Regex + Django’s built-in validators  

---

## ✨ Key Features

### ✅ Patient Interface

- **Book Appointments:**  
  Users submit validated appointment requests with name, email, phone, and a custom message.

- **Appointment History (API):**  
  Authenticated users can retrieve their past appointments through a secure REST endpoint.

- **Email Feedback:**  
  Users receive confirmation of appointment submission and response emails once accepted.

---

### 🔐 Authentication & Security

- **JWT Login System:**  
  Login issues access and refresh tokens stored in **HttpOnly** cookies for secure session handling.

- **Email-Based Activation:**  
  New users receive an activation link encoded with a JWT payload and expiration.

---

### 🛠️ Admin Panel

- **Appointment Management Dashboard:**  
  Admins can view, paginate, and accept appointment requests.

- **Automated Email Responses:**  
  HTML emails are sent to patients upon appointment acceptance, confirming time and details.

---

## 🔒 Security Highlights

- HttpOnly cookies for JWT tokens to prevent XSS  
- Custom regex validation for form inputs  
- User accounts remain inactive until verified via email  
- Expiring JWT tokens for secure email-based activation links

---

## 📌 Opportunities for Enhancement

- Add reCAPTCHA to forms to prevent spam  
- Use Celery + Redis for asynchronous email dispatch  
- Migrate input logic to Django `ModelForms` for cleaner validation  
- Expand the dashboard with analytics or appointment filters  
- Improve frontend with TailwindCSS or Bootstrap for responsive design

---

## 📂 Source & Demo

> *(Add these if applicable)*  
- 🔗 **GitHub:** (https://github.com/Python-on-my-backend/webSecurity)
<!-- - 🌐 **Live Demo:** [yourdomain.com/easydoc](https://yourdomain.com/easydoc) -->

