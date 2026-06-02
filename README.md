# Hotel_Management

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GRAND HOTEL Management Suite - README</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji";
            font-size: 16px;
            line-height: 1.5;
            word-wrap: break-word;
            color: #24292f;
            background-color: #ffffff;
            max-width: 1012px;
            margin: 0 auto;
            padding: 45px;
        }
        h1, h2, h3 {
            margin-top: 24px;
            margin-bottom: 16px;
            font-weight: 600;
            line-height: 1.25;
            padding-bottom: 0.3em;
            border-bottom: 1px solid #hsla(210,18%,87%,1);
        }
        h1 { font-size: 2em; }
        h2 { font-size: 1.5em; }
        h3 { font-size: 1.25em; }
        hr {
            height: 0.25em;
            padding: 0;
            margin: 24px 0;
            background-color: #d0d7de;
            border: 0;
        }
        code {
            padding: 0.2em 0.4em;
            margin: 0;
            font-size: 85%;
            background-color: rgba(175,184,193,0.2);
            border-radius: 6px;
            font-family: ui-monospace, SFMono-Regular, SF Mono, Menlo, Consolas, Liberation Mono, monospace;
        }
        pre {
            padding: 16px;
            overflow: auto;
            font-size: 85%;
            line-height: 1.45;
            background-color: #f6f8fa;
            border-radius: 6px;
            font-family: ui-monospace, SFMono-Regular, SF Mono, Menlo, Consolas, Liberation Mono, monospace;
        }
        pre code {
            padding: 0;
            margin: 0;
            font-size: 100%;
            background-color: transparent;
        }
        table {
            border-spacing: 0;
            border-collapse: collapse;
            margin-top: 0;
            margin-bottom: 16px;
            width: 100%;
        }
        table th, table td {
            padding: 6px 13px;
            border: 1px solid #d0d7de;
        }
        table tr {
            background-color: #ffffff;
            border-top: 1px solid #hsla(210,18%,87%,1);
        }
        table tr:nth-child(even) {
            background-color: #f6f8fa;
        }
        ul, ol {
            padding-left: 2em;
            margin-top: 0;
            margin-bottom: 16px;
        }
        li { margin-top: 0.25em; }
        .badge-container {
            margin-bottom: 16px;
        }
        .badge-container img {
            margin-right: 5px;
        }
    </style>
</head>
<body>

    <h1>🏨 GRAND HOTEL Management Suite</h1>

    [cite_start]<p>A professional, desktop-based <strong>Hotel Management System</strong> designed to streamline daily hotel operations, manage guest check-ins, automate billing mechanics, and provide real-time financial tracking[cite: 1, 2, 13, 14, 21, 22]. [cite_start]Built entirely with <strong>Python</strong>, utilizing an object-oriented graphical user interface via <strong>Tkinter</strong>, and powered by a local <strong>SQLite database</strong>[cite: 8, 10, 45].</p>

    <div class="badge-container">
        <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python" alt="Python">
        <img src="https://img.shields.io/badge/SQLite-Database-003B57?style=for-the-badge&logo=sqlite" alt="SQLite">
        <img src="https://img.shields.io/badge/GUI-Tkinter-gray?style=for-the-badge" alt="Tkinter">
    </div>

    <hr>

    <h2>👥 Group Members</h2>
    <ul>
        [cite_start]<li><strong>Adarsh Sharma</strong> [cite: 4]</li>
        [cite_start]<li><strong>Anuvanshika</strong> [cite: 5]</li>
        [cite_start]<li><strong>Chaitanay Parkash</strong> [cite: 6]</li>
        [cite_start]<li><strong>Janani</strong> [cite: 7]</li>
    </ul>
    [cite_start]<p><em>Course Project: Python Programming (BTECH CSE Batch 66) [cite: 11, 12]</em></p>

    <hr>

    <h2>🎯 Key Objectives</h2>
    <ul>
        [cite_start]<li><strong>Automate Manual Work:</strong> Replace physical registers and minimize errors with manual hotel operations[cite: 14, 16].</li>
        [cite_start]<li><strong>Dynamic Inventory Control:</strong> Keep track of room availability dynamically (Available, Occupied)[cite: 17, 18].</li>
        <li><strong>Smart Tiered Pricing:</strong> Automated stay and bill calculations adjusting dynamically for daily, weekly, and monthly rates.</li>
        [cite_start]<li><strong>Financial Tracking:</strong> Centralized ledger for tracking incoming revenue alongside operational expenses[cite: 22].</li>
    </ul>

    <hr>

    <h2>🖥️ System Modules & Features</h2>

    <h3>1. Dashboard UI</h3>
    <ul>
        [cite_start]<li>Live dynamic statistics detailing <strong>Available Rooms</strong>, <strong>Occupied Rooms</strong>, <strong>Active Bookings</strong>, and <strong>Total Revenue</strong>[cite: 56, 63, 64, 65, 66].</li>
        [cite_start]<li>Display stream tracking real-time recent guest arrivals[cite: 67].</li>
    </ul>

    <h3>2. Room Management</h3>
    <ul>
        <li>Inventory controls to add new rooms with targeted pricing.</li>
        <li>Global bulk-pricing updater that shifts base fees across specific room variants (<code>Single</code>, <code>Double</code>, <code>Suite</code>, <code>Deluxe</code>) simultaneously.</li>
    </ul>

    <h3>3. Smart POS Booking Engine</h3>
    <ul>
        <li>Direct phone-number lookups that automatically fetch returning customer data.</li>
        <li>Built-in checkout dates and dynamic bill estimators.</li>
        <li>Integrated payment selector fields handling <code>Cash</code>, <code>Debit Card</code>, and automated <code>Credit Card</code> profile links.</li>
    </ul>

    <h3>4. Automated Billing & Invoicing</h3>
    <ul>
        <li>Comprehensive layout displaying breakdown math including room charges, meal plans (<code>BB</code>, <code>HB</code>, <code>FB</code>), and a fixed 12% operational tax.</li>
        [cite_start]<li>Double-click integration connecting the bills table directly to invoice generators for instant print readouts[cite: 77].</li>
    </ul>

    <h3>5. Housekeeping Tracker</h3>
    <ul>
        [cite_start]<li>Tri-color visual warning grid designating real-time room cleanliness states (<code>Clean</code>, <code>Dirty</code>, or <code>Service Requested</code>)[cite: 79].</li>
    </ul>

    <h3>6. Finance & Analytics</h3>
    <ul>
        [cite_start]<li>Analytical comparison ledger tracking monthly growth margins[cite: 81, 82].</li>
        [cite_start]<li>Quick operational expense recorders for logged outflows (e.g., <em>Laundry, Electricity, Salaries</em>) against net margins[cite: 81, 82].</li>
    </ul>

    <hr>

    <h2>🛠️ Technology Stack & Architecture</h2>
    <ul>
        [cite_start]<li><strong>Core Logic & Application Flow:</strong> Python 3.x (Modular, Object-Oriented Layout using OOP Concepts)[cite: 38, 45, 46].</li>
        [cite_start]<li><strong>Frontend GUI Components:</strong> Tkinter & custom styled <code>ttk</code> widgets (buttons, forms, tables) using a dark-mode theme matrix[cite: 37, 40, 41, 48].</li>
        [cite_start]<li><strong>Database Engine:</strong> SQLite (Relational database management system featuring cascading data tables)[cite: 34, 42].</li>
        [cite_start]<li><strong>Date Handling:</strong> Datetime Module for check-in and check-out management[cite: 36, 43, 44].</li>
    </ul>

    <h3>🗄️ Database Table Relationships</h3>
