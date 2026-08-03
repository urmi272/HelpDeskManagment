# HelpDesk Management System

A full-stack Help Desk Management System built using **ASP.NET Core 8**, following a clean layered architecture with separate API and MVC projects. The application allows users to create, manage, update, and track support tickets efficiently.

## Features

- Create new help desk tickets
- View all submitted tickets
- Update ticket details
- Change ticket status
- Delete tickets
- RESTful Web API
- ASP.NET Core MVC Frontend
- Entity Framework Core with SQL Server
- Input validation using Data Annotations
- Swagger API Documentation
- Layered Architecture
- Unit Testing Support

---

## Tech Stack

### Backend
- ASP.NET Core 8 Web API
- Entity Framework Core
- SQL Server LocalDB
- C#

### Frontend
- ASP.NET Core MVC
- Razor Views
- Bootstrap

### Testing
- xUnit

### Tools
- Visual Studio 2022
- Swagger
- Git & GitHub

---

## Project Structure

```
HelpDeskManagement
│
├── HelpDesk.Api
│   ├── Controllers
│   ├── DTOs
│   ├── Models
│   ├── Data
│   ├── Services
│   ├── Repositories
│   └── Program.cs
│
├── HelpDesk.Mvc
│   ├── Controllers
│   ├── Views
│   ├── Models
│   ├── Services
│   └── Program.cs
│
├── HelpDesk.Tests
│
└── HelpDeskManagement.sln
```

---

## API Endpoints

| Method | Endpoint | Description |
|---------|----------|-------------|
| GET | `/api/Ticket/All` | Get all tickets |
| GET | `/api/Ticket/{id}` | Get ticket by ID |
| POST | `/api/Ticket` | Create a ticket |
| PUT | `/api/Ticket/{id}` | Update a ticket |
| DELETE | `/api/Ticket/{id}` | Delete a ticket |

---

## Getting Started

### Clone the repository

```bash
git clone https://github.com/urmi272/HelpDeskManagement.git
```

### Navigate to the project

```bash
cd HelpDeskManagement
```

### Restore packages

```bash
dotnet restore
```

### Apply database migrations

```bash
dotnet ef database update
```

### Run the API

```bash
cd HelpDesk.Api
dotnet run
```

### Run the MVC application

```bash
cd HelpDesk.Mvc
dotnet run
```

---

## Swagger

After running the API, open:

```
https://localhost:<port>/swagger
```

---

## Author

**Urmi Barman**

GitHub: https://github.com/urmi272

---

## License

This project is licensed under the MIT License.
