# 🌾 Smart Farming Alert System

A Flask-based web application that monitors real-time weather conditions and automatically sends crop-specific alerts to farmers. The system helps farmers take timely actions and reduce crop damage caused by sudden climate changes.

---

## 🚀 Features

### 👨‍💼 Admin Panel
- Add, update, and delete farmers
- Send alerts (individual or broadcast)
- View alert history

### 👨‍🌾 Farmer Dashboard
- Secure login system
- View crop details and weather data
- Receive alerts in Marathi

### 🌦️ Weather Monitoring
- Uses OpenWeather API
- Fetches real-time weather using latitude & longitude

### ⏱️ Automatic Alert System
- Runs every 5 minutes using scheduler
- Detects sudden climate changes
- Sends automated alerts

### 🌱 Smart Logic
- Season-based alerts (Summer / Monsoon / Winter)
- Crop-specific conditions

### 📧 Email Notification
- Gmail SMTP integration
- Supports bulk and individual alerts

---

## 🛠️ Tech Stack

- **Backend:** Python, Flask  
- **Frontend:** HTML, Tailwind CSS  
- **Database:** SQLite  
- **API:** OpenWeather API  
- **Scheduler:** schedule library  
- **Email:** SMTP (Gmail)

Admin → Add Farmer → Database
↓
Scheduler (5 min)
↓
Fetch Weather Data
↓
Check Conditions
↓
Send Alerts
↓
Farmer Dashboard


---

## 📁 Project Structure


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


---

## ⚙️ Installation & Setup

### 1. Clone Repository
```bash
git clone https://github.com/your-username/smart-farming-system.git
cd smart_farming_system
2. Create Virtual Environment
python -m venv venv
venv\Scripts\activate
3. Install Dependencies
pip install -r requirements.txt
4. Run Application
python app.py

Open in browser:

http://127.0.0.1:5000
🔐 Configuration

Update config.py:

EMAIL = "your_email@gmail.com"
APP_PASSWORD = "your_app_password"
WEATHER_API_KEY = "your_api_key"
⚠️ Limitations
Uses email instead of SMS/WhatsApp
Basic authentication system
Depends on internet connection
🚀 Future Improvements
SMS & WhatsApp alerts
Mobile app version
AI-based crop prediction
Push notifications
🎯 Conclusion

This system provides a smart solution for farmers by automating weather-based alerts and improving decision-making for crop protection.

👨‍💻 Author

Vishal Desai

## 📊 System Workflow
