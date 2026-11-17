# Logistics Tracker Dashboard – Laravel

A web-based dashboard for managing logistics operations, live location tracking, trips, orders, drivers, and customers. Designed to work with the companion Android mobile app.

---

## Overview

**Logistics Tracker Dashboard** provides administrators and managers with a centralized view of logistics activities:

- Monitor live driver locations and daily trails on maps
- Manage trips and orders
- Administer users (admins, drivers, and customers)
- View historical location data

The system pairs with the **Logistics Tracker Android App**, which drivers use in the field to create trips, add stopovers, and send real-time GPS updates.

---

## Key Features

### Live Tracking
- Real-time current location view
- Live trail visualization
- Daily trails for specific drivers and dates
- Historical location logs

### Trip & Order Management
- Create, edit, and delete trips
- View all trips and orders
- Customer-specific trip and order handling
- Trip distance calculations

### User Management
- **Admins** – full system access
- **Drivers** – field agents who use the mobile app
- **Customers** – associated with trips and orders
- Full CRUD operations for all user types

### Authentication
- Login / Logout
- User registration (signup)
- Laravel Sanctum for API authentication (used by the Android app)

---

## Tech Stack

| Layer       | Technology              |
|-------------|-------------------------|
| Backend     | PHP 8.1+ · Laravel 10   |
| Auth        | Laravel Sanctum         |
| Database    | MySQL / MariaDB         |
| Frontend    | Blade templates         |

---

## Installation

### Prerequisites
- PHP ≥ 8.1
- Composer
- MySQL / MariaDB

### Setup Steps

```bash
# 1. Clone the repository
git clone https://github.com/JavisOtieno/Logistics-Tracker-Dashboard-Web-App-Laravel-Based.git
cd Logistics-Tracker-Dashboard-Web-App-Laravel-Based

# 2. Install PHP dependencies
composer install

# 3. Copy environment file
cp .env.example .env

# 4. Generate application key
php artisan key:generate

# 5. Configure your database in .env
# DB_CONNECTION=mysql
# DB_HOST=127.0.0.1
# DB_PORT=3306
# DB_DATABASE=logistics
# DB_USERNAME=root
# DB_PASSWORD=

# 6. Run migrations
php artisan migrate

# 7. (Optional) Seed the database if seeders exist
# php artisan db:seed

# 8. Start the development server
php artisan serve
