## Project Overview

This project aims to provide a basic user management system with the following functionalities:

- **Listing Users**: Display a table of all users.
- **Adding User**: Open a form for user registration via a popup modal.
- **Deleting User**: Prompt a confirmation popup to delete a selected user.
- **Export Users**: Export the selected users' data in CSV format.

## Technology Stack

- **Backend**: Node.js with Express.js
- **Database**: MongoDB
- **Frontend**: ReactJS
- **Styling**: HTML5 and CSS3

## Features

- RESTful APIs for CRUD operations on users.
- Form validations in the signup form.
- Sorting and pagination in the users' table.
- A loading indicator during CSV export.

## Project Structure

- **Backend**: Located in the `/backend` folder.
- **Frontend**: Located in the `/frontend` folder.

## Setup Instructions

### Prerequisites

- **Node.js** and **npm** (for the backend and frontend setup)
- **MongoDB** (database)

### Backend Setup

1. **Install Dependencies**: Navigate to the `/backend` folder and install dependencies.
   ```bash
   cd backend
   npm install
Configure Environment Variables: Create a .env file in the /backend folder and add your MongoDB connection string.

bash
Copy code
MONGODB_URI=<your_mongodb_connection_string>
PORT=5000
Run the Backend Server:

bash
Copy code
npm start
Frontend Setup
Install Dependencies: Navigate to the /frontend folder and install dependencies.

bash
Copy code
cd frontend
npm install
Run the Frontend Application:


# deploy link front end :- https://frontend-one-jet-80.vercel.app/
# depploy link backend :-  https://backend-0j6o.onrender.com/




## Features
### 1. Usage
#### Listing Users
- ** View: The main page displays a table of all users, showing their first name, last name, and email.
- ** Sort: Click on column headers to sort the table by first name, last name, or email.
- ** Paginate: Navigate through the list of users using pagination controls if there are many users.
Adding a User
- ** Sign Up: Click the "SIGN UP" button to open the registration form.
- ** Form: Enter the user's first name, last name, email, and password.
- ** Submit: Click "SIGN UP" to add the new user.
Deleting a User
- ** Delete: Click the "DELETE" button next to the user you wish to remove.
- ** Confirm: A confirmation prompt will appear. Click "DELETE" to confirm or "CANCEL" to abort.
Exporting Users
- ** Select Users: Use checkboxes in the table to select users.
- ** Export: Click the "EXPORT" button to download the selected users’ data as a CSV file.
2. API Endpoints
- ** GET /users: Fetch all users.
- ** POST /users: Add a new user.
- ** DELETE /users/:id: Delete a user by ID.
- ** GET /users/export: Export selected users' data in CSV format.
3. Database Design
- ** The application uses a single collection users in MongoDB, structured as follows:

_id: ObjectId (unique identifier)
- ** firstName: String (user's first name)
- ** lastName: String (user's last name)
- ** email: String (user's email address)
- ** password: String (user's password, stored in plain text for this example)
- ** deleted: Boolean (indicates if the user is deleted, default is false)
4. Frontend Components
- ** UserTable: Displays a list of users with options for sorting and pagination.
- ** SignUpForm: A modal form for adding new users, with validations for email and password strength.
- ** DeleteUserPrompt: A modal prompt for confirming user deletion.
- **ExportButton: Exports selected users’ data to a CSV file.
5. Feedback and Comments
- ** The application adheres to best practices in API design and code organization.
- ** The UI design is simple and user-friendly, providing clear prompts and feedback for user actions.
- **Implementing sorting and pagination enhances the user experience when dealing with a large dataset.
- ** Future enhancements could include more comprehensive form validation and additional features like user role management.
Getting Started
