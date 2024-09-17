# HW1 - Spring Boot Backend and JavaScript Frontend

This repository contains the code for Homework 1, which includes a backend built using Spring Boot and a frontend built using JavaScript.

## Project Structure

The project is organized into two main directories:

- `/frontend`: This contains the JavaScript frontend code.
- `/backend`: This contains the Spring Boot backend code.

## Prerequisites

To run this project locally, you will need to have the following software installed:

- **Java 11 or higher**: Required to run the Spring Boot backend.
- **Maven**: Required to build and manage the Spring Boot project.
- **Node.js** and **npm**: Required to install dependencies and run the JavaScript frontend.
- **Git**: Required to clone the repository.

## Cloning the Repository

You can clone the repository using the following command:

```bash
git clone https://github.com/imanunited/hw1.git
cd hw1
```
## Backend Setup (Spring Boot)

Navigate to the backend directory:

```bash
cd backend
```
Build the project using Maven:

```bash
mvn clean install
```
Run the Spring Boot application:

```bash
mvn spring-boot:run
```
The backend will be available at http://localhost:8080.

### Backend Notes:
- The backend is a Spring Boot application that exposes REST APIs for the frontend to consume.
- By default, the backend runs on port 8080. You can change this in the application.properties file if needed.
- Ensure CORS settings are correctly configured to allow the frontend to interact with the backend.
## Frontend Setup (JavaScript)
Navigate to the frontend directory:

```bash
cd ../frontend
```

Install the required npm dependencies:

```bash
npm install
```
Start the frontend development server:

```bash
npm start
```
The frontend will be available at http://localhost:3000.

### Frontend Notes:
- The frontend interacts with the backend via REST API calls.
- You can configure the backend URL in the frontend code if needed (usually in a configuration file or .env file).
- The development server provides hot-reloading, which means any changes you make to the frontend will be automatically reflected.
## Running the Application
Make sure both the backend and frontend are running:

- The backend will be running at http://localhost:8080.
- The frontend will be running at http://localhost:3000.
Open a browser and go to http://localhost:3000 to interact with the application.

## Troubleshooting
- CORS Issues: If the frontend cannot communicate with the backend due to CORS (Cross-Origin Resource Sharing) restrictions, ensure that CORS is properly configured in the backend. You can modify the backend to allow requests from http://localhost:3000.
- Port Conflicts: If another application is using ports 8080 or 3000, either stop the conflicting application or change the ports in the backend's application.properties and frontend's configuration.

## Additional Information
- Ensure both the frontend and backend are running at the same time for the application to work correctly.
- You can modify the CORS settings in the backend if you're testing from a different domain or port.
## Contact
If there are any questions or issues, please contact me :jfu44@jh.edu.
