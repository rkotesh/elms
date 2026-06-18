# 🏫 Employee Leave Management System (ELMS) – Flask Application

[🚀 Live Demo on Render]([https://elms-3.onrender.com](https://elms-one.vercel.app/))

---

## 📌 Project Overview
The **Employee Leave Management System (ELMS)** is a secure, role-based web application developed using **Flask**.  
It allows employees to apply for leave, managers to review and approve/reject requests, and administrators to manage users and generate reports.  

This system improves leave tracking, enhances transparency, and provides admin-level insights with dashboards and reporting tools.

---

## 🎯 Objectives
- ✅ Provide a **role-based leave management platform** for organizations  
- ✅ Enable **real-time status updates** for employees on their leave applications  
- ✅ Allow managers to **approve, reject, or filter requests** based on date, employee, or status  
- ✅ Give administrators a **central dashboard** with analytics and reporting capabilities  
- ✅ Maintain **audit logs** of all key actions for accountability  
- ✅ Deploy seamlessly on **cloud platforms** such as Render  

---

## 🚀 Key Features

### 🔐 Authentication & Authorization
- Secure login & registration (Flask-Login)  
- Role-based access: **Admin, Manager, Employee**  

### 👨‍💼 Employee Management
- Add, update, and delete employee profiles  
- Manage departments and roles  

### 📅 Leave Management
- Employees: Apply, edit, or cancel leave requests  
- Managers: Approve / reject leave requests  
- Track leave history and status  

### 📊 Dashboard & Reporting
- Admin dashboard with **leave statistics**  
- Generate **PDF/CSV reports** using WeasyPrint & Pandas  
- Filter by date, employee, or team  

### 📧 Email Notifications
- Leave status updates via **Flask-Mail**  
- Configurable SMTP support  

### 🔒 Security
- Password hashing (Werkzeug)  
- CSRF protection (Flask-WTF)  
- Audit logs for user actions  

---

## 🛠️ Tech Stack
- **Backend:** Python, Flask  
- **Frontend:** HTML, CSS, Bootstrap, Jinja2  
- **Database:** SQLite (development), PostgreSQL (production)  
- **Authentication:** Flask-Login  
- **Email Service:** Flask-Mail  
- **Reports:** WeasyPrint, Pandas  
- **Deployment:** Render  

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/elms.git
cd elms
2️⃣ Create Virtual Environment & Install Dependencies
bash
Copy code
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
pip install -r requirements.txt
3️⃣ Configure Environment Variables
Create a .env file in the root directory:

env
Copy code
FLASK_APP=run.py
FLASK_ENV=development
SECRET_KEY=your_secret_key

SQLALCHEMY_DATABASE_URI=sqlite:///elms.db

MAIL_SERVER=smtp.gmail.com
MAIL_PORT=587
MAIL_USE_TLS=True
MAIL_USERNAME=your_email@gmail.com
MAIL_PASSWORD=your_password
4️⃣ Run Database Migrations
bash
Copy code
flask db init
flask db migrate -m "Initial migration"
flask db upgrade
5️⃣ Start the Application
bash
Copy code
python run.py
App runs locally on: 👉 http://127.0.0.1:5000

🚀 Deployment (Render)
Push code to GitHub

Connect repo with Render

Set build command:

bash
Copy code
pip install -r requirements.txt
Set start command:

bash
Copy code
gunicorn app.main:app
Configure environment variables in Render Dashboard

Deploy 🎉

📑 Documentation Deliverables
✅ Project Summary & Architecture Diagram

✅ Technical Documentation (setup, features, module structure)

✅ User Guide (roles, features, workflows)

✅ Future Enhancements (e.g., mobile support, role hierarchy, advanced analytics)

✅ Presentation (PPT) for final submission

👨‍💻 Author
S. Koteswararao
📧 srkotesh23@gmail.com
💼 LinkedIn - www.linkedin.com/in/sankula-koteswararao
🌐 Portfolio - https://rkotesh.github.io/kotesh-portfolio/
