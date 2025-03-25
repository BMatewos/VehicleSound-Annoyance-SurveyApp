# VehicleSound-AnnoyanceSurveyApp

A web-based application to collect and analyze human perception of vehicle sound annoyance.

---

## Project Overview

This app allows users to:
- Listen to vehicle sounds (car, motorcycle, truck, or other)
- Classify the type of vehicle
- Rate the loudness (annoyance level)

All user responses are stored for further analysis.

---

## Technology Stack

- **Backend:** Python (Flask)
- **Frontend:** HTML, CSS
- **Database:** MySQL
- **Data Analysis:** Python (Pandas, NumPy)

---

## 👥 User Roles

### Administrator
- Full access to all features and resources.
- Can manage users, generate reports, and configure system settings.

### Standard User
- Can access and interact with vehicle sound classification and rating.
- Cannot modify system settings or manage users.

---

## 🔐 User Credentials

- **Email:** Used as a unique identifier for login.
- **Password:** Must be at least **3 characters** long.
- Passwords are **hashed using MD5** before being stored in the database for security.

---

## Authentication Process

- **Registration:**
  - Users sign up with their email and password.
  - Password must be at least 3 characters and confirmed to avoid errors.
  - The password is hashed with MD5 before storage.

- **Login:**
  - Users enter email and password.
  - The system checks if the email exists and matches the hashed password.
  - On success, a session is created for the user.

---

## Session Management

- A session begins after successful login.
- It tracks user interactions during their time on the application.
- Sessions ensure personalized and secure user experience.

---

## Relational Diagram

![Relational Schema](images/relational_schema.png)

