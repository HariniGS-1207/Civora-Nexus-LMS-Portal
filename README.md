# 🎓 Civora Nexus LMS

<p align="center">
  <strong>A Production‑Ready Learning Management System built with Django</strong><br>
  Role‑based access • Progress tracking • Certificates with QR verification • Responsive UI
</p>

---

## ✨ Overview

**Civora Nexus** is a full‑stack **Learning Management System (LMS)** developed as an internship project, focusing on **real‑world workflows, clean UI/UX, security, and scalability**.

The system supports **Admins, Teachers, and Students**, provides **course progress tracking**, and issues **QR‑enabled certificates** that can be publicly verified on any device.

---

## 🚀 Implemented Features

### 🔐 Authentication & Roles

* Custom user model with profile‑based roles
* Role‑based access control (Admin / Teacher / Student)
* Secure login & session handling

---

### 📚 Course Management

* Course categorization
* Search functionality
* Lesson‑based course structure
* Locked lessons until prerequisites are completed

---

### 📊 Progress Tracking

* Lesson completion tracking
* Course progress percentage
* Certificate unlocked only after completion

---

### 🧑‍🏫 Dashboards

**Admin Dashboard**

* User management (students & teachers)
* Course approval & moderation
* System statistics (users, courses, certificates)

**Teacher Dashboard**

* Create & manage courses
* Add and update lessons
* Track enrollments

**Student Dashboard**

* Enrolled courses overview
* Progress visualization
* Certificate access

---

### 🎓 Certificate System

* Automatic certificate generation (PDF)
* QR code embedded in certificates
* Downloadable certificates

#### 🔍 Certificate Verification

* Public verification page
* QR code scanning via mobile camera
* Three verification states:

  * ✅ Valid certificate
  * ⚠️ Revoked / inactive
  * ❌ Invalid certificate ID

---

## 🌐 QR Code Mobile Compatibility (Major Fix)

**Issue:**
QR codes were hard‑coded to `127.0.0.1`, failing on mobile devices.

**Solution:**
Dynamic URL generation using request‑based host detection with automatic HTTP/HTTPS support.

**Result:**

* Works on Wi‑Fi, mobile data, and production servers
* Mobile camera scanning supported
* Production‑ready implementation

---

## 🎨 UI / UX Enhancements

### 🏠 Home Page

* Gradient hero section with CTA
* About section with feature highlights
* Live statistics dashboard
* Featured courses
* SEO‑friendly & responsive layout

### 📄 Verification Pages

* Professional card‑based design
* Status‑based color coding
* Clear user guidance
* Mobile‑optimized layout

---

## 📱 Responsive Design

* Desktop (≥1200px)
* Tablet (≥768px)
* Mobile (<768px)

Fully optimized for touch interaction and readability.

---

## ⚡ Performance & Quality

* Optimized database queries
* Clean separation of logic
* No hard‑coded credentials
* CSRF protection enabled
* No performance regressions

---

## 🛠️ Tech Stack

* **Backend:** Django (Python)
* **Frontend:** HTML5, CSS3, Flexbox
* **Database:** SQLite (dev) / PostgreSQL (prod‑ready)
* **Authentication:** Django Auth + Custom Profiles
* **PDF Generation:** Django‑based PDF rendering

---

## 🗓️ Development Timeline (Internship Log)

**Day 1:** Designed the required project structure, apps, models, and initial templates for the LMS.

**Day 2:** Continued Django development by implementing authentication, role-based access, and core app logic.

**Day 3:** Completed and verified the **course enrollment flow**, ensuring proper access control and data consistency.

**Day 4:** Implemented **lesson-level progress tracking**, enabling accurate course completion monitoring.

**Day 5:** Enhanced the **student dashboard** with key LMS features such as enrolled courses, progress visualization, and certificate access.

---

## 📂 Project Structure

```text
Civora-Nexus/
├── certificates/
├── courses/
├── users/
├── templates/
│   ├── home.html
│   └── certificates/
├── static/
│   ├── eduvillage/   # Assets folder (CSS, images, icons, UI resources)
│   │   ├── css/
│   │   ├── images/
│   │   └── js/
├── manage.py
└── README.md
```

---

## 🧪 Testing Checklist

* QR code scanning on mobile
* Certificate verification (valid & invalid cases)
* Responsive layout testing
* Role‑based permission checks
* Performance verification

---

## 🚀 Local Setup (VS Code Friendly)

```bash
# Clone the repository
git clone https://github.com/your-username/civora-nexus-lms.git
cd civora-nexus-lms

# Create virtual environment
python -m venv venv

# Activate environment
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Apply migrations
python manage.py migrate

# Run development server
python manage.py runserver 0.0.0.0:8000
```

---

## 📈 Future Enhancements

* Analytics dashboard
* Email notifications
* Multiple certificate templates
* Dark mode
* Multi‑language support
* REST API integration

---

## 📌 Project Status

* **Status:** ✅ Complete & Production‑Ready
* **Version:** 2.0.0

---

## 👩‍💻 Author

**Harini G S**
Internship Project – Civora Nexus LMS

---

⭐ *If you find this project useful, consider giving it a star!*

