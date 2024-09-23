# PropertyHub

### A location-based property listing platform with advanced search and filtering options

## Table of Contents
1. [Overview](#overview)
2. [Features](#features)
3. [Tech Stack](#tech-stack)
4. [Demo](#demo)
5. [Installation](#installation)
6. [Usage](#usage)
7. [Database Schema](#database-schema)
8. [Contributing](#contributing)
9. [License](#license)

## Overview
**PropertyHub** is a property listing platform designed to help users find and manage real estate listings with ease. Users can search for properties using various filters such as location, price, and type, and they can also authenticate securely to save their favorite properties or list their own.

## Features
- **Location-Based Search:** Users can find properties based on their geographical location.
- **Advanced Filtering:** Narrow down results by price, property type, and other criteria.
- **User Authentication:** Secure login and registration using authentication mechanisms.
- **Personalized Dashboard:** Users can save favorite properties, manage personal listings, and update preferences.
- **Responsive Design:** Optimized for both desktop and mobile users.

## Tech Stack
- **Frontend:** HTML, CSS, JavaScript
- **Backend:** Node.js, Express.js
- **Database:** MySQL
- **Authentication:** JSON Web Tokens (JWT)
- **Other Tools:** Docker (optional), Postman (for API testing)

## Demo

### Homepage
![Homepage Screenshot](images/home.png)

### Login Page
![Login/ Signup Screenshot](images/login.png)

### User Page
![Search Screenshot](docs/user.png)


## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/PropertyHub.git
   cd PropertyHub
   ```
2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   Create a `.env` file in the root directory and add the following:
   ```
   DB_HOST=your_mysql_host
   DB_USER=your_mysql_user
   DB_PASS=your_mysql_password
   DB_NAME=propertyhub
   JWT_SECRET=your_secret_key
   ```
5. Initialize the MySQL database:
   
   ```
   CREATE DATABASE propertyhub;
   ```

6. Start the application:
   ```bash
   npm start
   ```
   The app will be accessible at `http://localhost:3000`.
## Usage

- After starting the app, visit the homepage where you can search for properties using various filters.
- You can register an account to save your favorite properties or list your own.

## Database Schema
The MySQL database schema consists of the following tables:
- **Users:** Stores user account details (name, email, password).
- **Properties:** Stores property listings (title, description, price, location, owner).
- **Favorites:** Tracks users' saved properties.

For the detailed schema, refer to the `/database/schema.sql` file.

## Contributing
Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


