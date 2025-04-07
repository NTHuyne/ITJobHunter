# ITJobHunter

## Overview

ITJobHunter is a platform designed to connect job seekers with employers. It provides a comprehensive set of features for job searching, application management, and communication. The platform includes separate interfaces for employees, employers, and administrators, each with role-specific functionalities.

## Features

-   **Employee Interface:** Job searching, profile management, application submission, and direct messaging with employers.
-   **Employer Interface:** Job posting, application review, company profile management, and direct messaging with potential candidates.
-   **Administrator Interface:** User management, company verification, and platform analytics.
-   **Real-time Chat:** Integrated chat functionality for seamless communication between employees and employers.

## Technologies Used

### Client (React)

-   **React:** A JavaScript library for building user interfaces.
-   **TypeScript:** A superset of JavaScript that adds static typing.
-   **Tailwind CSS:** A utility-first CSS framework for rapid UI development.
-   **Redux Toolkit:** A set of tools and conventions that make working with Redux easier.
-   **Vite:** A fast build tool and development server for modern web projects.
-   **axios:** Promise based HTTP client for the browser and node.js

### Server (Node.js)

-   **Node.js:** An open-source, cross-platform JavaScript runtime environment.
-   **Express:** A minimal and flexible Node.js web application framework.
-   **Mongoose:** An Object Data Modeling (ODM) library for MongoDB and Node.js.
-   **JWT (JSON Web Tokens):** An open standard for securely transmitting information as a JSON object.
-   **dotenv:** Loads environment variables from a .env file into process.env.
-   **bcrypt:** A library for hashing passwords.
-   **cors:** A package for providing a Connect/Express middleware that can be used to enable CORS.

### Database

-   **MongoDB:** A NoSQL document database.

## Project Structure

```
itJobHunter/
├── client/  # React client application
│   ├── src/ # Source code
│   ├── public/ # Public assets
│   ├── ... # Other configuration files
├── server/  # Node.js/Express server application
│   ├── models/ # Mongoose models
│   ├── controllers/ # Route controllers
│   ├── routes/ # API routes
│   ├── config/ # Configuration files
│   ├── ... # Other server files
└── README.md
```

## Getting Started

### Prerequisites

-   Node.js and npm installed.
-   MongoDB installed and running.

### Installation

1.  Clone the repository:

    ```bash
    git clone [repository-url]
    ```

2.  Install server dependencies:

    ```bash
    cd server
    npm install
    ```

3.  Install client dependencies:

    ```bash
    cd client
    npm install
    ```

4.  Configure the server:

    -   Create a `.env` file in the `server/` directory based on the `.env.example` file.
    -   Set the MongoDB connection string, JWT secret, and other environment variables.

### Running the Application

1.  Start the server:

    ```bash
    cd server
    npm start
    ```

2.  Start the client:

    ```bash
    cd client
    npm run dev
    ```

## API Endpoints

The server provides the following API endpoints:

-   **Company Routes:**
    -   `POST /api/companies/register` - Register a new company.
    -   `POST /api/companies/login` - Login as a company.
    -   `GET /api/companies/:id` - Get company details.
    -   `PUT /api/companies/:id` - Update company details.
    -   `DELETE /api/companies/:id` - Delete a company.

-   **Employee Routes:**
    -   `POST /api/employees/register` - Register a new employee.
    -   `POST /api/employees/login` - Login as an employee.
    -   `GET /api/employees/:id` - Get employee details.
    -   `PUT /api/employees/:id` - Update employee details.
    -   `DELETE /api/employees/:id` - Delete an employee.

-   **Job Routes:**
    -   `POST /api/jobs` - Create a new job.
    -   `GET /api/jobs` - List all jobs.
    -   `GET /api/jobs/:id` - Get job details.
    -   `PUT /api/jobs/:id` - Update job details.
    -   `DELETE /api/jobs/:id` - Delete a job.

-   **Job Application Routes:**
    -   `POST /api/job-applications` - Create a new job application.
    -   `GET /api/job-applications/:id` - Get job application details.
    -   `PUT /api/job-applications/:id` - Update job application details.
    -   `DELETE /api/job-applications/:id` - Delete a job application.

-   **Message Routes:**
    -   `POST /api/messages` - Send a new message.
    -   `GET /api/messages/:conversationId` - Get all messages in a conversation.

## Contributing

Contributions are welcome! Please follow these steps:

1.  Fork the repository.
2.  Create a new branch for your feature or bug fix.
3.  Commit your changes.
4.  Push to the branch.
5.  Create a pull request.

