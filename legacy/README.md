# Loan Advisor

A simple web application for predicting loan eligibility using a pre-trained machine learning model.

## Features

- Form for inputting loan application details
- Prediction of loan eligibility using a simplified model
- Storage of loan applications in MongoDB
- Clean, responsive UI using Tailwind CSS

## Tech Stack

- **Backend**: Node.js, Express
- **Frontend**: EJS, Tailwind CSS, Vanilla JavaScript
- **Database**: MongoDB
- **ML Model**: Simplified rule-based prediction (placeholder for actual ML model)

## Setup Instructions

### Prerequisites

- Node.js (v14 or higher)
- MongoDB (local or remote instance)

### Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd loan-advisor
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Create a `.env` file in the root directory with the following content:
   ```
   MONGODB_URI=mongodb://localhost:27017/loanAdvisor
   PORT=3000
   ```
   
   Adjust the MongoDB URI as needed for your setup.

4. Start the application:
   ```
   npm start
   ```

   For development with auto-reload:
   ```
   npm run dev
   ```

5. Open your browser and navigate to `http://localhost:3000`

## ML Model Integration

The current implementation uses a simplified rule-based approach to simulate predictions. In a production environment, you would need to:

1. Place your `model.pkl` and `scaler.pkl` files in the `/public` directory
2. Update the `predictionService.js` to use actual model loading and prediction

## Project Structure

- `index.js` - Main Express application
- `routes/` - API routes
- `models/` - MongoDB schema definitions
- `services/` - Business logic services
- `views/` - EJS templates
- `public/` - Static assets and client-side JavaScript
- `utils/` - Utility functions

## License

MIT