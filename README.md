# Travel Companion

## Overview
**Travel Companion** is a full-stack web application built to simplify the travel planning process for modern explorers. It allows users to search and manage flights, accommodations, weather forecasts, and destination visuals all in one place. Designed for frequent travelers, vacation planners, and casual tourists, the platform helps users organize and personalize their travel itineraries with ease. The app supports user authentication, secure trip storage, and real-time data integration through multiple APIs.

## Features
- **User Authentication**: Secure account registration, login, logout, and profile editing.
- **Password Reset**: Password reset with security question and answer.
- **Flight Search**: Search flights by origin, destination, and date, and view real-time status updates.
- **Weather Forecast**: Display 5-day weather forecast for selected travel destinations.
- **Accommodation Finder**: Search hotels by city, check-in/out dates, and number of guests. View amenities and pricing.
- **Trip Planner**: Save and manage flights and hotel data into custom trip plans.
- **Destination Visuals**: Display images and descriptions of cities using Pixabay API.
- **Trip Management**: Edit and delete saved trips from a personal planner.
- **Trip Sharing**: Share planned trips via email or a shareable link.
- - **Quick Link Access**: Quick Link Access for solving common issues. 

## Technologies Used
- **Backend**: Node.js, Express.js
- **Frontend**: HTML, CSS, JavaScript (PUG templating engine)
- **Database**: MongoDB
- **Authentication**: Passport.js (local strategy)
- **APIs Integrated**:
  - **Aviationstack API** – Real-time flight data
  - **OpenWeatherMap API** – Weather forecasts
  - **Amadeus API** – Hotel listings and details
  - **Pixabay API** – Destination imagery and descriptions

## Challenges & Solutions
1. Creating a seamless user experience across multiple APIs was one of the biggest challenges. This was addressed by:
- Implementing robust error handling for API failures and timeouts.
- Using async/await for clean and manageable API calls.
- Introducing UI feedback (loading indicators and modals) during data fetching operations.
2. Implementing Password reset functionality was quite tough. This was addresses by:
- Introduced a security question and answer mechanism during user registration.
- When a user forgets their password, they must correctly answer their saved security question.
- This information is securely stored in the database and verified before allowing password updates.
- This method avoids external email services while still offering a layer of user identity verification.

## Future Enhancements
- **Map Integration**: Interactive maps to visualize saved trips geographically.
- **Calendar Sync**: Sync trip plans with Google Calendar or Outlook.
- **User Reviews**: Enable real user ratings and feedback on hotels and destinations.

## Installation & Setup
1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/travel-companion.git
2. **Navigate to the project directory**
   ```bash
   cd capstone-project
3. **Install dependencies**
    ```bash
    npm install
4. **Set environment variables**
   - Create a .env file and add your API keys and MongoDB URI:
   ```bash
   PORT=3000
   
   DBUSER=your_user_name
   DBPWD=your_password
   DBNAME=your_database_name
   DBHOST=your_host_name
   
   SESSION_SECRET=your_session_secret
   SALT=your_salt_key
   
   AVIATION_API_KEY=your_aviationstack_key
   WEATHER_API_KEY=your_openweathermap_key
   AMADEUS_API_KEY=your_amadeus_key
   PIXABAY_KEY=your_pixabay_key
   
   AVIATION_API_URL=your_aviationstack_url
   WEATHER_API_URL=your_openweathermap_url
   AMADEUS_API_URL=your_amadeus_url
   PIXABAY_URL=your_pixabay_url
5. **Start the server**
   ```bash
   npm start or npm run dev
6. **Open in browser**
   ```bash
   http://localhost:3000
   
---
**Work Done By**:
Jinal Patel


