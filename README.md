 Crop Insurance Verification System

This is my final year project – a platform built to make the crop insurance process smoother for both farmers and administrators.  
Farmers can easily submit and track their claims, while admins get tools to verify, approve, or reject them.  

I’ve also added role-based authentication, email updates, and even an AI chatbot (powered by Gemini) to guide users through the system.

---

## ✨ What it does

- 👨‍🌾 **For Farmers**
  - Submit crop insurance claims online
  - Upload documents directly
  - Check claim status anytime  

- 🏢 **For Admins**
  - Review and verify claims
  - Approve or reject with comments
  - Manage farmer records  

- 🔐 **Security**
  - JWT-based authentication
  - Separate dashboards for farmers and admins  

- 🤖 **AI Chatbot**
  - Helps answer common questions
  - Assists farmers during claim submission  

- 📩 **Email Updates**
  - Farmers get instant notifications about claim status  

---

## 🛠 Tech Stack

**Frontend (React + Tailwind)**  
- React.js for UI  
- Tailwind CSS for styling  
- Axios for API calls  
- React Router for navigation  

**Backend (Django REST Framework)**  
- Django REST Framework (DRF)  
- PostgreSQL  
- JWT Authentication  
- Django ORM  

**Extras**  
- Gemini API (Chatbot)  
- SMTP (Email notifications)  

---

## 📂 How the project is structured

crop-insurance-system/
│
├── crop_insurance_backend/ # Django backend (APIs, authentication, claims mgmt)
│ ├── accounts/ # Login, registration, roles
│ ├── claims/ # Claim submission & verification
│ ├── chatbot/ # Gemini chatbot integration
│ └── settings.py # Configurations
│
├── farm-claim-connect-main/ # React frontend
│ ├── src/
│ │ ├── components/ # Reusable UI components
│ │ ├── pages/ # Farmer & Admin dashboards
│ │ ├── services/ # Axios API setup
│ │ └── App.js # Main entry point
│
└── README.md

yaml
Copy code

---

## 🚀 Getting started

### Backend (Django)
```bash
cd crop_insurance_backend
python -m venv venv
venv\Scripts\activate   # for Windows
source venv/bin/activate   # for Linux/Mac

pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
Frontend (React)
bash
Copy code
cd farm-claim-connect-main
npm install
npm start
Frontend runs on: http://localhost:3000

Backend runs on: http://localhost:8000/api/

📸 Screenshots (to add later)
Farmer Dashboard

Admin Dashboard

Claim form

Chatbot demo

💡 What’s next
Support for multiple languages

Analytics dashboard for admins

Cloud deployment (AWS/GCP/Azure)

Mobile version
