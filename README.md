# Onboarding & Dashboard Application

A full-stack web application featuring a multi-step onboarding wizard and user dashboard.

---

## Features

### Frontend

- Multi-step onboarding wizard (3 steps):
  - Personal Info (Name, Email)
  - Business Info (Company Name, Industry, Size)
  - Preferences (Theme, Dashboard Layout)
- Progress bar and navigation buttons (Next, Back, Submit)
- Input validation for required fields
- Responsive UI with smooth transitions
- Dashboard with user info and cards for:
  - Team Members Count
  - Active Projects
  - Notifications
- Optional chart visualization (e.g., with Recharts)
- Data persistence via localStorage or API

### Backend (Django REST Framework)

- User Authentication with JWT:
  - Register (`POST /api/register/`)
  - Login (`POST /api/login/`)
  - Protected profile routes (`GET /api/profile/`, `PATCH /api/profile/`)
- Preferences API (`POST /api/preferences/`, `GET /api/preferences/`)
- Dashboard summary endpoint (`GET /api/dashboard-summary/`) returning dummy data
- Input validation via DRF serializers
- Secure routes protected with JWT
- Configurable with environment variables (`.env`)

---

## Tech Stack

- Backend: Python, Django, Django REST Framework, SimpleJWT
- Frontend: React, Tailwind CSS (or plain CSS), Axios
- Database: SQLite (default), PostgreSQL (optional)
- Authentication: JWT

---

## Getting Started

### Backend Setup

1. Clone the repo:

```bash
git clone https://github.com/yourusername/onboarding-dashboard.git
cd onboarding-dashboard/backend
# auth_dashboard_full
