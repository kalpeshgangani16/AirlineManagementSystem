# ✈️ Airline Management System

A web-based flight booking system built using **Django**. This platform enables users to **search, book flights**, make payments, and access tickets. Admins can manage flights, users, and bookings through a secure admin panel.

---

## ✅ Features

- 🔐 User authentication (Signup, Login, Logout)
- 🧾 Booking confirmation and ticket viewing
- 🛫 Flight search and booking system
- 👥 Passenger profile management
- 💳 Payment processing simulation
- ⚙️ Admin panel for managing data
- 📦 SQLite3 backend database

---

## 🧠 Functional Overview

| URL | Description |
|-----|-------------|
| `/` | Homepage |
| `/login/` | User login |
| `/logout/` | User logout |
| `/signup/` | User registration |
| `/profile/` | Update user profile |
| `/search/` | Search available flights |
| `/booking/<int:flight_id>/` | Create booking for selected flight |
| `/booking/confirmation/` | Booking confirmation page |
| `/ticket/<int:pk>/` | View ticket (class-based view) |
| `/ticket/view/<int:booking_id>/` | View ticket by booking ID |
| `/payment/<int:booking_id>/` | Payment page |
| `/payment/success/<int:booking_id>/` | Payment success confirmation |
| `/admin/` | Django admin panel |

---

## 📁 Project Structure

```text
flight_booking/
├── flight_booking/       # Django project settings
├── app/                  # Core app for flights, bookings, payments
├── templates/            # HTML templates (Bootstrap-based)
├── static/               # Static files (CSS, JS, images)
├── db.sqlite3            # SQLite database
├── manage.py             # Django management script
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation

```

---

## ⚙️ Installation & Setup

### 1. 📥 Clone the Repository

```bash
git clone https://github.com/yourname/YourRepo.git
cd YourRepo
```

### 2. 🧪 Create a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
```

### 3. 📦 Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. 🔄 Apply Migrations

```bash
python manage.py migrate
```

### 5. 👤 Create Superuser

```bash
python manage.py createsuperuser
```

### 6. 🚀 Run the Development Server

```bash
python manage.py runserver
```

### 🔗 Visit the App

[http://127.0.0.1:8000](http://127.0.0.1:8000)

---

## 🔐 Security
- 🔒 User passwords are securely hashed using Django's built-in authentication system
- ✅ Authentication required for booking, payment, and ticket viewing
- 🔐 Admin panel protected with superuser access only

---

## 🙏 Thank You
- Thank you for exploring the Airline Management System! Your feedback, suggestions, and contributions are always welcome. ✈️
