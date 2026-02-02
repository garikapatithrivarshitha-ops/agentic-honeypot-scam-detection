# agentic-honeypot-scam-detection
Agentic Honeypot Scam Detection System that automatically detects scam messages, engages scammers via an autonomous honeypot, and extracts threat intelligence such as UPI IDs, phone numbers, links, and domains using AI-assisted analysis.


🛡️ Agentic Honeypot Scam Detection System

An AI-assisted cybersecurity system that **detects scam messages**, **autonomously engages scammers using a honeypot**, and **extracts actionable threat intelligence** such as UPI IDs, phone numbers, links, and domains — all presented through a professional web dashboard.


## 📌 Problem Statement
Online scams through SMS, WhatsApp, email, and UPI-based fraud are rapidly increasing.  
Most existing solutions focus only on **detecting scams**, but they do not actively **interact with scammers** to gather intelligence.

This project introduces an **Agentic Honeypot Scam Detection System** that not only detects scams but also **engages scammers safely** to collect valuable threat intelligence.


## 🎯 Objectives
- Detect scam messages using AI-assisted rules
- Assign confidence-based scam scores
- Automatically trigger a honeypot for high-risk messages
- Engage scammers without exposing real users
- Extract and store threat intelligence
- Display insights via a professional dashboard


## 🧠 System Architecture
**Workflow:**
1. User submits a suspicious message
2. Scam Analyzer evaluates the message
3. A scam score is generated
4. If score ≥ threshold → Honeypot is activated
5. Honeypot interacts autonomously with the scammer
6. Intelligence is extracted and stored
7. Results are shown in the dashboard


## ✨ Key Features

### 🔍 Scam Analyzer
- Rule-based AI detection
- Scam type classification
- Confidence scoring
- Auto-trigger threshold control

### 🎭 Agentic Honeypot
- Automatic scammer engagement
- Safe conversational strategy
- Intelligent stopping conditions
- No OTP / payment sharing

### 📊 Threat Intelligence
- UPI ID extraction
- Phone number detection
- Link and domain extraction
- Memory matching for repeated scams

### 🎨 User Interface
- Dark professional cybersecurity theme
- Login / Logout support
- Clear, readable analytics view


## 🛠️ Technology Stack

**Backend**
- Python
- FastAPI
- Rule-based AI logic
- Honeypot state machine

**Frontend**
- Streamlit
- Custom CSS (professional dark theme)

**Tools**
- REST APIs
- JSON-based intelligence storage
- Git & GitHub


## 🧪 Sample Scam Messages
Your reward points are expiring today.
Pay ₹99 now to activate redemption.
Send payment to rewardsverify@upi.

Your courier is on hold due to address issue.
Pay ₹25 via UPI to reschedule delivery.


## ✅ Sample Legitimate Messages (Not Scam)
Your Amazon order has been delivered successfully.

Reminder: Assignment submission deadline is Friday.


## ▶️ How to Run the Project

### 1️⃣ Start Backend
uvicorn app.main:app --reload --port 8000
2️⃣ Start Frontend
streamlit run frontend/dashboard.py
📁 Project Structure
agentic-honeypot-scam-detection/
│
├── app/
│   ├── main.py
│   ├── classifier.py
│   ├── honeypot.py
│   └── intelligence.py
│
├── frontend/
│   └── dashboard.py
│
├── .gitignore
├── README.md
└── requirements.txt
