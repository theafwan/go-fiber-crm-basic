# Go-fiber-crm-basic

This is a basic CRM (Customer Relationship Management) system implemented using Go programming language and the Fiber web framework. The project demonstrates simple operations such as getting all leads, getting a lead by ID, adding a new lead, and deleting a lead by ID.

## Prerequisites

- Go should be installed on your system.
- GCC (MinGW) should be installed and added to the PATH.
- SQLite3 should be installed.

## Setup

1. Clone the repository:

```bash
git clone https://github.com/yourusername/Go-fiber-crm-basic.git
```

2. Navigate to the project directory:

```bash
cd Go-fiber-crm-basic
```

3. Install the dependencies:

```bash
go mod tidy
```

4. Install GCC:
   Download and install the MinGW package from https://mingw-w64.org/doku.php/download

5. Set CGO_ENABLED environment variable to 1:

In Windows PowerShell:

```bash
$env:CGO_ENABLED=1
```

## Running the Program

### Build the application:

```bash
go build main.go
```

### Run the main application:

```bash
go run main.go
```

The application will start and listen on port 3000.

## Usage

You can access the following endpoints:

- Get all leads: http://localhost:3000/api/v1/lead
- Get lead by ID: http://localhost:3000/api/v1/lead/:id
- Add new lead: http://localhost:3000/api/v1/lead
- Delete lead by ID: http://localhost:3000/api/v1/lead/:id

## Database

The application uses an SQLite database to store leads. The leads.db file will be created in the project directory.

## Project Structure

main.go: Entry point of the application. Sets up the Fiber app and initializes the database.
lead/lead.go: Defines the Lead model and the CRUD operations for leads.
database/database.go: Manages the database connection.

## Acknowledgements

This project is built using Go, Fiber web framework, and Gorm ORM.

License
This project is licensed under the MIT License - see the LICENSE file for details.
