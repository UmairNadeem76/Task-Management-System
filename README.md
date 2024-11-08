# Task Management System

## Getting Started

## Table of Contents
- [Prerequisites](#prerequisites)
- [Backend Setup](#backend-setup)
- [Frontend Setup](#frontend-setup)
- [Tech Stack](#tech-stack)
- [Additional Information](#additional-information)

## Prerequisites
Make sure you have the following installed on your machine:
- .NET SDK (version 6.0 or later)
- Node.js (version 14.0 or later)
- npm (Node Package Manager)
- SQL Server (or other preferred database)

## Backend Setup
### 1. Clone the repository:
```bash
git clone https://github.com/UmairNadeem76/Task-Management-System
cd Task-Management-System
```

### 2. Configure the database:
- Update the `appsettings.json` file with your database connection string.
- Example `appsettings.json`:
  ```json
  {
    "ConnectionStrings": {
      "Default": "Server=GAMINGPC\\SQLEXPRESS; Database=CustomAuth; Trusted_Connection=True; MultipleActiveResultSets=true; TrustServerCertificate=True;"
    },
    ...
  }
  ```

### 3. Run Entity Framework migrations:
```bash
cd CustomAuth
dotnet ef migrations add InitialCreate
dotnet ef database update
```

### 4. Install dependencies:
```bash
dotnet restore
```

### 5. Running the Backend
```bash
dotnet run
```
The backend API will be available at `http://localhost:5191`


## Frontend Setup
### 1. Navigate to the frontend directory:
```bash
cd ../new-frontend
```

### 2. Install dependencies:
```bash
npm install
```


### 3. Running the Frontend
```bash
npm start
```
The frontend will be available at ` http://localhost:3000/`.


# Tech Stack:
Following Tech Stack is being implemented:
- React + Typescript for frontend
- ASP.NET Core Web Api
- SQL Server Management Studio for database
- Redux for state management in React
- Serilog for Application logging (to be implemented)
- xUnit for unit testing (to be implemented)
- SonarQube for analyzing code quality (to be implemented)

## Additional Information
TBD