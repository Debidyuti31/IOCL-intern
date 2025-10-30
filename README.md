# Overview
The Smart Security System was developed during my internship at Indian Oil Corporation Limited (IOCL), Guwahati Refinery, under the mentorship of Mr. Prakash Kumar Sinha (Senior Manager – IS Department).
It enhances workplace safety by integrating QR-based access control, real-time face recognition, and safety gear detection to ensure compliance and streamline entry/exit monitoring in industrial environments.

# Features
1. *QR Entry Pass Generation* – Generates unique QR codes for secure access control.
2. *Real-Time Face Recognition* – Verifies personnel identity using InsightFace (Buffalo1 model) with Euclidean distance matching.
3. *Automated Entry/Exit Tracking* – Logs all check-ins and check-outs, and raises alerts for overtime or unauthorized access.
4. *Safety Gear Detection* – Detects helmets, safety shoes, full suits, and IFR suits using YOLOv11.
5. *Optimized Edge Deployment* – Designed to operate efficiently in real-time on edge devices in industrial setups.

# Tech Stack

## Backend: 
Django – Handles authentication, data processing, and business logic.
Django REST Framework (DRF) – Enables RESTful API communication between backend and frontend.
    
## Computer Vision & Machine Learning
 YOLOv11 – For personal protective equipment (PPE) detection.
 OpenCV & dlib – For QR code decoding and face detection preprocessing.
 InsightFace – Performs accurate facial recognition and verification.

## Frontend:
React.js – Provides an interactive, responsive, and API-integrated user interface.


# Installation & Setup

*1. Clone the Repository*

git clone https://github.com/<your-username>/SmartSecuritySystem.git
cd SmartSecuritySystem

*2. Backend Setup (Django)*

cd backend
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver

*3. Frontend Setup (React.js)*

cd frontend
npm install
npm run dev
