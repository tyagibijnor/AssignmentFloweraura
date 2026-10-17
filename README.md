# Floweraura

A lightweight PHP project built with CodeIgniter for displaying and exporting MySQL table data. The application loads records from the `tbltest` table, renders them in a responsive HTML table, and includes a basic CSV export button and JavaScript progress bar UI.

## Project Overview

This repository is a small CodeIgniter assignment that demonstrates:

- MySQL database connectivity
- Data retrieval through a model
- HTML table rendering in a CodeIgniter view
- CSV export from the browser
- Progress indicator for export actions

The main flow is:

- `application/controllers/Exportdata.php` loads the model and fetches data
- `application/models/exportdata_model.php` queries the `tbltest` table
- `application/views/home.php` displays the table and export controls

## Tech Stack

- PHP
- CodeIgniter
- MySQL / MariaDB
- HTML, CSS, JavaScript

## Requirements

- PHP 5.3.7+ (or a compatible PHP version for your environment)
- Apache or Nginx web server
- MySQL / MariaDB database server

## Setup Instructions

1. Clone the project to your local web server directory.
2. Import the database schema and sample data from `db.sql` into MySQL.
3. Update database credentials in `application/config/database.php` if needed:
   - hostname
   - username
   - password
   - database name
4. Set your base URL in `application/config/config.php` if required by your local environment.
5. Start the project in your browser, usually at:

   `http://localhost/AssignmentFloweraura/`

   or directly via the exported controller route:

   `http://localhost/AssignmentFloweraura/index.php/exportdata`

## Database Notes

The project is configured to use a database named `navneet` by default and queries a table named `tbltest`.

You can change the query limit in `application/models/exportdata_model.php` if needed:

```php
$this->db->limit(500);
```

## Author

Navneet Tyagi

## Contact

For project-related queries, you can reach the author at:

- tyagibijnor@gmail.com
