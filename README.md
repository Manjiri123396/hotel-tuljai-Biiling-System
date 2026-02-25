# hotel-tuljai-Biiling-System
A full-stack restaurant POS and billing system for Hotel Tuljai, featuring real-time table management, GST-compliant invoicing, and professional receipt generation using React, PHP, and MySQL.
Hotel Tuljai - Restaurant POS and Billing System
A professional, full-stack Point of Sale (POS) and Billing management application. This system is designed to streamline restaurant operations through real-time table management, dynamic order processing, and automated receipt generation.

Core Features
Management Dashboard: Centralized monitoring of total tables, active orders, and daily sales metrics.

Table Management Interface: Dedicated controls for assigning orders to specific tables or managing walk-in service types.

Professional Billing Engine:

Real-time itemized cart with quantity adjustment logic.

Automated GST calculation (5% toggle) with precision rounding.

Integrated Settle & Print workflow for synchronized database updates.

Menu and Search System: Searchable menu database categorized by service types (Starter, Main Course, Dessert, Beverage).

Database Integration: Permanent storage of sales reports and transaction history via MySQL.

Technical Stack
Frontend: React.js with Lucide-React icons and Axios for HTTP requests.

Backend: PHP REST API.

Database: MySQL for menu data and transaction storage.

Styling: Custom CSS3 focusing on professional restaurant aesthetics and responsive layouts.

Installation and Deployment
1. Frontend Configuration
Ensure that Node.js is installed on the local environment.

Navigate to the project root directory.

Execute npm install to install required dependencies.

Execute npm start to initialize the development server.

2. Backend Configuration
The system requires a local server environment (XAMPP, WAMP, or Apache).

Move the HOTEL-API folder into the server's root directory (e.g., /htdocs or /www).

Ensure the PHP scripts are accessible via the endpoint http://localhost/HOTEL-API/.

3. Database Setup
Access phpMyAdmin or a MySQL client.

Create a database named hotel_tuljai.

Import the provided SQL schema to generate the menu and sales tables.

Project Structure
/src/Billing.js: Contains the logic for the billing cart, GST calculations, and receipt generation.

/src/Billing.css: Defines the typography, professional table layouts, and receipt print styles.

/HOTEL-API/: Contains the PHP backend logic for database communication.

Operational Workflow
Order Creation: Select a table or walk-in service.

Item Selection: Add items from the searchable menu to the order summary.

Bill Generation: Review the summary, apply GST if required, and generate the receipt UI.

Settlement: Print the bill and settle the transaction, which automatically saves the record to the sales database and resets the table status.
