### Importing Database Using phpMyAdmin

To set up the database with phpMyAdmin:

1. Open WAMP server and go to `http://localhost/phpmyadmin` in your browser.
2. Log in with your MySQL credentials.
3. Create a new database (e.g., `ev_charging`).
4. Select the new database, then click on the "Import" tab.
5. Choose the `database/ev_charging.sql` file and click "Go" to import.
6. The tables and data will be loaded into your database.

Update your Python application's database connection settings to use this database.
### Accessing the Application

If you run the Python application (e.g., using Flask), the default port is usually `5000`. Access the app in your browser at:

```
http://localhost:5000
```

If you use WAMP server for hosting static files or PHP, access via:

```
http://localhost/ev_charging
```

Make sure to use the correct port and URL based on your setup.
# EV Charging Station Management System

This project is a web-based application for managing electric vehicle (EV) charging stations. It provides features for users, station administrators, and system admins to interact with charging stations, book slots, make payments, and view reports.

## Features

- User registration and login
- Admin and station login
- EV charging slot booking
- Payment processing
- Charging history and reports
- Interactive map for station locations
- Tariff management
- OTP verification for secure actions

## Project Structure

```
main.py                # Main application entry point
static/                # Static files (CSS, JS, images, fonts)
  ├── css/             # Stylesheets
  ├── js/              # JavaScript files
  ├── images/          # Image assets
  ├── fonts/           # Font files
  └── scss/            # SCSS source files
templates/             # HTML templates for all pages
  ├── admin.html
  ├── blog.html
  ├── book.html
  ├── ...
database/
  └── ev_charging.sql  # Database schema and data
```

## Getting Started

### Prerequisites

- Python 3.x
- Required Python packages (see below)

### Hosting on Localhost (WAMP Server)

To host this application on localhost, you need to install and configure WAMP server:

1. Download and install WAMP server from [https://www.wampserver.com/](https://www.wampserver.com/).
2. Start WAMP server and ensure Apache and MySQL services are running.
3. Place your project folder (`ev_charging`) inside the `www` directory of WAMP (usually `C:/wamp64/www/`).
4. Import the `ev_charging.sql` file into your MySQL database using phpMyAdmin or MySQL command line.
5. Update your database connection settings in your Python code to match WAMP's MySQL configuration (host, user, password, database name).
6. Access the application in your browser at `http://localhost/ev_charging`.

> **Note:** WAMP server is required for local hosting and database management. Make sure your Python application connects to the MySQL database provided by WAMP.

### Installation

1. Clone the repository:
   ```
   git clone https://github.com/Jebastin215/ev_charging.git
   ```
2. Navigate to the project directory:
   ```
   cd ev_charging
   ```
3. Install required packages:
   ```
   pip install -r requirements.txt
   ```
4. Set up the database using `database/ev_charging.sql`.

### Running the Application

Run the main application:

```
python main.py
```

### Folder Details

- **static/**: Contains all static assets (CSS, JS, images, fonts, SCSS).
- **templates/**: Contains all HTML templates for user, admin, and station interfaces.
- **database/**: Contains the SQL file for database setup.
- **main.py**: Main Python file to start the web server.

## Usage

- Register as a user or station admin.
- Log in to access booking, payment, and management features.
- Admins can view reports and manage stations.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Author

- [Jebastin215](https://github.com/Jebastin215)
