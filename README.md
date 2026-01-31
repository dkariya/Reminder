# AdminPanel

A modern full-stack Admin Admin Panel built with .NET 8 Web API and Angular 21. Features secure JWT authentication, Entity Framework Core with SQL Server, and a responsive Angular Material UI. Fully containerized with Docker for easy deployment and scalability.

## Tech Stack

### Backend (`AdminPanel.API`)
*   **.NET 8.0** (ASP.NET Core Web API)
*   **Entity Framework Core 8.0** (SQL Server)
*   **Identity** (JWT Authentication)
*   **Swagger/OpenAPI** (API Documentation)

### Frontend (`AdminPanel.Client`)
*   **Angular 21.0**
*   **TypeScript**
*   **Angular Material**
*   **Vitest** (Unit Testing)

### Infrastructure
*   **Docker & Docker Compose**

## Getting Started

### Prerequisites
*   [Docker Desktop](https://www.docker.com/products/docker-desktop/)
*   (Optional) [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0) and [Node.js](https://nodejs.org/) for local non-containerized development.

### Running with Docker (Recommended)

1.  Clone the repository:
    ```bash
    git clone <repository-url>
    cd AdminPanel
    ```

2.  Run the application using Docker Compose:
    ```bash
    docker-compose up --build
    ```

3.  Access the application:
    *   **Frontend**: http://localhost:4200
    *   **API**: http://localhost:8080
    *   **Swagger UI**: http://localhost:8080/swagger

### Running Locally (Manual)

#### Backend
1.  Navigate to `AdminPanel.API`:
    ```bash
    cd AdminPanel.API
    ```
2.  Update the connection string in `appsettings.json` if relying on a local SQL Server instance.
3.  Run the application:
    ```bash
    dotnet run
    ```

#### Frontend
1.  Navigate to `AdminPanel.Client`:
    ```bash
    cd AdminPanel.Client
    ```
2.  Install dependencies:
    ```bash
    npm install
    ```
3.  Start the development server:
    ```bash
    ng serve
    ```

## Project Structure

*   **/AdminPanel.API**: ASP.NET Core Web API backend.
*   **/AdminPanel.Client**: Angular Single Page Application.
*   **/AdminPanel.Tests**: Unit and integration tests.
*   **docker-compose.yml**: Orchestration for running the full stack.

## Features
*   **Authentication**: Secure login flow with JWT.
*   **Dashboard**: Overview of system status.
*   **Reminders**: Manage tasks and events with Google Calendar integration support.