<pre>
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
</pre>

    <hr>

    <h2>⚡ Tiered Billing Logic Structure</h2>
    <p>The system bypasses plain scalar math, incorporating real-world hospitality bulk-stay logic directly inside the dynamic pricing functions:</p>

    <table>
        <thead>
            <tr>
                <th align="left">Room Type</th>
                <th align="left">Daily Rate</th>
                <th align="left">Weekly Bundle Rate</th>
                <th align="left">Monthly Bundle Rate (30+ Days)</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><strong>Single</strong></td>
                <td>₹350</td>
                <td>₹2,000</td>
                <td>₹8,000</td>
            </tr>
            <tr>
                <td><strong>Double</strong></td>
                <td>₹700</td>
                <td>₹3,500</td>
                <td>₹10,000</td>
            </tr>
            <tr>
                <td><strong>Suite</strong></td>
                <td>₹1,000</td>
                <td>₹6,000</td>
                <td>₹25,000</td>
            </tr>
        </tbody>
    </table>

    <hr>

    <h2>🚀 Installation & Running Local Builds</h2>

    <h3>Prerequisites</h3>
    <p>Make sure Python 3.x is configured in your system environment variables. [cite_start]No external pip libraries are required, as <code>sqlite3</code> and <code>tkinter</code> come packed directly with standard Python setups[cite: 34, 37].</p>

    <h3>Execution Steps</h3>
    <ol>
        <li>Clone the repository down to your computer terminal:
            <pre><code>git clone https://github.com/YOUR_USERNAME/Hotel-Management-System.git
cd Hotel-Management-System</code></pre>
        </li>
        <li>Run the main codebase to generate the initial schema tables and launch the GUI application:
            <pre><code>python Project.py</code></pre>
        </li>
    </ol>

    <hr>

    <h2>📦 Creating an Executable (.exe)</h2>
    [cite_start]<p>To bundle the application into a standalone production executable utility for desktop computers without requiring Python interpreters, run PyInstaller with the project parameters below[cite: 51]:</p>

    <pre><code>pyinstaller --noconsole --onefile --icon=hotel_icon.ico Project.py</code></pre>

    <h3>Parameter Breakdown:</h3>
    <ul>
        [cite_start]<li><code>--noconsole</code>: This prevents a black command prompt window from popping up when you open your app[cite: 52].</li>
        [cite_start]<li><code>--onefile</code>: This packs everything into a single .exe file workspace[cite: 53].</li>
        [cite_start]<li><code>--icon</code>: If you have an .ico file, this will set the app's logo on the desktop[cite: 54].</li>
    </ul>

</body>
</html>

