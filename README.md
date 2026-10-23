# Online Donation & Charity Platform

A MERN-stack student project that connects donors with charitable causes.

## Features in this starter
- Responsive React homepage with charity campaign cards
- Express REST API
- MongoDB/Mongoose campaign model and API routes
- Demo campaign fallback when MongoDB is not configured
- Clear separation between frontend and backend

## Technology
MongoDB, Express.js, React, Node.js, Vite, CSS.

## Project structure
```text
online-donation-charity-platform/
├── frontend/
│   ├── src/
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   └── index.css
│   ├── index.html
│   ├── package.json
│   └── vite.config.js
├── backend/
│   ├── models/Campaign.js
│   ├── routes/campaignRoutes.js
│   ├── .env.example
│   ├── package.json
│   └── server.js
├── .gitignore
├── package.json
└── README.md
```

## Requirements
- Node.js 20.19+ or 22.12+
- npm
- MongoDB Atlas account (optional for the demo; required to persist campaigns)

## Run locally
Open a terminal in the project root:

```bash
npm install
npm run install:all
```

Copy `backend/.env.example` to `backend/.env`. Set `MONGO_URI` if you want to use MongoDB. Do not commit `.env`.

Start both applications:

```bash
npm run dev
```

Frontend: http://localhost:5173  
Backend health check: http://localhost:5000/api/health  
Campaign API: http://localhost:5000/api/campaigns

## Important notes
- The sample campaign amounts and content are demonstration data, not verified real fundraisers.
- This starter does not process real donations or payments. The Donate buttons are demo interactions.
- Before real deployment, add authentication, admin authorization, input validation, payment verification, rate limiting, and privacy/security review.
