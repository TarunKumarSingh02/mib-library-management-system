# M.I.B. Library Management System

A modern library management web application built using **ASP.NET Core MVC, .NET 8, Entity Framework Core, ASP.NET Core Identity, and SQL Server**.

The project features an M.I.B.-inspired mission-control interface for managing books, publications, students, librarians, and borrowing transactions.

## Features

- **Dashboard:** Overview of library statistics, active borrowings, overdue alerts, and recent transactions.
- **Book Management:** Add, update, search, and manage book inventory.
- **Publication Management:** Manage newspapers, magazines, and other publications.
- **Student Directory:** Maintain student records and account information.
- **Librarian Management:** Manage librarian records.
- **Borrowing and Returns:** Track issued books, due dates, returns, and availability.
- **Role-Based Access:** Admin, Librarian, and Student roles using ASP.NET Core Identity.
- **Search and Pagination:** Easily navigate records and inventory.
- **Database Seeding:** Automatically populate sample library data.

## Technology Stack

| Technology | Purpose |
|---|---|
| C# | Backend programming |
| ASP.NET Core MVC | Web application framework |
| .NET 8 | Runtime and SDK |
| Entity Framework Core 8 | Database access |
| ASP.NET Core Identity | Authentication and roles |
| SQL Server / LocalDB | Database support |
| In-Memory Database | Development and testing option |
| HTML, CSS, JavaScript | Frontend |

## Project Structure

```text
MIB_Library-Management-System/
├── Controllers/
├── Data/
├── Models/
├── ViewModels/
├── Views/
├── wwwroot/
├── Program.cs
├── appsettings.json
├── LibraryManagementSystem.csproj
├── DOCUMENTATION.md
└── README.md
```

## Prerequisites

- Windows, Linux, or macOS
- .NET 8 SDK
- Visual Studio or Visual Studio Code
- SQL Server / LocalDB if using SQL Server mode

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/mib-library-management-system.git
cd mib-library-management-system
```

### 2. Restore dependencies

```bash
dotnet restore
```

### 3. Configure the database

Review `appsettings.json` and `Program.cs` to select the supported database configuration.

### 4. Configure administrator credentials

Set the following environment variables before running the application if you want the database seeder to create an administrator account:

- `MIB_ADMIN_EMAIL`
- `MIB_ADMIN_PASSWORD`

Do not commit actual credentials, API keys, or secrets to source control.

### 5. Build and run

```bash
dotnet build
dotnet run
```

Open the local URL displayed in the terminal.

## Security Notes

- Administrator credentials are supplied through environment variables.
- Never publish passwords or private credentials.
- Use secure configuration for production deployments.
- Review authentication and authorization settings before deployment.

## Project Purpose

This project demonstrates practical experience with ASP.NET Core MVC, database integration, authentication, role-based authorization, CRUD operations, and web application development.

## License

This project is available for educational and portfolio demonstration purposes. Add a license file if you intend to specify reuse and distribution permissions.