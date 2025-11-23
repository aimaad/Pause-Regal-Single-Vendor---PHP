🖥️ Pause Regal – Single Vendor Dashboard (Admin Panel)

Pause Regal – Single Vendor Dashboard is the administration panel for the Pause Regal ecosystem.
It allows the vendor to manage menu items, orders, delivery workflow, vendor settings, and analytics.

This project is built using PHP, JavaScript, CSS, and includes a full database SQL dump for easy setup.

🧩 Pause Regal Ecosystem

The complete Pause Regal system includes:

🍽️ Customer App – browse meals, place orders, set delivery addresses, and pay online.

🚚 Rider App – receive delivery tasks, navigate routes, and update delivery status.

🖥️ Vendor Dashboard (this repository) – manage restaurant operations, menu, orders, riders, and settings.

🚀 Key Features
📦 Order Management

View real-time customer orders

Update order status: pending → processing → completed

Assign orders to riders

🍽️ Menu & Category Management

Add, update, delete meals

Set prices, images, descriptions, and availability

Manage categories and subcategories

🧑‍🍳 Vendor Settings

Update restaurant details

Manage branch hours

Configure delivery fees

📊 Reports & Analytics

Sales reports

Order history

Best-selling items

👥 Rider Management

Add/edit riders

Assign orders

Track rider performance

⚙️ API Integration

The dashboard exposes APIs used by:

Customer App

Rider App

API documentation files included in the repo:

api-doc.txt

rider-api-doc.txt

🏗️ Tech Stack

PHP – backend logic

MySQL / MariaDB – database

JavaScript / CSS / HTML – frontend

Apache / Nginx support with .htaccess

Custom MVC-style structure (application/ + system/)

Built-in installer for database and configuration

📥 Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/aimaad/Pause-Regal-Single-Vendor---PHP.git
cd Pause-Regal-Single-Vendor---PHP

2️⃣ Move Files to Your Web Server

XAMPP: place the project in htdocs/

WAMP: place the project in www/

Start Apache and MySQL

🗄️ Database Setup (Using Provided SQL)

The repository includes a SQL dump for all required tables.

1️⃣ Create a Database

Open phpMyAdmin and create a new database:

pause_regal

2️⃣ Import the SQL File

Select the database.

Click Import.

Upload the SQL file included in /database/pause_regal.sql.

Click Go.

✅ This will create all tables, default groups (admin / members / rider), languages, branches, menu items, orders, carts, notifications, live tracking, API keys, and more.

🔧 Configuration

Edit the database configuration in:

application/config/database.php


Set your database credentials:

'hostname' => 'localhost',
'username' => 'root',
'password' => '',
'database' => 'pause_regal',

▶️ Access the Dashboard

Open your browser and go to:

http://localhost/Pause-Regal/


Login with the admin account created during installation or via the default credentials in the SQL file if any.

📁 Project Structure
/
├── application/       → Main application logic (controllers, models, views)
├── system/            → Core system files
├── assets/            → CSS, JS, images
├── install/           → Installation wizard
├── database/          → SQL dump file
├── uploads/           → Uploaded images and media
├── index.php          → Application entry point
└── .htaccess          → URL rewriting and access control
