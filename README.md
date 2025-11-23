# 🚚 Pause Regal – Vendor Rider App

Pause Regal – Vendor Rider App is the official delivery application used by riders to receive, manage, and deliver customer orders efficiently.  
This app is part of the Pause Regal ecosystem, supporting a smooth end-to-end food ordering and delivery workflow for a single vendor.

## 🧩 Pause Regal Ecosystem

The complete Pause Regal solution contains:

### 🛠️ Vendor Admin Dashboard
Where the vendor manages:
- Menu items
- Orders
- Delivery assignments
- Working hours
- Payments & settings

### 🍽️ Customer App
- Customers browse dishes, place orders, select delivery addresses, and pay online.

### 🚚 Delivery Rider App (this repository)
- Riders receive orders, navigate to customers, and update delivery status in real time.

## 🚀 Features – Rider App

### 📦 Order Management
- Receive new delivery tasks immediately
- View order details (customer info, items, total, notes)
- Accept or decline delivery tasks

### 🗺️ Navigation
- Integrated Google Maps
- Step-by-step navigation to vendor location and customer address
- Real-time location tracking

### 🔔 Status Updates
Update order status:
- On the way to vendor
- Picked up
- Out for delivery
- Delivered  

Vendor and customer receive real-time notifications.

### 👤 Rider Profile
- Manage account information
- View delivery history
- Check performance and statistics (depending on backend)

## 🏗️ Tech Stack
- Flutter (Dart)
- Firebase (push notifications, API keys, analytics depending on your setup)
- REST API for all backend communication
- Google Maps SDK
- Location & background tracking

## 📥 Installation & Setup

### 1️⃣ Clone the repository
```bash
git clone https://github.com/aimaad/Pause-Regal-Vender-Rider-App
cd Pause-Regal-Vender-Rider-App
```
## 2️⃣ Move Files to Your Web Server

**XAMPP :** place the project in `htdocs/`  
**WAMP :** place the project in `www/`

Start **Apache** and **MySQL**

---

## 🗄️ Database Setup (Using Provided SQL)

The repository includes a SQL dump for all required tables.

### 1️⃣ Create a Database

Open **phpMyAdmin** and create a new database:
pause_regal


### 2️⃣ Import the SQL File

- Select the database  
- Click **Import**  
- Upload: `/database/pause_regal.sql`  
- Click **Go**

✅ This will create all tables, default groups (admin / members / rider), languages, branches, menu items, orders, carts, notifications, live tracking, API keys, and more.

---

### 🔧 Configuration

Edit the database configuration file:

application/config/database.php
```bash

```php
'hostname' => 'localhost',
'username' => 'root',
'password' => '',
'database' => 'pause_regal',
```
## ▶️ Access the Dashboard

Open your browser:
```bash
http://localhost/Pause-Regal/
```

Login with the admin account created during installation or with the default credentials provided in the SQL file.
