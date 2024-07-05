Eymen's Fruit Shop Budget App Frontend
This project serves as the frontend for Eymen's Fruit Shop Budget App, providing a user interface to manage transactions.

Features
View All Transactions: List all transactions.
View a Single Transaction: View details of a specific transaction.
Add a New Transaction: Add a new transaction to the list.
Edit a Transaction: Update an existing transaction.
Delete a Transaction: Remove a transaction from the list.
Responsive Design: Adjusts layout and styling for different screen sizes.
Styled with CSS: Custom styles for a clean and modern look.
Total Amount Display: Show the total amount of all transactions with visual feedback based on the amount.
Technologies Used
React
React Router
Vite
CSS
ESLint (for linting)
Environment Variables with .env
Setup Instructions
Clone the repository:

bash
Copy code
git clone <repository-url>
cd fruit-app-frontend
Install dependencies:

bash
Copy code
npm install
Set up environment variables:

Create a .env file in the root directory and add the following line:

env
Copy code
VITE_BASE_URL=http://localhost:4001/transactions
Run the development server:

bash
Copy code
npm run dev
Open your browser and go to http://localhost:3000 to view the application.

Build for production:

bash
Copy code
npm run build
The build files will be in the dist directory.

Run linting:

bash
Copy code
npm run lint
Project Structure
plaintext
Copy code
fruit-app-frontend/
│
├── public/             # Public assets
│
├── src/                # Source files
│   ├── components/     # React components
│   │   ├── Navbar.js
│   │   ├── Index.js
│   │   ├── Show.js
│   │   ├── New.js
│   │   └── Edit.js
│   │
│   ├── App.js          # Main App component
│   ├── App.css         # Global CSS styles
│   └── main.js         # Entry point
│
├── .env                # Environment variables
├── .eslintrc.js        # ESLint configuration
├── vite.config.js      # Vite configuration
├── package.json        # Project metadata and scripts
└── README.md           # This file
API Documentation
GET /transactions
Returns an array of all transactions.

GET /transactions/:arrayIndex
Returns the transaction at the specified arrayIndex.

POST /transactions
Adds a new transaction to the array. Requires a JSON body with item_name, amount, date, from, and category.

DELETE /transactions/:indexArray
Deletes the transaction at indexArray.

PUT /transactions/:arrayIndex
Updates the transaction at arrayIndex with new data. Requires a JSON body with item_name, amount, date, from, and category.

Contributing
Feel free to contribute to this project by opening issues or pull requests. Your feedback is much appreciated!