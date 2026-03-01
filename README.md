# Falcon Crest Bank

## Project Overview
Falcon Crest Bank is an innovative banking application designed to offer customers a seamless and secure online banking experience. The app allows users to manage their accounts, perform transactions, and access various banking services from the comfort of their homes.

## Features
- **User Authentication**: Secure login and registration process for users.
- **Account Management**: Users can view account balances and transaction history.
- **Funds Transfer**: Easy transfer of funds between accounts.
- **Bill Payments**: Pay bills quickly and hassle-free.
- **Dashboard**: View account overview and recent transactions.
- **Customer Support**: Access to customer service.

## Tech Stack
- **Frontend**: React.js
- **Backend**: Node.js with Express
- **Database**: PostgreSQL
- **Authentication**: JWT (JSON Web Tokens)

## Project Structure
```
falcon-crest-bank/
├── frontend/                 # React frontend application
│   ├── src/
│   ├── public/
│   └── package.json
├── backend/                  # Node.js backend API
│   ├── routes/
│   ├── controllers/
│   ├── models/
│   ├── middleware/
│   └── server.js
├── database/                 # Database schema and migrations
│   └── schema.sql
└── README.md
```

## Setup Instructions

### Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a .env file with database credentials and JWT secret
4. Run migrations:
   ```bash
   npm run migrate
   ```
5. Start the server:
   ```bash
   npm start
   ```

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm start
   ```
4. Open http://localhost:3000 in your browser

## API Endpoints
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login user
- `GET /api/accounts` - Get user accounts
- `GET /api/transactions` - Get transaction history
- `POST /api/transfers` - Transfer funds
- `POST /api/bills/pay` - Pay bills

## Security Features
- Password hashing with bcrypt
- JWT-based authentication
- Protected API routes with middleware
- SQL injection prevention with parameterized queries
- HTTPS support

## Contributing
Contributions are welcome! Please feel free to submit pull requests or open issues.

## License
MIT License