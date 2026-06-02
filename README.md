# 🏨 GRAND HOTEL Management Suite

A professional, desktop-based **Hotel Management System** designed to streamline daily hotel operations, manage guest check-ins, automate billing mechanics, and provide real-time financial tracking. Built entirely with **Python**, utilizing an object-oriented graphical user interface via **Tkinter**, and powered by a local **SQLite database**.

<p align="left">
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python" alt="Python">
  <img src="https://img.shields.io/badge/SQLite-Database-003B57?style=for-the-badge&logo=sqlite" alt="SQLite">
  <img src="https://img.shields.io/badge/GUI-Tkinter-gray?style=for-the-badge" alt="Tkinter">
</p>

---

## 👥 Group Members
* **Adarsh Sharma**
* **Anuvanshika**
* **Chaitanay Parkash**
* **Janani**

*Course Project: Python Programming (BTECH CSE Batch 66)*

---

## 🎯 Key Objectives
* **Automate Manual Work:** Replace physical registers and minimize errors with manual hotel operations.
* **Dynamic Inventory Control:** Keep track of room availability dynamically (Available, Occupied).
* **Smart Tiered Pricing:** Automated stay and bill calculations adjusting dynamically for daily, weekly, and monthly rates.
* **Financial Tracking:** Centralized ledger for tracking incoming revenue alongside operational expenses.

---

## 🖥️ System Modules & Features

### 1. Dashboard UI
* Live dynamic statistics detailing **Available Rooms**, **Occupied Rooms**, **Active Bookings**, and **Total Revenue**.
* Display stream tracking real-time recent guest arrivals.

### 2. Room Management
* Inventory controls to add new rooms with targeted pricing.
* Global bulk-pricing updater that shifts base fees across specific room variants (`Single`, `Double`, `Suite`, `Deluxe`) simultaneously.

### 3. Smart POS Booking Engine
* Direct phone-number lookups that automatically fetch returning customer data.
* Built-in checkout dates and dynamic bill estimators.
* Integrated payment selector fields handling `Cash`, `Debit Card`, and automated `Credit Card` profile links.

### 4. Automated Billing & Invoicing
* Comprehensive layout displaying breakdown math including room charges, meal plans (`BB`, `HB`, `FB`), and a fixed 12% operational tax.
* Double-click integration connecting the bills table directly to invoice generators for instant print readouts.

### 5. Housekeeping Tracker
* Tri-color visual warning grid designating real-time room cleanliness states (`Clean`, `Dirty`, or `Service Requested`).

### 6. Finance & Analytics
* Analytical comparison ledger tracking monthly growth margins.
* Quick operational expense recorders for logged outflows (e.g., *Laundry, Electricity, Salaries*) against net margins.

---

## 🛠️ Technology Stack & Architecture
* **Core Logic & Application Flow:** Python 3.x (Modular, Object-Oriented Layout using OOP Concepts).
* **Frontend GUI Components:** Tkinter & custom styled `ttk` widgets (buttons, forms, tables) using a dark-mode theme matrix.
* **Database Engine:** SQLite (Relational database management system featuring cascading data tables).
* **Date Handling:** Datetime Module for check-in and check-out management.

### 🗄️ Database Table Relationships
```text
  ┌───────────────┐          ┌───────────────┐
  │   CUSTOMERS   │          │     ROOMS     │
  ├───────────────┤          ├───────────────┤
  │ PK  cust_id   │          │ PK  room_no   │
  │     name      │          │     room_type │
  │     phone     │          │     price     │
  │     country   │          │     status    │
  │     meal_plan │          │     hk_status │
  └───────┬───────┘          └───────┬───────┘
          │                          │       
          └───────────┐  ┌───────────┘       
                     ▼  ▼                    
             ┌───────────────┐               
             │   BOOKINGS    │               
             ├───────────────┤               
             │ PK  booking_id│               
             │ FK  cust_id   │               
             │ FK  room_no   │               
             │     check_in  │               
             │     check_out │               
             │     status    │               
             └───────┬───────┘               
                     │                       
                     ▼                       
             ┌───────────────┐       ┌───────────────┐
             │     BILLS     │       │   EXPENSES    │
             ├───────────────┤       ├───────────────┤
             │ PK  bill_id   │       │ PK  expense_id│
             │ FK  booking_id│       │     category  │
             │     total_amt │       │     amount    │
             │     paid      │       │     exp_date  │
             │     pay_date  │       └───────────────┘
             └───────────────┘
