# 🛡️ SecureAid Bot

**AI-Based Disaster Communication and Blockchain-Based Transparent Fundraising System**  

SecureAid Bot is a full-stack application designed to provide real-time disaster alerts and enable secure, transparent fundraising. The system combines an AI-powered chatbot for emergency communication with blockchain-based donation tracking, ensuring every transaction is secure, immutable, and fully traceable.  

---

## ✨ Features

- **AI Chatbot for Disaster Alerts:** Provides fast, location-based alerts and guidance during emergencies.  
- **Email Notifications:** Sends disaster alerts and updates to registered users automatically.  
- **Secure Donations via Blockchain:** Uses Solidity smart contracts to collect and record donations securely.  
- **Transparent Donation Tracking:** Every donation and withdrawal is recorded on-chain for auditability.  
- **Admin Dashboard:** Monitor donations, withdrawals, and user activity in real time.  
- **Real-Time Fundraising Stats:** Displays total funds raised, contract balance, and donor details.  
- **MetaMask Integration:** Allows safe and easy user transactions on Ethereum/Polygon networks.  
- **User-Friendly Interface:** Dark/light mode and clear navigation for accessibility.  

---

## 🛠️ Tech Stack

| Layer | Technologies |
|-------|---------------|
| **Frontend** | React.js, HTML, CSS, Tailwind CSS |
| **Backend** | Node.js / Flask, REST APIs |
| **AI** | NLP Chatbot (LLM/API-based), Weather & Disaster APIs |
| **Blockchain** | Solidity, Ethereum / Polygon, MetaMask, Web3.js / Ethers.js |
| **Database** | MongoDB / PostgreSQL |
| **Dev Tools** | Hardhat / Remix, Truffle, Docker, Postman, VS Code |

---
### 📝 Paper

**Title:** SecureAid Bot — AI-Based Disaster Communication and Blockchain-Based Transparent Fundraising System  

**Overview:**  
SecureAid Bot combines AI and Blockchain to enhance disaster management. It features an AI chatbot for real-time, personalized alerts and a blockchain-based donation system for secure, transparent contributions. An admin dashboard allows NGOs and government agencies to track donations and coordinate relief efficiently.

**Highlights:**  
- AI chatbot for hyper-local disaster alerts  
- Blockchain fundraising via smart contracts  
- Admin dashboard for real-time monitoring  
- Supports web/mobile, text/voice, and multi-language accessibility  

**Objective:** Provide a secure, decentralized platform for real-time disaster communication and transparent fundraising.

**Scope:** Pre-emergency alerts, automatic donations, real-time monitoring, and scalable system for wide accessibility.  

**Certificate:**  
<img src="https://github.com/codeypas/SecureAID-Bot/blob/8572347d29f4521f8fa6118588e0ba464323ce4d/SecureAid.jpg" width="50%" alt="Clipboard Tab"/>

---

**Read full paper:** [SecureAid Bot Paper](https://www.ijisrt.com/secureaid-bot)

---

**Read full Report:** [SecureAid Bot Report](https://drive.google.com/file/d/1Jdff1c5WKowq0xKHcVPzAGGeDjDaB_vo/view?usp=sharing)
---

## 🚀 Getting Started

### Prerequisites

- Node.js (v18+)  
- Python 3.10+  
- MetaMask  
- Ganache (local blockchain)  
- MongoDB or PostgreSQL (local or Docker)  
- Docker (optional, for chatbot & email services)

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/codeypas/secure-aid-bot.git
cd secure-aid-bot

```
### Setup & Installation

# 1️⃣ Install Dependencies

```bash

# Backend
cd backend
npm install

# Frontend
cd ../frontend
npm install

# 2️⃣ Start Local Blockchain
# Open Ganache → click “QUICKSTART” and keep it running

# 3️⃣ Deploy the Smart Contract
cd ../
truffle migrate --network development --reset
# Copy the deployed contract address from the terminal for frontend configuration

# 4️⃣ Configure Frontend
# In frontend/src/App.jsx:
# - Paste contract address into `contractAddress`
# - Paste ABI from build/contracts/Donation.json into `contractABI`

# 5️⃣ Configure and Run Backend
cd backend
touch .env
# Add MongoDB connection string to .env
echo "MONGO_URI=mongodb://localhost:27017/secureaid" >> .env

# Start MongoDB (Mac example)
brew services start mongodb-community@7.0

# Run backend server
node server.js

# 6️⃣ Run Frontend
cd ../frontend
npm start
# Open http://localhost:3000 in your browser

# 7️⃣ Run Chatbot & Email Services
cd ../
docker-compose up -d

# Setup Python virtual environment for Flask
cd backend
python -m venv venv
source venv/Scripts/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt

# Initialize Flask database
flask db init
flask db migrate
flask db upgrade

# Start Flask server
python run.py

```

### Application URLs

- **Flask backend:** http://localhost:5000  
- **PostgreSQL database:** localhost:5432  
- **PgAdmin interface:** http://localhost:5050  
- **Frontend:** http://localhost:3000  
- **Chatbot & Email services:** running via Docker  

---


### 🖼 Screenshots

**Home Page / Dashboard**  
<img src="https://github.com/codeypas/SecureAID-Bot/blob/455b4dcf756b30d21b5ecf02efafb17046814760/M_P-images/User-Dashboard.png" width="60%" alt="Home Page Screenshot" />

**Chatbot Interface**  
<img src="https://github.com/codeypas/SecureAID-Bot/blob/455b4dcf756b30d21b5ecf02efafb17046814760/M_P-images/ChatInterface.png" width="60%" alt="Chatbot Screenshot" />

**Donation & Blockchain Dashboard**  
<img src="https://github.com/codeypas/SecureAID-Bot/blob/455b4dcf756b30d21b5ecf02efafb17046814760/M_P-images/Screenshot%202025-11-10%20at%2021.35.23.png" width="60%" alt="Donation Dashboard Screenshot" />

**Blockchan Admin Dashboard**  
<img src="https://github.com/codeypas/SecureAID-Bot/blob/455b4dcf756b30d21b5ecf02efafb17046814760/M_P-images/Screenshot%202025-11-10%20at%2021.37.03.png" width="60%" alt="Admin Panel Screenshot" />

---

### 🌐 Connect & Contribute

📌 [GitHub Profile](https://github.com/codeypas)  
📧 Contact: bjbestintheworld@gmail.com  
🔗 [Portfolio](https://bijayadhikari28.com.np/) 


Pull requests are welcome! For major changes, please open an issue first to discuss your idea.


---
### 🏆 Motto  
**“Build. Learn. Repeat.”**
---


⭐ **If you find this project helpful, give it a star on GitHub!**
