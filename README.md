<div align="center">

  <img src="coffee-logo.png" alt="Aura & Bean Logo" width="100" style="border-radius: 50%;" />

  # ☕ Aura & Bean
  ### Enterprise Coffee Partnership Network & Automated Ops Pipeline

  <p>
    <a href="https://auraandbeans.vercel.app" target="_blank">✨ View Live Demo</a> •
    <a href="#-architecture">🏗️ Architecture</a> •
    <a href="#-features">🚀 Features</a> •
    <a href="#-tech-stack">🛠️ Tech Stack</a>
  </p>

  <p>
    <img src="https://img.shields.io/badge/Status-Production%20Ready-success?style=for-the-badge" alt="Status" />
    <img src="https://img.shields.io/badge/Frontend-Vite%20%2B%20React-blue?style=for-the-badge&logo=react" alt="Frontend" />
    <img src="https://img.shields.io/badge/Backend-Node.js%20%2B%20Express-green?style=for-the-badge&logo=node.js" alt="Backend" />
    <img src="https://img.shields.io/badge/Database-MongoDB%20Atlas-orange?style=for-the-badge&logo=mongodb" alt="Database" />
  </p>
</div>

---

## 🌟 Overview

**Aura & Bean** is a full-stack production-grade B2B web application engineered to bridge corporate tech parks and college campuses with specialty coffee partners. It features an automated 3-tier business logic engine, webhook dispatch synchronization, secure credential authentication, and persistent cloud storage.

---

## 🚀 Key Features

* **Deterministic 3-Tier Classification Engine:** Automatically processes incoming footfall metrics to classify locations into **Flagship Space** ($\ge$ 1,000 footfall), **Campus Partner** (300–999 footfall), or **Micro-Kiosk** ($<$ 300 footfall).
* **Automated Webhook & Sync Workflow:** Flagship spaces auto-sync on ingestion, while operational reviews remain safely staged in a Pending queue until manually dispatched.
* **Full-Stack Cloud Persistence:** Powered by a React (Vite) frontend, an Express REST backend, and MongoDB Atlas cloud storage.
* **Secure Ops Portal:** Role-based administrative dashboard with encrypted session validation and live analytics.

---

## 🛠️ Tech Stack

* **Frontend:** React, TypeScript, Vite, Tailwind CSS, Lucide Icons
* **Backend:** Node.js, Express.js, Mongoose, CORS, Dotenv
* **Database:** MongoDB Atlas (Cloud Cluster)
* **Deployment & CI/CD:** Vercel (Frontend CI/CD) & Render (Backend Web Service)

---

## 🏗️ Architecture & Data Flow

```text
[ React Frontend (Vercel) ] 
       │
       ▼ (HTTP Requests / REST API via VITE_API_URL)
[ Express.js Backend (Render) ]
       │
       ▼ (Mongoose ODM)
[ MongoDB Atlas Cloud Database ]
