Black Pearl Tours Website

A modern, full-stack travel and tours web application for Black Pearl Tours — built with React, Node.js, Express, and MongoDB. The platform allows users to explore tours, submit bookings and quotes, send feedback, and contact the company.
 
🚀 Features

🌐 Frontend
•	Responsive, interactive UI built with React
•	Google Maps integration using @react-google-maps/api
•	Booking, Quote, and Contact forms via Formspree
•	Chatbot feature for user support
•	Admin dashboard for managing bookings, messages, gallery, and settings

⚙️ Backend (Black_pearl-backend)
•	Express.js server with RESTful API routes
•	MongoDB Atlas for storing users, bookings, quotes, feedback, messages, reviews, gallery albums, and images
•	JWT Authentication for secure login and protected routes
•	Cloudinary integration for media uploads
•	Loyalty system via loyaltyService.js
•	Middleware for auth and error handling
🗂️ Black Pearl Website/
•	├── Black_pearl-backend/
•	│   ├── middleware/
•	│   │   └── auth.js
•	│   ├── models/
•	│   │   ├── Booking.js
•	│   │   ├── quote.js
•	│   │   ├── User.js
•	│   │   ├── Feedback.js
•	│   │   ├── Message.js
•	│   │   ├── Review.js
•	│   │   ├── GalleryAlbum.js
•	│   │   ├── Image.js
•	│   │   ├── ImageUploadRequest.js
•	│   │   └── PendingImage.js
•	│   ├── routes/
•	│   │   ├── auth.js
•	│   │   ├── bookingRoutes.js
•	│   │   ├── bookings.js
•	│   │   ├── loyalty.js
•	│   │   ├── profile.js
•	│   │   ├── quotes.js
•	│   │   ├── messageRoutes.js
•	│   │   ├── feedbackRoutes.js
•	│   │   ├── uploadRoutes.js
•	│   │   ├── userRoutes.js
•	│   │   ├── galleryRequests.js
•	│   │   ├── gallery.js
•	│   │   ├── terms.js
•	│   │   └── imageRoutes.js
•	│   ├── scripts/
•	│   │   └── createAdmin.js
•	│   ├── services/
•	│   │   └── loyaltyService.js
•	│   ├── uploads/review/
•	│   ├── node_modules/
•	│   ├── .env
•	│   ├── package.json
•	│   ├── package-lock.json
•	│   └── server.js
•	│
•	├── black_pearl-frontend/
•	│   ├── node_modules/
•	│   ├── public/
•	│   ├── src/
•	│   │   ├── chatbot/
•	│   │   ├── Components/
•	│   │   ├── Pages/
•	│   │   ├── Services/
•	│   │   ├── Styles/
•	│   │   ├── utils/
•	│   │   └── index.js / App.js / App.jsx / etc.
•	│   ├── package.json
•	│   ├── package-lock.json
•	│   └── README.md
•	│
•	├── package.json
•	└── .gitignore

Tech Stack
Layer	Technology
Frontend	React, React Router, Axios, Recharts, Google Maps API, Chatbot
Backend	Node.js, Express, JWT, Nodemailer, Cloudinary, Multer, MongoDB, Mongoose
Database	MongoDB Atlas
Authentication	JWT (JSON Web Token)
Dev Tools	Nodemon, ESLint, React Scripts
Deployment	Render (Backend), Netlify/Vercel (Frontend)
🔑 Environment Variables

Create a .env in Black_pearl-backend and include the following:
# Database
MONGODB_URI=

# JWT
JWT_SECRET=
JWT_EXPIRES_IN=
JWT_COOKIE_EXPIRE=

# Server
PORT=
CLIENT_URL=
NODE_ENV=

# Email (Ethereal)
EMAIL_HOST=
EMAIL_PORT=
EMAIL_USER=
EMAIL_PASSWORD=
EMAIL_FROM=
CONTACT_EMAIL=
FRONTEND_URL=
Frontend
REACT_APP_GOOGLE_MAPS_API_KEY=
REACT_APP_API_URL=
⚡ Setup & Installation

1️⃣ Clone repository
git clone https://github.com/<your-username>/BlackPearlWebsite.git
cd Black_Pearl_Website
2️⃣ Backend setup
cd Black_pearl-backend
npm install
npm run dev   # Starts server with nodemon
3️⃣ Frontend setup
cd ../black_pearl-frontend
npm install
npm start     # Starts React app
🧩 API Overview

Key backend endpoints:
Method	Endpoint	Description
POST	/api/users/register	Register a new user
POST	/api/users/login	Login and receive JWT
GET	/api/bookings	Fetch all bookings
POST	/api/bookings	Create a booking
GET	/api/quotes	Fetch quotes
POST	/api/feedback	Submit feedback
POST	/api/messages	Send contact message
GET	/api/reviews	Fetch reviews
…	/api/gallery	Manage albums & images

📨 Form Handling
•	Contact, Quote, and Booking forms use Formspree or direct backend integration.
•	Admin receives submissions via email for follow-up.
 
☁️ Cloudinary Integration
•	Images uploaded to Cloudinary via multer-storage-cloudinary.
•	Gallery management and pending image approval are supported.
 
🔒 Authentication
•	Users authenticate via JWT.
•	Middleware protects routes and verifies user roles.

🤝 Contributors
Name	Role
Linda	Project Manager / Business Analyst
Anele	Backend Developer, Database Manager, API Integration Specialist
Ntokozo	Client Relationship Manager / Backend
Lwandle	Frontend Lead / Full-Stack Contributor
Olebogeng	Backend Development


🧪 Testing
•	Use Postman or Insomnia to test APIs at:

🌍 Deployment
•	Backend: Render
•	Frontend: Netlify / Vercel
•	Database: MongoDB Atlas
 
📌 Future Enhancements
•	Restaurant detail page via Google Maps markers
•	Loyalty points system integration on the frontend
•	Chatbot enhancements with AI-powered responses
•	Admin analytics dashboard
 
🪶 License
•	MIT License — free to use, modify, and distribute with proper attribution.


