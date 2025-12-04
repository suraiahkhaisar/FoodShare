# 🍽️ FoodShare  
*A Flask + MongoDB powered food donation platform*

FoodShare is a web application that connects food donors (individuals, restaurants, organizations) with recipients (NGOs, shelters, and people in need).  
It supports multiple user roles, donation tracking, location-based matching, and notifications.

---

## 🌟 Features

- 🔐 **Authentication & Role-Based Access**
  - User registration & login (Flask sessions)
  - Roles: **Donor, Recipient, Inspector, Admin, Super Admin**

- 🎁 **Food Donation Management**
  - Donors can create, edit, and manage food donations
  - Inspectors/Admins can review **pending** donations
  - Admins can **assign donations** to recipients
  - View and manage **recipients** and user profiles

- 📊 **Admin Dashboard**
  - Analytics view for donations and users
  - Manage **flagged users** and system activity

- 🔔 **Notification System**
  - In-app notifications for approvals, assignment, and status changes

- 📍 **Location Mapping**
  - Show donors and recipients on a map
  - Help match nearby donors and recipients
  - Useful for delivery planning and pickup routes


- 📷 **Image Uploads**
  - Attach images for donation items (e.g., food pictures)
  - Store and display uploaded images in the UI

---

## 🧱 Tech Stack

| Category     | Technology              |
|-------------|-------------------------|
| Backend     | Flask (Python)          |
| Database    | MongoDB                 |
| Frontend    | HTML, CSS, (Bootstrap if used) |
| Auth        | Flask sessions / custom auth |
| Mapping     | Map API (e.g., Google Maps / similar) |
| File Uploads | Flask file upload handling |
| Environment | Python 3.x              |

> The exact Python packages are listed in `requirements.txt`.

---

## 📁 Project Structure

```bash
FOOD/
├── app.py                # Main Flask app entry point
├── requirements.txt      # Python package dependencies
├── .env.example          # Example environment variables
├── README.md             # Project documentation
├── static/               # CSS, JS, images, uploaded files (if configured here)
├── templates/
│   ├── base.html
│   ├── index.html
│   ├── notifications.html
│   ├── auth/
│   │   ├── login.html
│   │   └── register.html
│   ├── admin/
│   │   ├── analytics.html
│   │   ├── assign_donations.html
│   │   ├── flagged_users.html
│   │   ├── pending.html
│   │   ├── profile.html
│   │   └── recipients.html
│   ├── donor/           # Donor-specific pages
│   ├── inspector/       # Inspector views
│   ├── recipient/       # Recipient views
│   └── superadmin/      # Super admin views
└── utils/               # Helper modules (DB, auth, notifications, etc.)

---
## ▶️ Run the Application

Once everything is set up, run the following command from the project root:

```bash
python app.py
