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

### 🌐 Connect & Contribute

📌 [GitHub Profile](https://github.com/codeypas)  
📧 Contact: bjbestintheworld@gmail.com  

Pull requests are welcome! For major changes, please open an issue first to discuss your idea.


---
### 🏆 Motto  
**“Build. Learn. Repeat.”**
---


⭐ **If you find this project helpful, give it a star on GitHub!**
