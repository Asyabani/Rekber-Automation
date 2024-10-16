# Rekber Automation

Rekber Automation is a secure and efficient platform designed to facilitate transactions between buyers and sellers through an escrow (rekening bersama) system. The platform ensures a safe, trustworthy environment by holding payments in escrow until both parties are satisfied with the transaction, integrating verification and dispute resolution to ensure seamless operation.

## Features

- **Secure Escrow System**: Payments are held in escrow until transaction completion, ensuring buyer and seller protection.
- **Buyer-Seller Chat**: Built-in chat feature for buyers and sellers to communicate directly during a transaction.
- **Transaction Management**: Track order status, view transaction history, and manage payments.
- **Dispute Resolution**: Admin intervention for resolving disputes between buyers and sellers.
- **Verification System**: Both buyers and sellers can be verified through identity checks (optional for buyers, mandatory for sellers).
- **Notifications**: Real-time notifications about transaction status, disputes, and updates.
- **Admin Dashboard**: Admins can manage disputes, monitor transactions, and verify users.

## Tech Stack

### Backend
- **Node.js** - Provides scalable performance for backend services.
- **Express** - Used for building the RESTful API server.
- **MongoDB** - NoSQL database for flexible data management.

### Frontend
- **Next.js** - Server-side rendering and client-side navigation for a seamless user experience.
- **React.js** - Modular and efficient frontend development.
- **React Bootstrap** - For a flexible, responsive, and accessible design system.
- **Socket.IO** - Real-time communication for chat and notifications.

### Other Tools
- **ESLint** - Linting to ensure clean, consistent code.
- **Prettier** - Code formatting to maintain readability.
- **Docker** - Containerization for easy deployment.

## Prerequisites
Ensure you have the following installed:
- [Node.js](https://nodejs.org/)
- [Yarn](https://yarnpkg.com/)
- [MongoDB](https://www.mongodb.com/)

## Installation
1. Clone the repository:
    ```bash
    git clone "https://github.com/orgs/rekber-automation/rekber"
    ```

2. Navigate to the project directory:
    ```bash
    cd rekber
    ```

3. Install dependencies:
    ```bash
    yarn install
    ```

4. Set up environment variables:
    - Copy `.env.example` to `.env`:
        ```bash
        cp .env.example .env
        ```
    - Update the `.env` file with your MongoDB URI, API keys, and other environment-specific variables.

5. Start the development server:
    ```bash
    yarn dev
    ```
   Open [http://localhost:3000](http://localhost:3000) in your browser.


## Directory Structure
```plaintext
REKBER-AUTOMATION/
│
├── README.md                   # Overview of the entire project
│
├── backend/                    # Backend application directory
│   ├── src/                    # Source code for the backend
│   │   ├── config/             # Configuration files (e.g., database, environment variables)
│   │   ├── controllers/        # Controller functions for handling requests
│   │   ├── models/             # Database models (e.g., User, Transaction)
│   │   ├── routes/             # Express route handlers
│   │   ├── services/           # Business logic and service functions
│   │   ├── middlewares/        # Middleware functions (e.g., authentication)
│   │   └── app.js              # Main application file for Express server
│   ├── .env.example            # Example environment configuration
│   ├── .eslintrc.js            # ESLint configuration for backend
│   ├── Dockerfile              # Docker configuration for backend
│   ├── package.json            # Project dependencies and scripts for backend
│   └── README.md               # Documentation for the backend
│
├── frontend/                   # Frontend application directory
│   ├── public/                 # Static assets (favicon, logos, etc.)
│   ├── src/                    # Source code for the frontend
│   │   ├── assets/             # Static assets like CSS, images, and fonts
│   │   ├── components/         # Reusable UI components
│   │   ├── context/            # Context providers for global state
│   │   ├── hooks/              # Custom React hooks for shared logic
│   │   ├── layouts/            # Page layouts (e.g., AuthLayout, MainLayout)
│   │   ├── pages/              # Application pages (Home, Orders, etc.)
│   │   ├── services/           # API service functions and business logic
│   │   ├── store/              # Redux or Zustand store configuration
│   │   ├── utils/              # Utility functions and helper methods
│   │   ├── validation/         # Form validation schema (e.g., Yup validation)
│   │   └── App.js              # Main entry point for the React application
│   ├── .env.example            # Example environment configuration for frontend
│   ├── .eslintrc.js            # ESLint configuration for frontend
│   ├── .prettierrc             # Prettier configuration for frontend
│   ├── Dockerfile              # Docker configuration for frontend
│   ├── package.json            # Project dependencies and scripts for frontend
│   └── README.md               # Documentation for the frontend
│
└── docs/                       # Documentation for the entire project
    ├── architecture/           # Architectural overview and design decisions
    ├── api/                    # API documentation (endpoints, request/response)
    ├── backlog/                # Project backlog (user stories, tasks)
    ├── erd/                    # Entity-Relationship Diagram documentation
    └── index.md                # Epic Overview     

```


## Backlog

For detailed information on the project backlog, including user stories and tasks, visit the [Backlog Documentation](./docs/index.md).
## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.