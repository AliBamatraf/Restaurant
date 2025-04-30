# 🍽️ Restaurant Management System

> **A modular, scalable, and maintainable restaurant management system built with ASP.NET Core following Clean Architecture principles.**  
> This project serves as a robust foundation for developing enterprise-grade web applications in the food service industry.

---

## 🧱 Architecture Overview

This solution is structured to promote **separation of concerns**, **testability**, and **scalability**:

- **Restaurant.Domain**: Core business entities and interfaces.
- **Restaurant.Application**: Business logic, use cases, and service contracts.
- **Restaurant.Infrastructure**: External services like data persistence and third-party integrations.
- **Restaurant.Persistence**: Database context and configurations.
- **Restaurant.Identity**: Authentication and authorization mechanisms.
- **Restaurant.Api**: RESTful API endpoints.
- **Restaurant.MVC**: User-friendly web interface for end-users.

---

## 🚀 Getting Started

### Prerequisites

- [.NET 6 SDK](https://dotnet.microsoft.com/download/dotnet/6.0)
- [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)
- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/AliBamatraf/Restaurant.git
   cd Restaurant
   ```

2. **Configure the database**

   Update the `appsettings.json` files in `Restaurant.Api` and `Restaurant.Identity` to match your SQL Server connection settings.

3. **Apply migrations**

   ```bash
   dotnet ef database update --project Restaurant.Persistence
   ```

4. **Run the application**

   ```bash
   dotnet run --project Restaurant.Api
   ```

   Access the API at:  
   ➡️ `https://localhost:5001` or `http://localhost:5000`

---

## 📦 Features

- 🔐 **User Authentication & Authorization** — Secure login and role-based access control.
- 🧾 **Menu Management** — CRUD operations for menu items and categories.
- 📦 **Order Processing** — Manage customer orders and track statuses.
- 📅 **Reservation System** — Book and manage table reservations.
- 📊 **Reporting** — Generate sales and performance reports.
- 🖥️ **Responsive UI** — Built with ASP.NET Core MVC and Razor Pages.

---

## 🛠️ Technologies Used

| Category         | Technology                              |
| ---------------- | ---------------------------------------- |
| Backend          | ASP.NET Core 6, Entity Framework Core, AutoMapper |
| Authentication   | ASP.NET Core Identity, JWT              |
| Database         | SQL Server                              |
| Frontend         | ASP.NET Core MVC, Razor Pages            |
| Architecture     | Clean Architecture                     |

---

## 📁 Project Structure

```bash
Restaurant/
├── Restaurant.Api/            # API Layer
├── Restaurant.Application/    # Business Logic
├── Restaurant.Domain/         # Core Entities & Interfaces
├── Restaurant.Identity/       # Authentication & Authorization
├── Restaurant.Infrastructure/ # External Service Implementations
├── Restaurant.MVC/            # Web UI
├── Restaurant.Persistence/    # Database Context & Migrations
└── Restaurant.sln             # Solution File
```

---

## 🧪 Testing

Unit and integration tests can be added using **xUnit** or **NUnit** frameworks.  
Make sure to **mock dependencies** to keep test cases isolated and reliable.

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 🤝 Contributing

Contributions are **welcome and appreciated**!  
If you have suggestions, ideas, or bug fixes:

1. Fork the repository.
2. Create a feature branch.
3. Open a pull request.

---

## 📬 Contact

For questions, issues, or collaboration:  
👤 [Ali Bamatraf](https://github.com/AliBamatraf)
