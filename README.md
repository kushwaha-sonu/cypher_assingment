

Project Setup

Prerequisites
Node.js (v14 or higher)
npm (v6 or higher)


Backend Setup
Navigate to the backend directory:  

cd backend
Install dependencies:  
npm install

Create a .env file in the backend directory and add the following environment variables:  
PORT=4000
MONGO_URI='your_mongo_uri'
JWT_SECRET='your_jwt_secret'
GOOGLE_EMAIL='your_google_email'
GOOGLE_PASSWORD='your_google_password'
EMAIL_FROM='your_email_from'

Start the backend server:  
npm run dev

Frontend Setup
Navigate to the frontend directory:  
cd frontend
Install dependencies:  

npm install
Start the frontend development server:  
npm run dev



Running the Application
Start the backend server:  
cd backend
npm run dev

Start the frontend development server:  
cd frontend
npm run dev
Open your browser and navigate to:  
http://localhost:5173


Build for Production

Build the frontend:  
cd frontend
npm run build

Start the backend server:
cd backend
npm start

Scripts
Backend
npm run dev: Starts the backend server with nodemon for development.
npm start: Starts the backend server.


Frontend
npm run dev: Starts the frontend development server.
npm run build: Builds the frontend for production.
