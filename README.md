# School Payments Backend

This is the backend for the School Payments application. It handles user authentication, payments, transactions, and webhooks.

## Features
- User registration and login with JWT authentication
- Payment creation and transaction handling
- Webhook endpoints for payment updates
- MongoDB database integration
- CORS enabled for frontend deployment

## Tech Stack
- Node.js
- Express.js
- MongoDB (Mongoose)
- dotenv for environment variables
- CORS middleware

## Installation

1. Clone the repository:

       git clone https://github.com/ermemon12/school-payments-backend.git
Navigate to the backend folder:


    cd school-payments-backend
2. Install dependencies:


       npm install
3. Create a .env file in the root with the following variables:


       PORT=5000
       MONGO_URI=<your_mongodb_connection_string>
       JWT_SECRET=<your_jwt_secret>
       PAYMENT_API_KEY=<your_payment_api_key>
       PG_KEY=<your_pg_key_if_any>
4. Start the server (development):


       npm start
Server will run at http://localhost:5000.

## API Endpoints

### Auth

    POST /api/users/register → Register new user

    POST /api/users/login → Login user

### Payments

    POST /api/payments → Create payment

    GET /api/transactions → Get all transactions

### Webhooks

    POST /api/webhook → Payment gateway webhooks






# School Payments Frontend

This is the frontend for the School Payments application built with React.

## Features
- Landing page with “Get Started” CTA
- User registration and login
- Secure token-based authentication (JWT)
- Payment creation and viewing
- Dark/Light mode toggle

## Tech Stack
- React.js
- React Router
- Axios for API calls
- Tailwind CSS for styling

## Installation

1. Clone the repository:

       git clone https://github.com/ermemon12/school-payments-frontend.git
2. Navigate to the frontend folder:


       cd school-payments-frontend
3. Install dependencies:


       npm install
4. Create a .env file if needed (for API URLs):


       REACT_APP_API_URL=https://school-payments-backend-42rn.onrender.com/api
5. Start the development server:


       npm start
The frontend will run at http://localhost:3000.

### Deployment
You can build the app for production using:


    npm run build
Then deploy the contents of the build folder to Netlify, Vercel, or any static hosting service.
