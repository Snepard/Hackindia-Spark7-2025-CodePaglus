# 📚 Decentralized Attendance App (DAA)

A blockchain-powered decentralized attendance tracking system that ensures tamper-proof records, real-time access, and high security using smart contracts and geolocation verification.

---

## 🚀 Project Overview

DAA is a secure and decentralized solution to traditional attendance systems. It aims to eliminate the risks of proxy attendance, tampering, and centralized control by leveraging blockchain technology. Designed for educational institutions and corporate organizations, this app offers a modern approach to attendance marking with transparency and decentralization at its core.

---

## 🧩 Features

- ✅ **Decentralized Attendance Records** – All records are stored on the blockchain, making them immutable and transparent.
- 📍 **Geolocation Verification** – Ensures that students/employees mark attendance only within the designated area.
- 🦊 **MetaMask Integration** – Enables users to connect their wallets and verify identity.
- 🔐 **Smart Contracts on Telos Blockchain** – Attendance logic is securely handled via Solidity-based smart contracts.
- 📊 **Supabase Backend** – Stores additional data like user profiles, time logs, thresholds, and admin flags.
- 🖥️ **React.js Frontend with Vite** – Fast and modern frontend for a smooth user experience.

---

## 🏗️ Tech Stack

| Layer | Technology |
|-------|------------|
| Frontend | React.js + Vite + Tailwind CSS |
| Blockchain | Solidity + Telos Testnet |
| Wallet | MetaMask |
| Backend | Supabase (PostgreSQL + Auth + Storage) |
| Location | HTML5 Geolocation API |
| Deployment | Vercel (Frontend) + Telos Explorer (Contracts) |

---

## 🔁 Workflow

1. **User signs in** using MetaMask.
3. On click of `Mark Attendance`, **geolocation is captured**.
4. Smart contract checks:
   - ✅ Location within range
   - ✅ Not marked today already
5. Attendance is logged **on-chain**.
6. Supabase stores attendance status for admin viewing/reporting.

---

## 📦 Project Structure
│
├── /client # Frontend - React app
│ ├── /src
│ │ ├── components/
│ │ ├── pages/
│ │ ├── hooks/
│ │ └── utils/
│ └── index.html
│
├── /contracts # Solidity smart contracts
│ └── Attendance.sol
│
├── /backend # Supabase integration logic
│ └── supabase.js
│
└── README.md


---

## ⚙️ Smart Contract Details

- **Language:** Solidity
- **Functions:**
  - `markAttendance(address user, string memory date)`
  - `hasMarked(address user, string memory date)`
  - `getAttendance(address user)`
- **Chain:** Telos Testnet

---

## 🛠️ Setup Instructions

### 📌 Prerequisites

- Node.js & npm
- MetaMask installed
- Supabase account
- Telos testnet account & wallet

### 📥 Installation

```bash
# Clone repo
git clone https://github.com/your-username/daa-app.git
cd daa-app

# Install client dependencies
cd client
npm install

# Start frontend
npm run dev

🙌 Team & Credits
👨‍💻 Yugal – Full Stack Dev & Blockchain Engineer
👨‍💻 Aryan Balodi – Backend Developer
👨‍💻 Aryan Singh – Frontend Developer & UI Designer
👩‍💻 Sakshi Saini – Frontend Developer & UI Designer


🧠 Special thanks to HackIndia 2025 and Telos for the inspiration and infrastructure.

🤝 Contributing
Pull requests are welcome! If you have any suggestions or improvements, feel free to raise an issue or PR.



