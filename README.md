
Built by https://www.blackbox.ai

---

```markdown
# ERP 365Trip

## Project Overview
ERP 365Trip is a complete web application that integrates a backend service with a MongoDB database and a frontend interface to provide a user-friendly experience for managing trips. This project is designed to help users manage their travel itineraries, bookings, and related information efficiently. The application is structured into distinct services, utilizing Docker for containerization and deployment.

## Installation

To get started with ERP 365Trip, ensure you have Docker and Docker Compose installed on your machine. You can follow the installation steps below:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/erp-365trip.git
   cd erp-365trip
   ```

2. **Build and start the services:**
   ```bash
   docker-compose up --build
   ```

3. **Access the application:**
   - Frontend: [http://localhost:8000](http://localhost:8000)
   - Mongo Express (to manage MongoDB data): [http://localhost:8081](http://localhost:8081)

## Usage

Once the application is running, you can interact with the frontend to manage your trips. The application allows users to log in, manage itineraries, and access various features related to travel management.

- You can customize the MongoDB connection details, JWT secret, and other configurations within the `docker-compose.yml` file.
- The frontend is served via an Nginx web server, ensuring performance and reliability.

## Features

- **Multi-tier Architecture:** Separate services for frontend, backend, and database.
- **MongoDB Integration:** Persistent data storage using MongoDB.
- **User Authentication:** Secured with JWT for safe user sessions.
- **Administration UI:** Access and manage the MongoDB database through Mongo Express.

## Dependencies

The application consists of the following main dependencies, which are defined in the respective Docker images and services:

- **Backend Service:**
  - Node.js (with Express framework)
  - Mongoose (for MongoDB interactions)
  
- **Frontend Service:**
  - Nginx (for serving the static frontend files)

- **MongoDB Service:**
  - MongoDB (version 5.0)
  
- **Mongo Express:**
  - A simple web-based MongoDB admin interface.

## Project Structure

The project is structured as follows:

```
/erp-365trip
├── backend              # Contains the backend code (Node.js)
├── frontend             # Contains the frontend code (HTML/CSS/JavaScript)
├── docker-compose.yml   # Configuration for Docker services
```

Each service is designed to allow for easy scaling and deployment, ensuring that developers can maintain clear separation of concerns and can work independently on different components of the application.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```