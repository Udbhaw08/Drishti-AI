# Drishti – AI-Powered Intelligent Surveillance

Drishti is an AI-driven surveillance and public safety system that converts existing CCTV, drone, and bodycam networks into a real-time **threat detection, lost-person search, and smart alert** platform for large events (like Mahakumbh), campuses, and smart cities. It focuses on **safe and trusted AI** with strong emphasis on low false alerts, human oversight, and ethical deployment.[1][2]

***

## 🔍 Problem Statement

Traditional CCTV is mostly used **after** an incident as evidence. In high-density environments:

- Operators cannot monitor hundreds of live feeds in real time  
- Weapons, suspects, and missing persons disappear into crowds  
- Alerts are slow, fragmented, and often missed  
- Ground staff get vague, delayed information with no unified view  

Drishti solves this by combining **live video AI** with **NFC-based smart alerts** and a **unified safety dashboard**.[2][1]

***

## 🚀 Key Features

- **Real-Time Threat Detection**  
  Detects weapons, suspicious objects, and anomalous behavior across CCTV, drones, and bodycams using state-of-the-art deep learning models (YOLO-based detection, SlowFast-like action recognition).[1]

- **Criminal & Person-of-Interest Flagging**  
  Uses face recognition and person re-identification (ArcFace-style embeddings + clothing + posture) to spot wanted individuals across multiple cameras.[1]

- **Lost & Found (Missing Person Search)**  
  Given a reference image, Drishti searches live and recorded footage using **facial features, clothing, and body pose** to locate missing persons even in dense crowds.[1]

- **NFC-Based Smart Alerts**  
  NFC tags placed at strategic points allow staff/citizens to tap and raise contextual SOS (lost person, threat, PoI). The system auto-attaches location, camera context, and AI insights to an incident card.[2]

- **Unified Safety Dashboard**  
  Web dashboard showing:
  - Live multi-camera grid with AI overlays  
  - Incident timeline (threats, NFC alerts, missing persons)  
  - Heatmaps and search across events and identities  

- **False Alert Reduction & Trusted AI**  
  - Whitelist database of authorized weapon-carrying personnel  
  - Human-in-the-loop review for high-risk decisions  
  - Audit logs, role-based access, DPDP-aligned design[1]

***

## 🧱 Tech Stack

- **Backend:** FastAPI (Python), REST APIs, WebSockets  
- **AI Models:** YOLO (object/weapon detection), ArcFace-style face recognition, person Re-ID, action recognition (SlowFast-style)[1]
- **Computer Vision:** OpenCV, MediaPipe / similar landmark & pose tools  
- **Frontend:** React.js dashboard (live video, alerts, maps)  
- **Database & Infra:** PostgreSQL, Redis, object storage, Docker  

***

## ⚙️ High-Level Architecture

1. Ingest RTSP / video feeds from CCTV, drones, and bodycams  
2. Run AI pipelines (detection, recognition, re-ID, behavior analysis)  
3. Fuse results with whitelist/watchlist and context  
4. Trigger alerts + NFC events → central incident engine  
5. Display everything on a real-time operator dashboard with controls and logs[1]

***

## 🧪 Getting Started (Dev Setup)

1. **Clone the repo**  
   ```bash
   git clone https://github.com/your-username/drishti.git
   cd drishti
   ```

2. **Backend Setup**  
   ```bash
   cd backend
   pip install -r requirements.txt
   uvicorn app.main:app --reload
   ```

3. **Frontend Setup**  
   ```bash
   cd frontend
   npm install
   npm start
   ```

4. **Configure Streams & NFC**  
   - Update `.env` / config with RTSP URLs, API keys, NFC endpoint base URL  
   - Add test video streams or dummy camera sources  

(Adapt these commands to your actual folder structure.)

***

## 📌 Use Cases

- Mass events (Mahakumbh, fairs, festivals) – lost child tracing, crowd threat detection  
- University / corporate campuses – safety, access control, incident tracking  
- Smart cities – integrated city surveillance and command centers[2]

***

## 👥 Team & Credits

Drishti is built by a student AI/full-stack team with experience in **5+ hackathon wins**, focusing on production-grade AI surveillance, FastAPI backends, and React dashboards.[2]

***

Demo video link : https://drive.google.com/file/d/1cMjR3T5IVEEZhz06oLIh2fxDM_sK3OJz/view?usp=drive_link
LANDING PAGE 
<img width="2879" height="1466" alt="Screenshot 2025-10-12 024117" src="https://github.com/user-attachments/assets/8d6b0767-61af-447d-95dc-af359c66802b" />


DETECTED FRAME BY MODEL

![WhatsApp Image 2025-11-04 at 11 08 48 AM](https://github.com/user-attachments/assets/bf7a9032-1d7a-44a9-a588-079b176017cb)




 WEAPON DETECTION
 <img width="1329" height="998" alt="Al and ML enabled video analysis and interpretation" src="https://github.com/user-attachments/assets/1295baa7-7c59-4039-8467-ba51c079778b" />



