# Expense Tracking Application

**A MERN Stack Project for Tracking Expenses and Visualizing Data**

Expense Tracking Application is a full-stack project built using the MERN stack (MongoDB, Express.js, React, and Node.js). It helps users manage their expenses and gain insights into their spending habits through data visualization.

## Features

- **MERN Stack Architecture:**
  - Developed with MongoDB, Express.js, React, and Node.js.
  - Implements an MVC architecture, separating the backend (in the `server` directory) from the frontend (in the `client` directory) for easier maintenance and scalability.

- **User Authentication:**
  - **Google Login using OAuth 2.0:** Quickly authenticate using your Google account.
  - **Email Login with JWT:** Secure login via email/password using JSON Web Tokens for authentication.

- **RESTful API:**
  - Provides endpoints for managing user information, expense categories, and expense records.
  - Designed following RESTful principles for clean and efficient integration.

- **Data Visualization:**
  - Displays expense data with interactive visualizations to help users understand spending trends.

- **Security:**
  - Uses `express-rate-limit` to protect the backend from sudden surges in traffic and potential malicious attacks.

- **Deployment:**
  - Successfully deployed on AWS EC2, ensuring reliable performance and scalability.

## Project Structure

```plaintext
expense-tracking-application/
├── client/                # Frontend React application
│   ├── package.json       # Client dependencies and scripts
│   ├── public/            # Static files (e.g., index.html, images)
│   └── src/               # React components, styles, and source code
├── server/                # Backend Node.js/Express application
│   ├── package.json       # Server dependencies and scripts
│   ├── app.js             # Main entry point for the server
│   └── routes/            # RESTful API route handlers
├── README.md              # Project documentation and setup guide
└── .gitignore             # Files and directories to be ignored by Git (e.g., node_modules/)
```

## Getting Started

### Prerequisites

- Node.js (v14 or higher recommended)
- npm or yarn
- MongoDB (local or cloud instance)

### Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/your-username/expense-tracking-application.git
   cd expense-tracking-application

2. **Set Up the Backend:**
   ```bash
   cd server
   npm install

- Create a `.env` file in the `server` directory with the necessary environment variables (e.g., MongoDB URI, JWT secret, Google OAuth credentials).
3. **Set Up the Frontend:**
    ```bash
    cd ../client
    npm install

- Configure any required environment variables in a `.env` file for the frontend.
4. **Run the Application:**
  - **Start the Backend:**
    ```bash
    cd ../server
    npm start

  - **Start the Frontend:**
    ```bash
    cd ../client
    npm start

### Deployment
For deployment, the application is hosted on AWS EC2. In production, consider using process managers like PM2 for the backend and ensure that environment variables are securely managed.

### Contributing
Contributions are welcome! If you have suggestions, improvements, or bug fixes, feel free to open an issue or submit a pull request.

### License
This project is licensed under the Apache License, Version 2.0.  
See the [LICENSE](LICENSE) file for more details.
