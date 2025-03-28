﻿# E-Learning-platform
Pre-Requisite:
Ensure that Node.js is installed on your system. You can check it by running:
node -v
If it's not installed, download it from the official Node.js website.

Setup Instructions:
Navigate to the Project Folder: Go to the directory where you have the StudyNotion project:
cd path/to/StudyNotion
Install Project Dependencies: In the root directory of your project, run:
npm install
Navigate to the server Directory: After the frontend dependencies are installed, move into the server directory:
cd server
Install Server Dependencies: Inside the server folder, run:
npm install
Start the Server: Once the dependencies are installed, start the server by running:
npm start

Configuration:
Create a .env file in the server folder and add the following environment variables:
# Server Configuration
PORT=4000  

# MongoDB Connection
MONGODB_URL="mongodb+srv://<USERNAME>:<PASSWORD>@cluster0.<CLUSTER_ID>.mongodb.net/<DATABASE_NAME>"  

# Email Configuration
MAIL_HOST=smtp.gmail.com  
MAIL_USER=<YOUR_EMAIL>  
MAIL_PASS=<YOUR_EMAIL_PASSWORD>  

# Authentication and Security
JWT_SECRET=<YOUR_JWT_SECRET>  
FOLDER_NAME=<YOUR_FOLDER_NAME>  

# Cloud Storage (Cloudinary)
CLOUD_NAME=<YOUR_CLOUDINARY_NAME>  
API_KEY=<YOUR_CLOUDINARY_API_KEY>  
API_SECRET=<YOUR_CLOUDINARY_API_SECRET>  

# Payment Gateway (Razorpay)
RAZORPAY_KEY=<YOUR_RAZORPAY_KEY>  
RAZORPAY_SECRET=<YOUR_RAZORPAY_SECRET>  


 Also craete a .env in src 
 REACT_APP_BASE_URL = http://localhost:4000/api/v1

After This:
The server should now be running at localhost:4000.
The frontend (React app) can usually be run separately with the command:
npm run dev
