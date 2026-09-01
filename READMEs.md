# Google Maps Application

This application displays Google Maps using a React frontend and a Node.js backend. It includes user authentication and data persistence with MySQL.

## Project Structure

- **index.html**: Entry point for the Vite application.
- **src/main.jsx**: Main entry file for the React application.
- **src/App.jsx**: Root React component, setting up routes and rendering the main layout.
- **src/pages/MapPage.jsx**: React component that displays the Google Map.
- **src/components/Map.jsx**: Encapsulates the Google Map rendering logic.
- **src/components/Navbar.jsx**: Navigation bar component.
- **src/components/LoginForm.jsx**: Login form component for user authentication.
- **src/components/SignupForm.jsx**: Signup form component for new user registration.
- **vite.config.js**: Vite configuration file.
- **package.json**: Defines project dependencies and scripts.
- **server/index.js**: Entry point for the Express server.
- **server/routes/auth.js**: Authentication routes using JWT.
- **server/routes/health.js**: Health check route.
- **server/controllers/authController.js**: Handles authentication logic.
- **server/db/connection.js**: Sets up MySQL database connection.
- **server/middleware/authMiddleware.js**: Middleware for verifying JWT tokens.
- **server/utils/hash.js**: Utility functions for password hashing.
- **schema.sql**: Database schema definition.
- **.env.example**: Example environment variables file.

## Setup

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/google-maps-app.git
   cd google-maps-app
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

3. **Set up environment variables:**

   Create a `.env` file in the root directory and fill it with your configuration based on `.env.example`.

   ```
   JWT_SECRET=your_jwt_secret
   DB_HOST=your_db_host
   DB_USER=your_db_user
   DB_PASSWORD=your_db_password
   DB_NAME=your_db_name
   GOOGLE_MAPS_API_KEY=your_google_maps_api_key
   ```

4. **Set up the database:**

   Run the SQL commands in `schema.sql` to set up the database schema.

5. **Run the application:**

   Start the backend server:

   ```bash
   node server/index.js
   ```

   Start the frontend development server:

   ```bash
   npm run dev
   ```

## Running Locally

- Ensure MySQL is running and accessible with the credentials provided in your `.env` file.
- Start the backend server and the frontend development server as described in the setup section.
- Access the application at `http://localhost:3000`.

## Environment Variables

- **JWT_SECRET**: Secret used to sign JWT tokens.
- **DB_HOST**: Database host address.
- **DB_USER**: Database user.
- **DB_PASSWORD**: Password for the database user.
- **DB_NAME**: Database name.
- **GOOGLE_MAPS_API_KEY**: API key for accessing Google Maps services.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.