# QuantArena - Cryptocurrency Trading Simulator

QuantArena is a full-stack web application that allows users to practice cryptocurrency trading in a risk-free environment. Every new user starts with a simulated balance of 10,000 dollars in virtual cash. The platform fetches live, real-time cryptocurrency prices from an external data feed, handles buying and selling operations, manages inventory portfolios, and logs a permanent transaction history ledger.

## Core Features

1. Virtual Wallet: Automatically provisions a default balance of 10,000 dollars for simulated trading upon user initialization.
2. Live Market Rates: Connects to a live external network to pull the most current market prices for digital assets like Bitcoin and Ethereum.
3. Order Execution Engine: Validates user balances, calculates total order costs, executes instant fractional purchases or sales, and updates portfolio state balances.
4. Permanent Data Ledger: Records every single buy and sell order in a centralized database with exact quantities, prices, and timestamps.

## Technologies Used

* Frontend: React.js, React Router, Axios
* Backend: Node.js, Express.js, Dotenv
* Database: MongoDB, Mongoose (Object Data Modeling)
* External Connection: Live Cryptocurrency Price API

## Database Architecture

The backend utilizes MongoDB to permanently store three primary data formats:

* Users: Keeps track of basic profile accounts and their remaining virtual cash balances.
* Portfolios: Tracks the exact quantity of each specific cryptocurrency a user currently holds, along with their average buy prices.
* Transactions: Acts as an unchangeable record book logging the full history of every single trade executed on the platform.

## Local Installation Guide

Follow these steps to run this project on your computer:

### 1. Prerequisites
Make sure you have Node.js and MongoDB Community Server installed on your local operating machine.

### 2. Clone the Repository
Run this command in your terminal:
git clone https://github.com/YOUR_USERNAME/QuantArena.git
cd QuantArena

### 3. Setup the Database and Backend
Go into the backend folder and install the required packages:
cd backend
npm install

Start the backend server:
node server.js

The console will display a success message once the connection to your local MongoDB engine is established.

### 4. Setup the Frontend Website
Open a second terminal window, navigate into the frontend folder, install the user interface packages, and start the development server:
cd frontend
npm install
npm run dev

Open your internet browser and navigate to http://localhost:5173 to begin trading.
