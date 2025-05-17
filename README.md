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
├── templates/       # HTML templates (Bootstrap-based)
├── views.py         # View logic
├── urls.py          # URL routing
├── models.py        # Models for Flights, Bookings, Users
├── forms.py         # Forms for registration, profile, booking
├── static/          # Static files (CSS, JS)
├── admin.py         # Admin configuration
└── migrations/      # Django migrations

manage.py            # Django management script
db.sqlite3           # SQLite database
requirements.txt     # Python dependencies

---

# 1. Clone the Repository
git clone https://github.com/yourname/YourRepo.git
cd YourRepo

# 2. Create a Virtual Environment
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate

# 3. Install Dependencies
pip install -r requirements.txt

# 4. Apply Migrations
python manage.py migrate

# 5. Create Superuser
python manage.py createsuperuser

# 6. Run the Development Server
python manage.py runserver

# Visit the app at:
http://127.0.0.1:8000

