<p align="center">
  <h1>AI-Finance Dashboard</h1>
</p>

<p align="center">
  <a href="#"><img src="https://img.shields.io/badge/status-production-2ea44f" alt="status"/></a>
  <a href="#"><img src="https://img.shields.io/badge/license-MIT-blue" alt="license"/></a>
  <a href="#"><img src="https://img.shields.io/badge/build-passing-brightgreen" alt="build"/></a>
</p>

---

## 📘 Overview

**Inventory Management System / AI-Finance Dashboard** — a full-stack application to help businesses track and manage stock levels, purchases, sales, and financial insights.
Built with **Next.js**, **TypeScript**, **RTK Query**, **Express.js**, and **Recharts**. Deployed on **AWS** (EC2, RDS, Amplify, API Gateway, S3).

---

## 🔎 Table of Contents

- [Demo / Screenshots](#-dashboard-preview)
- [Example Insights](#-example-insights)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Architecture & Data Flow](#️-project-architecture--data-flow)
- [Getting Started](#-getting-started)
- [Environment Variables](#-environment-variables)
- [Run Locally](#-run-locally)
- [Contributing](#-contributing)
- [License](#-license)
- [Contact](#-contact)

---

## 📸 Dashboard Preview

<p align="center">
  <strong>1️⃣ Dashboard Overview</strong><br/>
  <img src="Images/Dashboard.png" alt="Dashboard Overview" width="800"/>
</p>

<p align="center">
  <strong>2️⃣ Inventory</strong><br/>
  <img src="Images/Prediction.png" alt="Inventory" width="800"/>
</p>

<p align="center">
  <strong>3️⃣ Products</strong><br/>
  <img src="Images/Prediction.png" alt="Products" width="800"/>
</p>

<p align="center">
  <strong>4️⃣ Users</strong><br/>
  <img src="Images/Prediction.png" alt="Users" width="800"/>
</p>

<p align="center">
  <strong>5️⃣ Expenses</strong><br/>
  <img src="Images/Prediction.png" alt="Expenses" width="800"/>
</p>

---

## 📊 Example Insights

- Popular product (top sellers)
- Sales summary (daily / weekly / monthly)
- Purchase summary and supplier breakdown
- Expense summary & categories
- Discounts applied and impact on revenue
- Inventory levels & low-stock alerts
- Products catalogue overview
- Users / roles analytics
- Expense trends and forecasts

---

## 🚀 Features

- ✅ User authentication & role-based access (admin, manager, staff)
- ✅ Product CRUD (create, read, update, delete) with images
- ✅ Inventory management with stock level tracking & alerts
- ✅ Purchase order and sales order management
- ✅ Expense management & categories
- ✅ Interactive dashboards & charts (Recharts) for financial insights
- ✅ Search, filters, and pagination for lists
- ✅ CSV export / import for products, inventory, and reports
- ✅ RESTful API (Express) consumed by Next.js frontend using RTK Query
- ✅ Deploy-ready (Dockerfile examples + AWS deployment notes)
- ✅ Unit & integration testing setup (Jest + React Testing Library)
- ✅ Basic CI workflow (GitHub Actions) for builds & tests

---

## 🛠️ Tech Stack

- Frontend: **Next.js**, **React**, **TypeScript**, **RTK Query**, **Recharts**
- Backend: **Express.js**, **Node.js**, **TypeScript**
- Database: **MongoDB** (or can swap to **Postgres** on RDS)
- Authentication: **JWT** (or OAuth support)
- DevOps / Hosting: **AWS EC2**, **RDS**, **Amplify**, **API Gateway**, **S3**
- Testing: **Jest**, **React Testing Library**
- Tooling: **ESLint**, **Prettier**, **Docker**, **GitHub Actions**

---

## 📂 Project Structure (example)

```
ai-finance-dashboard/
├─ client/ # Next.js frontend
│  ├─ public/
│  │  └─ Images/
│  ├─ src/
│  │  ├─ components/
│  │  ├─ pages/
│  │  ├─ features/
│  │  └─ styles/
│  ├─ package.json
│  └─ tsconfig.json
├─ server/ # Express backend
│  ├─ src/
│  │  ├─ controllers/
│  │  ├─ routes/
│  │  ├─ models/
│  │  └─ services/
│  ├─ tests/
│  ├─ package.json
│  └─ tsconfig.json
├─ infra/ # Deployment scripts, Terraform (optional)
├─ docker/
│  ├─ Dockerfile.client
│  └─ Dockerfile.server
├─ .github/
│  └─ workflows/
├─ README.md
└─ .env.example
```

---

## 🏗️ Project Architecture & Data Flow

<p align="center">
  <strong>1️⃣ Architecture Diagram</strong><br/>
  <img src="Images/Architecture.png" alt="Architecture Diagram" width="800"/>
</p>

<p align="center">
  <strong>2️⃣ Server Architecture</strong><br/>
  <img src="Images/Server Architecture.png" alt="Server Architecture" width="800"/>
</p>

<p align="center">
  <strong>3️⃣ Data Flow</strong><br/>
  <img src="Images/DataFlow.png" alt="Data Flow" width="800"/>
</p>

<p align="center">
  <strong>4️⃣ Database Tables</strong><br/>
  <img src="Images/Database Tables.png" alt="Database Tables" width="800"/>
</p>

---

## ⚡ Getting Started

### Prerequisites

- Node.js (v18+) & npm / pnpm / yarn
- MongoDB (local or Atlas) or a managed DB (RDS)
- (Optional) Docker & Docker Compose

### Clone the repository

```bash
git clone <repository-url>
cd ai-finance-dashboard
```

### Environment variables

Create a `.env` (or use `.env.local` for Next.js). Example:

```ini
# server
PORT=5000
MONGO_URI=mongodb+srv://<user>:<pass>@cluster0.mongodb.net/mydb?retryWrites=true&w=majority
JWT_SECRET=your_jwt_secret

# client
NEXT_PUBLIC_API_URL=http://localhost:5000/api
```

### Install dependencies

```bash
# from project root
cd client && npm install
cd ../server && npm install
```

### Run locally (development)

```bash
# start backend
cd server
npm run dev

# start frontend
cd ../client
npm run dev
```

### 🧪 Tests

```bash
# run server tests
cd server
npm test

# run client tests
cd client
npm test
```

### 🐳 Docker (optional)

```bash
# build and run all with docker-compose
docker-compose up --build
```

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feat/your-feature`
3. Commit your changes: `git commit -m "feat: add ..."`
4. Push branch and open a PR

Please follow the code style (ESLint + Prettier) and add tests for new features.

---

## 📜 License

This project is licensed under the MIT License. See the LICENSE file for details.

---

## 🧾 Conclusion

This Inventory / AI-Finance Dashboard is designed to be modular and deployable. It provides real-time insights into sales, inventory, and expenses and is easily extensible to add ML-driven forecasts or third-party integrations.

---

## ✉️ Contact

Bhanu — feel free to open issues or PRs.
Project: github.com/your-username/ai-finance-dashboard

<p align="center">Made with ❤️ · Built with Next.js + Express + TypeScript</p>
