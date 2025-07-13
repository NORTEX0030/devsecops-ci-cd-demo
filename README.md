<h1 align="center">
  ⚙️ DevSecOps CI/CD Pipeline for Tic Tac Toe Game 🎮
</h1>

<p align="center">
  <img src="https://img.shields.io/github/deployments/NORTEX0030/devsecops-ci-cd-demo/github-pages?label=Deployment&logo=github&style=flat-square" />
  <img src="https://img.shields.io/github/workflow/status/NORTEX0030/devsecops-ci-cd-demo/CI/CD%20Pipeline/main?logo=githubactions&style=flat-square" />
  <img src="https://img.shields.io/github/issues/NORTEX0030/devsecops-ci-cd-demo?style=flat-square" />
  <img src="https://img.shields.io/github/stars/NORTEX0030/devsecops-ci-cd-demo?style=social" />
</p>

---

###  🔄 DevSecOps CI/CD Pipeline Workflow (Horizontal View)
```bash
[ Developer Pushes Code ]
            │
            ▼
[ GitHub Actions Triggered ]
            │
            ▼
[ Unit Testing (npm test) ]
            │
            ▼
[ Linting (ESLint) ]
            │
            ▼
[ Build App (npm run build) ]
            │
            ▼
[ Docker Build & Push to GHCR ]
            │
            ▼
[ Trivy Security Scan ]
            │
            ▼
[ Update Kubernetes Deployment ]
```

### 🎮 Project Overview

This is a fully responsive **Tic Tac Toe game** built using modern web technologies and enhanced with a **DevSecOps CI/CD Pipeline** using:

- GitHub Actions
- Docker
- Kubernetes
- Trivy (Security Scan)
- GHCR (GitHub Container Registry)

---

### 🧩 Features

- 🧠 **Smart game logic** with turn-based play
- ✅ **Highlights winning combinations**
- 📊 **Score tracking** for Player X, O, and Draws
- 📜 **Game history** with timestamps
- 🔁 **Reset functionality** for both game & scores
- 📱 **Fully responsive** and mobile-friendly

---

### 🚀 Technologies Used

- ⚛️ React 18
- ⌨️ TypeScript
- 🎨 Tailwind CSS
- 🧩 Lucide Icons
- 🔐 GitHub Actions + Trivy for CI/CD & Security
- 🐳 Docker + Kubernetes + GHCR

---

### 📁 Project Structure

```bash
src/
├── components/
│   ├── Board.tsx        # Game board
│   ├── Square.tsx       # Each square
│   ├── ScoreBoard.tsx   # Score tracker
│   └── GameHistory.tsx  # Game logs
├── utils/
│   └── gameLogic.ts     # Game logic
├── App.tsx              # Root component
└── main.tsx             # Entry point
 ```

### 🧠 Game Logic
- X always starts first

- Players take turns placing marks

- The first with 3 in a row (horizontal, vertical, diagonal) wins

- If the board is full and no winner → Draw

- Winning line is visually highlighted


###  🛠️ Getting Started
✅ Prerequisites
```bash
Node.js (v14+)

npm or yarn
 ```

 🔧 Installation
```bash
 git clone https://github.com/NORTEX0030/devsecops-ci-cd-demo.git
cd devsecops-ci-cd-demo

npm install   # or yarn
 ```

 🚀 Run Locally
```bash
 npm run dev   # or yarn dev
```

Visit: http://localhost:5173

📦 Production Build
```bash
npm run build   # or yarn build
```
The output will be in the dist/ directory.
