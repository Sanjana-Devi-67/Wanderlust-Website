# Airbnb Clone – MERN Stack Major Project

A full-featured Airbnb clone web application built using the **MERN stack** (MongoDB, Express.js, React.js, Node.js). This project replicates core Airbnb functionalities including user authentication, property listings, booking interactions, and reviews — all structured using the **MVC architecture** for better scalability and maintainability.

---

## Features

### User Management
- Secure user **registration and login** using `Passport.js`
- Manage user **profile details** and authentication sessions
- Role-based actions: **Host** (listing properties) and **Guest** (view & book)

### Property Listings
- Hosts can **create**, **edit**, and **delete** listings
- Each property includes **title**, **description**, **images**, **pricing**, **location (Mapbox)**, and **availability**

### Map Integration
- Integrated with **Mapbox API** for selecting and displaying property locations

### Reviews & Ratings
- Guests can leave **ratings and written reviews** for properties after their stay
- Average ratings displayed per listing

---

## Tech Stack

| Technology     | Role                                |
|----------------|-------------------------------------|
| MongoDB        | NoSQL database                      |
| Express.js     | Backend framework for Node.js       |
| React.js       | Frontend user interface             |
| Node.js        | Server-side JavaScript runtime      |
| Passport.js    | Authentication middleware           |
| Mapbox         | Map integration for listings        |
| HTML/CSS/JS    | UI structure and styling            |


---

## Authentication

- Handled using **Passport.js (Local Strategy)**
- Sessions and secure password storage (via `bcrypt`)
- Middleware to protect routes for **hosts** and **guests**

---

## Mapbox Integration

- Display property locations with markers
- Allow hosts to select location during listing creation
- API key stored in environment variables

---

## Installation & Setup

### Prerequisites

- Node.js and npm
- MongoDB installed locally or cloud DB URI
- Mapbox API key

### Backend Setup (Server)

```bash
cd server
npm install
# Create .env file and add:
# MONGO_URI=your_mongo_uri
# SESSION_SECRET=your_secret_key
# MAPBOX_TOKEN=your_mapbox_token
node app.js


