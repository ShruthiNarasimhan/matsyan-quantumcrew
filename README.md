### 🐟 Matsyan – QuantumCrew

### Smart Coastal Copilot for Overfishing Alert System

A hackathon project aimed at promoting sustainable fishing practices through technology. Built with Python (Flask), Node.js, HTML, CSS, and JavaScript.

## 🚀 Problem Statement

Overfishing threatens marine biodiversity and the livelihood of coastal communities. There is no real-time mechanism for:

* Monitoring fishing activities
* Identifying overfishing zones
* Sending alerts or warnings to stakeholders

## 💡 Our Solution

We present a Smart Coastal Copilot that:

* Allows fishermen to log catch data
* Calculates CPUE (Catch per Unit Effort) and determines if the zone is overfished
* Automatically sends an SMS warning to fishermen if they exceed limits
* Enables officers to track logs and identify trends
* Allows authorities to audit logs and download records

## 👥 Roles and Features

### 1. Fisherman

* Login (username only)
* Enter catch details (weight, effort, region)
* Geolocation detection (via browser)
* CPUE calculation & color zone alert:

  * 🟢 Green Zone: Safe
  * 🟠 Orange Zone: Monitor
  * 🔴 Red Zone: Overfishing
* SMS alert if Red Zone
* Data is saved to the backend (JSON file)

### 2. Officer

* Login with phone number
* View logs by Fisher ID
* CPUE trends using Chart.js
* Zone alerts for specific IDs

### 3. Authority

* Login with phone number
* View all logs across fishers
* Download logs as .txt file


## 🛠️ Tech Stack
 _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
| Layer              | Tools Used                        |
| ------------------ | --------------------------------- |
| Frontend           | HTML, CSS, JavaScript             |
| Backend            | Python (Flask), Node.js + Express |
| Database           | JSON File (local simulation)      |
| Charts             | Chart.js                          |
| SMS Alerts         | Twilio API                        |
| Hosting (optional) | Replit/Vercel                     |
 _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 


## 📦 Folder Structure

```plaintext SMART-CREW/ │ ├── __pycache__/ │ ├── data/ │ ├── logs.json │ └── users.json │ ├── static/ │ ├── chart.js │ ├── login_background.gif │ ├── ocean_background.gif │ ├── ocean.gif │ ├── script.js │ └── style.css │ ├── templates/ │ ├── auth.html │ ├── authority.html │ ├── fisherman.html │ ├── index.html │ ├── login.html │ ├── officer.html │ ├── preview.html │ ├── select.html │ └── signup.html │ ├── app.py ├── last_sms_sent.json ```

## 🔧 How to Run Locally

1. Clone the repo:

   git clone https://github.com/YourName/matsyan-quantumcrew.git
   
2. Setup Python Flask backend:

   cd project
   pip install flask
   python app.py

3. Setup Node.js backend (for data API):

   cd project
   npm install express
   node index.js

4. Go to your browser:

   http://localhost:5000

## 🔒 Twilio SMS Setup (optional)

1. Create a Twilio account and get:

   * Account SID
   * Auth Token
   * Twilio phone number

2. Add them to `sms_alert.py`:

   account_sid = "your_sid"
   auth_token = "your_token"
   from_number = "+1xxxxxxxxxx"

## 📽️ Demo Video

🎬 Watch our 3-minute demo on YouTube:
[📺 Click here to view](https://youtube.com/your-demo-link)

---

## 👨‍💻 Team Quantum Crew

* Shruthi N
* Sibi Sushan E
* Sruthika R
* Tharani A S

## 📄 License

This project is built for educational and hackathon purposes only.
