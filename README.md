# CloudLedger

<div align="center">

<h1>☁️ CloudLedger</h1>

<p>
<strong>Open Source ERP & CRM Platform for Modern Business Operations</strong>
</p>

<p>
Manage customers, products, sales, invoices, payments, quotes, inventory, and business operations from a single platform.
</p>

</div>

---

## 🚀 Overview

**CloudLedger** is a full-stack ERP and CRM platform designed to centralize essential business operations in one application.

It provides tools for managing customers, products, sales, invoices, payments, quotations, inventory, and financial workflows through a modern web-based interface.

The platform is built around a modular architecture using the **MERN stack**, with a React-based frontend, Node.js/Express backend, and MongoDB database.

### Core Technology

* **Frontend:** React.js
* **UI Framework:** Ant Design
* **State Management:** Redux
* **Backend:** Node.js
* **API Framework:** Express.js
* **Database:** MongoDB
* **Architecture:** MERN Stack
* **API:** REST
* **Language:** JavaScript

---

# ✨ Features

## 👥 Customer Management

* Create and manage customers
* Customer profiles
* Contact information
* Customer transaction history
* Customer activity tracking

## 🧾 Invoice Management

* Create invoices
* Update and manage invoices
* Track invoice status
* Customer invoice history
* Invoice totals and calculations
* Outstanding invoice tracking

## 💳 Payment Management

* Record payments
* Track payment status
* Payment history
* Outstanding balances
* Customer payment tracking

## 📋 Quote Management

* Create quotations
* Manage quotation status
* Customer quotation history
* Convert quotations into invoices
* Track quote lifecycle

## 📦 Product & Inventory Management

* Product management
* Product categorization
* Inventory tracking
* Stock management
* Product pricing
* Inventory operations

## 💰 Accounting

* Revenue tracking
* Invoice tracking
* Payment records
* Customer balances
* Financial summaries

## 📊 Business Dashboard

CloudLedger provides a centralized dashboard for monitoring important business activity, including:

* Sales
* Revenue
* Customers
* Invoices
* Payments
* Products
* Business activity

---

# 🏗️ Architecture

CloudLedger follows a client-server architecture built around a RESTful API.

```text
                         ┌──────────────────────┐
                         │     CloudLedger      │
                         │      Web Client      │
                         │        React         │
                         └──────────┬───────────┘
                                    │
                                    │ REST API
                                    ▼
                         ┌──────────────────────┐
                         │      API Server      │
                         │   Node.js / Express  │
                         └──────────┬───────────┘
                                    │
                    ┌───────────────┴───────────────┐
                    │                               │
                    ▼                               ▼
          ┌──────────────────┐           ┌──────────────────┐
          │     MongoDB      │           │ Business Logic   │
          │     Database     │           │    & Services    │
          └──────────────────┘           └──────────────────┘
```

The frontend communicates with the backend through REST APIs.

The backend handles:

* Authentication
* Authorization
* Request validation
* Business logic
* Database operations
* API responses
* Error handling

---

# 🛠️ Technology Stack

| Layer                    | Technology |
| ------------------------ | ---------- |
| Frontend                 | React.js   |
| UI Framework             | Ant Design |
| State Management         | Redux      |
| Backend                  | Node.js    |
| API Framework            | Express.js |
| Database                 | MongoDB    |
| Language                 | JavaScript |
| API Architecture         | REST       |
| Application Architecture | MERN       |

---

# 📁 Project Structure

```text
cloudledger/
│
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── services/
│   ├── middleware/
│   ├── helpers/
│   └── server.js
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── redux/
│   │   ├── services/
│   │   ├── routes/
│   │   └── utils/
│   │
│   └── public/
│
├── docs/
│
├── .env.example
├── docker-compose.yml
└── README.md
```

---

# 🚀 Getting Started

## Prerequisites

Before running CloudLedger locally, make sure you have:

* Node.js
* npm
* MongoDB
* Git

---

## 1. Clone the Repository

```bash
git clone <your-repository-url>
cd cloudledger
```

---

## 2. Configure Environment Variables

Create your environment configuration:

```bash
cp .env.example .env
```

Configure the required environment variables.

Example:

```env
NODE_ENV=development

PORT=5000

MONGO_URI=mongodb://localhost:27017/cloudledger

JWT_SECRET=your-secret-key

CLIENT_URL=http://localhost:3000
```

> Never commit production credentials or secrets to the repository.

---

# ⚙️ Backend Setup

Navigate to the backend:

```bash
cd backend
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

The API will be available at:

```text
http://localhost:5000
```

---

# 🎨 Frontend Setup

Open another terminal and navigate to the frontend:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm start
```

The application will be available at:

```text
http://localhost:3000
```

---

# 🔌 API

CloudLedger exposes REST APIs for the major business domains.

Example API resources:

```text
/api/auth
/api/customers
/api/products
/api/invoices
/api/payments
/api/quotes
/api/suppliers
/api/inventory
```

The API layer provides the foundation for communication between the web application and business services.

---

# 🔐 Security

CloudLedger uses environment-based configuration for sensitive application settings.

Security considerations include:

* Authentication
* Authorization
* Protected API routes
* Environment-based secrets
* Input validation
* Secure database configuration

Production deployments should use secure credentials, HTTPS, restricted database access, and appropriate secret-management solutions.

---

# 🐳 Docker

CloudLedger can be run using Docker where supported by the project configuration.

Build the application:

```bash
docker compose build
```

Start the services:

```bash
docker compose up
```

Stop the services:

```bash
docker compose down
```

---

# 🧪 Testing

Run the available tests using:

```bash
npm test
```

For frontend tests:

```bash
cd frontend
npm test
```

Additional integration and end-to-end tests can be added as the platform evolves.

---

# 📈 Roadmap

CloudLedger is intended to evolve into a more complete business management platform.

### Platform

* [ ] Improved authentication
* [ ] Role-based access control
* [ ] Multi-company support
* [ ] Audit logging
* [ ] Advanced permissions
* [ ] API documentation

### CRM

* [ ] Customer activity timeline
* [ ] Lead management
* [ ] Sales pipeline
* [ ] Customer segmentation

### Accounting

* [ ] Financial reports
* [ ] Expense management
* [ ] Tax configuration
* [ ] Account reconciliation

### Inventory

* [ ] Stock alerts
* [ ] Purchase orders
* [ ] Warehouse management
* [ ] Inventory movement history

### Platform Engineering

* [ ] Automated test coverage
* [ ] CI/CD pipeline
* [ ] Docker deployment
* [ ] Cloud deployment
* [ ] Application monitoring
* [ ] Performance monitoring

---

# 🤝 Contributing

Contributions and improvements are welcome.

Before submitting a pull request:

1. Create a feature branch.
2. Implement your changes.
3. Add or update tests where appropriate.
4. Verify the application builds successfully.
5. Update documentation when necessary.
6. Submit a pull request describing your changes.

---

# 📸 Screenshots

Screenshots and product demonstrations will be added as the platform evolves.

Suggested screenshots:

* Dashboard
* Customer management
* Invoice management
* Quote management
* Product management
* Payment management
* Reports

---

# 📄 License & Attribution

CloudLedger is based on the open-source **IDURAR ERP/CRM** project.

The original project is released under the **GNU Affero General Public License v3.0 (AGPL-3.0)**.

This repository retains the applicable license requirements and attribution from the upstream project.

Please review the project's license and original attribution files before redistributing or deploying modified versions.

---

# 🌟 Project

<div align="center">

**CloudLedger**

ERP · CRM · Accounting · Invoicing · Inventory

Built with **React · Node.js · Express · MongoDB**

</div>

