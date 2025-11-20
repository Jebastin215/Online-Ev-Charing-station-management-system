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
