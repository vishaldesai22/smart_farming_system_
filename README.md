# smart_farming_system_
📌 GitHub Project Description
🌾 Smart Farming Alert System

A Flask-based web application that helps farmers receive real-time weather-based alerts to protect crops from sudden climate changes. The system automatically monitors environmental conditions and sends notifications in Marathi, enabling timely decision-making.

🚀 Key Features
👨‍🌾 Admin Dashboard
Add, update, and delete farmers
Send alerts (individual or broadcast)
View alert history
🌦️ Weather Monitoring
Fetches real-time weather data using API
Uses latitude & longitude for accurate location tracking
⏱️ Automatic Alerts
Scheduler runs every 5 minutes
Detects climate changes (temperature, humidity)
Sends alerts automatically
🌱 Season-Based Intelligence
Different alerts for Summer, Monsoon, and Winter
Crop-specific alert logic
📧 Email Notification System
Sends alerts via Gmail SMTP
Supports bulk and individual messaging
Marathi language alerts
👤 Farmer Dashboard
Login system for farmers
View crop details and alerts

🛠️ Tech Stack
Backend: Python, Flask
Frontend: HTML, Tailwind CSS
Database: SQLite
API: OpenWeather API
Scheduler: Python schedule library
Email Service: SMTP (Gmail)


📊 System Workflow
Admin → Add Farmer → Store in Database
                        ↓
                Scheduler (5 min)
                        ↓
              Fetch Weather Data
                        ↓
             Check Alert Conditions
                        ↓
              Send Email Alerts
                        ↓
              Farmer Dashboard


📁 Project Structure
smart_farming_system/
│
├── app.py
├── config.py
├── models/
├── routes/
├── services/
├── templates/
├── static/
└── database/


⚙️ How to Run
git clone <your-repo-link>
cd smart_farming_system
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python app.py

Open:

http://127.0.0.1:5000



🔐 Configuration

Update config.py:

EMAIL = "your_email@gmail.com"
APP_PASSWORD = "your_app_password"
WEATHER_API_KEY = "your_api_key"
⚠️ Limitations
Uses email instead of SMS/WhatsApp
Basic authentication system
Depends on internet connectivity


🚀 Future Improvements
SMS & WhatsApp alerts
Mobile application
AI-based crop recommendations
Real-time push notifications
🎯 Conclusion

