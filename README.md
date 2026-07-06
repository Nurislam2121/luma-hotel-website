# Luma — Hotel Booking Platform

A full-stack web application designed for a hotel booking system. Built using Python and the Django framework, the platform offers potential guests a seamless experience from browsing rooms to managing active bookings, alongside an automated system validation process.

## 🚀 Key Features

The application comprises 9 fully integrated pages with distinct functionalities:

1. **Authentication System (Login & Registration)**:
   - Secure authorization.
   - Robust sign-up validation enforcing strict security policies (passwords must be $\ge 8$ characters, distinct from username/email, and checked against common compromised password lists).
2. **Home Page**: Includes overview statistics, interactive customer reviews, service advantages, business contacts, an integrated map location, and a quick-booking modal shortcut.
3. **Booking Panel**: A multi-parameter reservation interface where guests select check-in/check-out dates, room types (4 configurations available), automatic or precise room distribution, number of guests, and special requests.
4. **Rooms & Rates**: A structured catalog displaying hotel room categories, precise price brackets, and entry points for reservation or detailed overviews.
5. **Detailed Room Overview**: Individual product pages equipped with custom dynamic media galleries tailored to the selected room type.
6. **Reviews Hub**: An interactive platform for logged-in users to submit ratings and written feedback regarding their stay.
7. **Contact & Feedback**: Includes physical location details alongside a backend-powered contact form that dispatches user messages straight to the hotel's operational email.
8. **My Bookings Dashboard**: A personalized user dashboard showing complete reservation history, live tracking statuses, and an option to request booking cancellations.

## 🛠 Tech Stack

**Frontend:**
- HTML5 / CSS3
- Vanilla JavaScript (Modal triggers, calendar date restrictions)

**Backend & Core:**
- Python
- Django Web Framework (Forms, Templates, Admin Contrib)
- SQLite3 (Default relational database engine)

## 📁 Project Structure

```text
├── booking/             # Core application logic (Models, Views, Forms)
│   ├── management/      # Custom management commands
│   ├── migrations/      # Database schema evolution track
│   ├── static/          # App-specific stylesheets and client scripts
│   └── templates/       # Component-based HTML views
├── hotel/               # Project configuration root (settings.py, urls.py)
├── media/               # Dynamic uploads directory
│   ├── room_images/     # Photo assets per explicit room units
│   └── room_type_images/# Base galleries for category overviews
├── myvenv/              # Isolated Python virtual environment
├── db.sqlite3           # Local SQLite database file
├── manage.py            # Django administrative command-line utility
└── requirements.txt     # Locked production dependencies

```
## 🔧 Local Setup & Installation
Note: Ensure you have Python installed on your operating system before initialization.

### 1. Environment Activation & Dependencies
```bash
# Navigate to the hotel project directory
cd site_hotel_code

# Activate your virtual environment
# On Windows:
myvenv\Scripts\activate
# On macOS/Linux:
source myvenv/bin/activate

# Install required dependencies
pip install -r requirements.txt
```
### 2. Database Synchronization
```bash
# Apply development migrations
python manage.py migrate
```
### 3. Running the Server
```bash
# Boot up the local development web server
python manage.py runserver
```
Once executed successfully, access the dashboard and web layout at http://127.0.0.1:8000/.
