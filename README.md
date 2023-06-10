# Backend for Smart Brain App

This is the backend server for the application. It provides the necessary API endpoints to interact with the database and handle user authentication and image processing.

## Technologies Used

- Node.js
- Express.js
- PostgreSQL
- Knex.js
- Bcrypt.js
- Cors

## Getting Started

To get started with the backend server, follow the instructions below.

### Prerequisites

- Node.js and npm must be installed on your machine.
- PostgreSQL database with the required tables must be set up.

### Installation

1. Clone the repository:

   ```shell
   git clone https://github.com/LukeHSalmons/SmartBrainAPI.git
   ```

2. Navigate to the project directory:

   ```shell
   cd backend-server
   ```

3. Install the dependencies:

   ```shell
   npm install
   ```

4. Set up the database:

   - Create a PostgreSQL database.
   - Update the `connection` object in the `knex` configuration in `server.js` with your database details.

5. Start the server:

   ```shell
   npm start
   ```

   The server will run on http://localhost:3001/ by default.

## API Endpoints

The following API endpoints are available:

- `POST /signin`: Handles user sign-in and authentication.
- `POST /register`: Handles user registration.
- `GET /profile/:id`: Retrieves user profile information.
- `PUT /image`: Updates user image count.

## Database Schema

The application uses a PostgreSQL database with the following tables:

- `users`: Stores user information such as name, email, password, and joined date.

## Configuration

The server uses environment variables for configuration. The following environment variables should be set:

- `DATABASE_URL`: Connection string for the PostgreSQL database.
- `DATABASE_HOST`: Hostname of the PostgreSQL server.
- `DATABASE_USER`: Username for the PostgreSQL database.
- `DATABASE_PW`: Password for the PostgreSQL database.
- `DATABASE_DB`: Name of the PostgreSQL database.
- `PORT`: Port number on which the server should run.
