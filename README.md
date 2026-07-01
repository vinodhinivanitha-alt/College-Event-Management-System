# 🎓 College Event Management System

A web-based **College Event Management System** developed using **Python (Flask)** and **SQLite/MySQL**. This application allows administrators to create and manage college events while students can register, make payments, and provide feedback through a simple and attractive interface.

---

# 📌 Features

## 👨‍💼 Admin
- Admin Login
- Create new events
- Add event category
- Set event date and time
- Add venue
- Set registration fee
- Add organizer name
- Add organizer contact
- AI-generated event instructions
- View all events
- View registrations
- View payment reports
- View feedback

---

## 👨‍🎓 Student
- Student Registration
- Student Login
- View available events
- Register for events
- Multiple event registration
- View AI-generated instructions
- Online Payment
- Spot Payment
- Submit Feedback
- Logout

---

# 🤖 AI Features

The system automatically generates event instructions based on the selected event category.

### Technical Events
- Carry your laptop.
- Coding must be original.
- Internet usage is allowed.
- Submit before deadline.
- Follow all rules.

### Cultural Events
- Wear proper costume.
- Be ready before performance.
- Respect other participants.
- Bring required props.
- Performance time is limited.

### Non-Technical Events
- Report 30 minutes early.
- Carry your College ID.
- Follow event rules.
- Maintain discipline.
- Judges' decision is final.

---

# 💳 Payment Module

Supports two payment methods:

- Online Payment
- Spot Payment

Payment Status:
- Paid
- Pending

---

# ⭐ Feedback Module

Students can submit:

- Rating (1–5)
- Comments

Admin can view all feedback.

---

# 📊 Reports

Admin can generate reports including:

- Total Events
- Total Registrations
- Payment Status
- Event Statistics

---

# 🗄 Database Tables

## User

| Field | Type |
|--------|------|
| user_id | Integer (PK) |
| name | String |
| email | String |
| password | String |
| role | String |

---

## Event

| Field | Type |
|--------|------|
| event_id | Integer (PK) |
| event_name | String |
| category | String |
| date | String |
| time | String |
| venue | String |
| description | Text |
| price | Float |
| organizer_name | String |
| organizer_contact | String |

---

## Instruction

| Field | Type |
|--------|------|
| instruction_id | Integer (PK) |
| event_id | Integer |
| text | Text |

---

## Registration

| Field | Type |
|--------|------|
| registration_id | Integer (PK) |
| user_id | Integer |
| event_id | Integer |
| registration_date | DateTime |

---

## Payment

| Field | Type |
|--------|------|
| payment_id | Integer (PK) |
| registration_id | Integer |
| amount | Float |
| payment_mode | String |
| payment_status | String |

---

## Feedback

| Field | Type |
|--------|------|
| feedback_id | Integer (PK) |
| user_id | Integer |
| event_id | Integer |
| rating | Integer |
| comments | Text |

---

# 🛠 Technologies Used

- Python 3
- Flask
- SQLAlchemy
- Flask Login
- SQLite / MySQL
- HTML
- CSS

---

# 📂 Project Structure

```
College_Event_Management/
│
├── app.py
├── requirements.txt
├── README.md
├── static/
│   ├── css/
│   ├── images/
│
├── templates/
│   ├── login.html
│   ├── signup.html
│   ├── dashboard.html
│   ├── events.html
│   ├── feedback.html
│
└── database.db
```

---

# ⚙ Installation

Clone the repository

```bash
git clone https://github.com/yourusername/College-Event-Management-System.git
```

Move into project folder

```bash
cd College-Event-Management-System
```

Install required packages

```bash
pip install flask
pip install flask_sqlalchemy
pip install flask_login
pip install pymysql
```

Run the application

```bash
python app.py
```

Open browser

```
http://127.0.0.1:5000
```

---

# 🔐 Login

## Admin

```
Email:
admin@gmail.com

Password:
admin123
```

## Student

Register a new account and login.

---

# 🚀 Future Enhancements

- Email Notifications
- QR Code Event Entry
- Certificate Generation
- Real AI Integration
- Online Payment Gateway (Razorpay/Stripe)
- Attendance Tracking
- Event Images Upload
- Dashboard Analytics
- PDF Report Generation
- Mobile Responsive UI

---

# 👩‍💻 Developed By

**Vinodhini Vanitha**

College Event Management System

Python • Flask • SQLite/MySQL • HTML • CSS

---

# 📄 License

This project is developed for educational and academic purposes.
