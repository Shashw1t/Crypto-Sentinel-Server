# Crypto-Sentinel-Server

#De-anonymizing Blockchain to Combat Illicit Crypto Activity

A fullstack B2G crypto wallet de-anonymization platform designed to identify and trace illegal transactions on the dark web. Built with a combination of real-time scraping, graph analytics, and transformer-based fraud detection models, Crypto Sentinels empowers law enforcement to monitor and investigate suspicious blockchain activity with enriched KYC metadata.

---

## ⚙️ Tech Stack

| Layer          | Tech                                                                 |
|----------------|----------------------------------------------------------------------|
| Frontend       | React.js, Electron                                                   |
| Backend        | Node.js, Express.js, MongoDB, Redis                                  |
| ML/AI Layer    | BERT4CRYPTO (Transformer model), TensorFlow                          |
| Data Pipeline  | Python, BeautifulSoup, Requests, Tor Network Scraping                |
| DevOps         | AWS EC2, PM2, Nginx, GitHub Actions (CI/CD)                          |
| Visualization  | Force-directed Graphs (D3.js / Cytoscape)                            |
| Data Storage   | MongoDB (NoSQL for wallet metadata), Redis (in-memory for scoring)   |

---

## Demo Screenshots

## System Architecture

> Real-time scraping pipeline feeds data to backend → ML model scores wallets → Visualizer maps wallet networks → Law enforcement dashboard shows flagged activity.


## Key Features

-  **Wallet Risk Scoring** using transformer-based model (BERT4CRYPTO)
-  **Real-time scraping** of dark web forums and pastebins over Tor
-  **Visual Network Graph** of transaction flows and suspicious nodes
-  **KYC-enriched wallet profiles** with external data sources
-  **Flagging & Alerting** engine based on risk score thresholds
-  **Investigation Dashboard** for law enforcement or compliance teams

---

# How It Works

1. **Scraper** pulls data from dark web listings related to wallet addresses.
2. **Transformer model (BERT4CRYPTO)** scores each wallet on risk scale 0–1.
3. **Wallet metadata + transactions** are stored in MongoDB with KYC overlays.
4. **Graph module** maps transaction links between wallets.
5. **Flagged nodes** are displayed in a React/Electron dashboard.
6. **Alerts** are pushed when patterns match known fraud schemas.

---

## 📦 Installation

```bash
# Clone the repo
git clone https://github.com/your-username/crypto-sentinels.git
cd crypto-sentinels

# Setup backend
cd backend
npm install
npm run dev
