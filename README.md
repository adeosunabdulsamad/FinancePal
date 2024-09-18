# FinancePal Solo

FinancePal Solo is a personal finance tracking application designed to help users manage their expenses and monitor spending habits by connecting directly to their bank accounts using the Plaid API. The app provides users with insights into their finances through categorized transactions and custom reports.

![FinancePal Solo Screenshot](Screenshot%20(35).png)

## Features
- **Automated Transaction Categorization**: Pulls transaction data from your bank and automatically sorts it into categories like groceries, entertainment, utilities, etc.
- **Spending Reports**: Generate reports that show where you're spending your money over time.
- **Secure Bank Connection**: Uses the Plaid API to securely connect your bank accounts and retrieve financial data.
- **Responsive Design**: Accessible across devices with a mobile-friendly UI built using React.
- **Custom Alerts**: Set up alerts to notify you of overspending in particular categories.

## Tech Stack
- **Frontend**: React, JavaScript, HTML5, CSS3
- **Backend**: Python, Flask
- **Database**: MySQL
- **API**: Plaid API for transaction and bank account data
- **Version Control**: Git, GitHub
- **Deployment**: Docker, GitHub Actions

## Architecture Overview

![Architecture Diagram](link-to-diagram)

The FinancePal Solo application consists of three main components:
1. **Frontend (React)**: A responsive and user-friendly interface for managing your finances.
2. **Backend (Flask)**: Handles API requests, user authentication, and transaction data processing.
3. **Database (MySQL)**: Stores user data, transaction history, and categorized reports.

The app uses the Plaid API to securely retrieve transaction data from users' bank accounts and stores that data in a MySQL database. The backend processes and categorizes transactions, while the frontend provides an intuitive interface for users to track their spending.

## Getting Started

### Prerequisites
To run this project locally, you’ll need:
- Python 3.8+
- MySQL
- Node.js
- Plaid API keys (You can sign up for access [here](https://plaid.com/))

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/financepal-solo.git
   cd financepal-solo

2. Set up the backend:
  ```bash
  python3 -m venv env
  source env/bin/activate  # For Windows, use `env\Scripts\activate`
  pip install -r requirements.txt
  
3. Set up the MySQL database:
Create a MySQL database and update the connection string in config.py with your credentials.

4. Set up the frontend:
  ```bash
  Copy code
  cd frontend
  npm install
  npm start

5. Set up Plaid API keys:

Create a .env file in the root directory and add your Plaid API keys:
  ```bash
  Copy code
  PLAID_CLIENT_ID=your-client-id
  PLAID_SECRET=your-secret
  
6.Run the backend:

  ```bash
  Copy code
  flask run
