# 🟠 Safron CRM - Financial Services CRM Platform

<p align="center">
  <img src="public/logo.png" alt="Safron CRM Logo" width="180">
</p>

<p align="center">

![Next.js](https://img.shields.io/badge/Next.js-16-black?logo=next.js)
![React](https://img.shields.io/badge/React-19-61DAFB?logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?logo=typescript)
![Prisma](https://img.shields.io/badge/Prisma-ORM-2D3748?logo=prisma)
![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?logo=mysql)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-v4-38B2AC?logo=tailwind-css)
![License](https://img.shields.io/badge/License-Proprietary-red)

</p>

---

# Enterprise CRM Built for Financial Services

**Safron CRM** is a modern, secure, and enterprise-ready Customer Relationship Management platform designed specifically for financial services organizations.

Built by **Horsemen Technologies (Pty) Ltd**, Safron CRM enables consultants, managers, executives, and support teams to efficiently manage customer relationships, sales opportunities, claims, service queries, and operational workflows from a single platform.

The platform includes:

* Client Management
* Deal Pipeline Management
* Claims Management
* Query Management
* SLA Monitoring
* Executive Dashboards
* Business Reporting
* Notifications
* Role-Based Access Control (RBAC)
* Client 360°
* Activity Auditing

Safron CRM is designed for scalability and can be deployed on:

* Docker
* Ubuntu
* Debian
* AlmaLinux
* Rocky Linux
* cPanel
* VPS
* Dedicated Servers
* Private Cloud
* Public Cloud

---

# Technology Stack

| Technology      | Version              |
| --------------- | -------------------- |
| Next.js         | 16 (App Router)      |
| React           | 19                   |
| TypeScript      | Latest               |
| Tailwind CSS    | v4                   |
| shadcn/ui       | Latest               |
| Prisma ORM      | Latest               |
| MySQL           | 8+                   |
| NextAuth.js     | Credentials Provider |
| Zod             | Latest               |
| React Hook Form | Latest               |
| Recharts        | Latest               |
| Sonner          | Latest               |
| Lucide Icons    | Latest               |

---

# Features

## Executive Dashboard

* Executive KPI Cards
* Revenue Dashboard
* Deal Pipeline
* Monthly Performance
* SLA Metrics
* Recent Activities
* Consultant Performance

---

## Client Management

* Client 360°
* Client Profiles
* Contact Information
* Revenue Tracking
* Satisfaction Score
* Risk Score
* Assigned Consultant
* Assigned Manager

---

## Deal Management

* Complete CRUD
* Kanban Board
* List View

### Deal Stages

```
NEW
CONTACTED
QUALIFIED
PROPOSAL_SENT
NEGOTIATION
WON
LOST
```

Features include:

* Deal Value
* Expected Close Date
* Priority
* Activity Timeline
* Notes
* Attachments
* Conversation History

---

## Claims Management

Automatic Claim Numbers

```
CLM-2026-000001
```

Features

* SLA Tracking
* Escalation
* Attachments
* Conversation Log
* Audit History
* Activity Timeline
* Notifications

---

## Query Management

Automatic Query Numbers

```
QRY-2026-000001
```

Features

* SLA Monitoring
* Escalation
* Internal Notes
* Attachments
* Conversation History

---

## Notifications

* In-App Notifications
* SLA Alerts
* Assignment Notifications
* Claim Notifications
* Query Notifications

---

## Reporting

* Revenue Reports
* Consultant Performance
* SLA Compliance
* CSV Export
* Executive Dashboard Reports

---

## User Management

Supported Roles

* SUPER_ADMIN
* EXECUTIVE
* MANAGER
* CONSULTANT
* SUPPORT_AGENT

Role-Based Access Control (RBAC) is implemented throughout the application.

---

# Installation

## Clone Repository

```bash
git clone https://github.com/Horsementech/safron-crm.git

cd safron-crm
```

---

## Install Dependencies

```bash
npm install
```

---

## Configure Environment

```bash
cp .env.example .env
```

Update:

```
DATABASE_URL=

NEXTAUTH_SECRET=

NEXTAUTH_URL=
```

---

## Generate Prisma Client

```bash
npx prisma generate
```

---

## Push Database Schema

```bash
npx prisma db push
```

---

## Seed Database

```bash
npx tsx prisma/seed.ts
```

---

## Start Development Server

```bash
npm run dev
```

Application URL

```
http://localhost:3000
```

---

# Docker Deployment

Build

```bash
docker compose build --no-cache
```

Start

```bash
docker compose up -d
```

Stop

```bash
docker compose down
```

View Logs

```bash
docker compose logs -f
```

---

# Default Login Credentials

| Role          | Email                                                     | Password     |
| ------------- | --------------------------------------------------------- | ------------ |
| Super Admin   | [admin@evofs.co.za](mailto:admin@evofs.co.za)             | Admin@123456 |
| Executive     | [executive@evofs.co.za](mailto:executive@evofs.co.za)     | Admin@123456 |
| Manager       | [manager@evofs.co.za](mailto:manager@evofs.co.za)         | Admin@123456 |
| Consultant 1  | [consultant1@evofs.co.za](mailto:consultant1@evofs.co.za) | Admin@123456 |
| Consultant 2  | [consultant2@evofs.co.za](mailto:consultant2@evofs.co.za) | Admin@123456 |
| Support Agent | [support@evofs.co.za](mailto:support@evofs.co.za)         | Admin@123456 |

> **Important:** Change all default passwords immediately after the first login.

---

# Project Structure

```text
src/
├── app/
│   ├── (dashboard)/
│   │   ├── dashboard/
│   │   ├── deals/
│   │   ├── claims/
│   │   ├── queries/
│   │   ├── clients/
│   │   ├── users/
│   │   ├── reports/
│   │   ├── notifications/
│   │   └── settings/
│   ├── api/
│   ├── login/
│   └── layout.tsx
│
├── components/
│   ├── ui/
│   ├── dashboard/
│   ├── forms/
│   └── shared/
│
├── lib/
│   ├── auth.ts
│   ├── prisma.ts
│   ├── permissions.ts
│   └── utils.ts
│
├── hooks/
├── types/
└── prisma/
```

---

# Security

Safron CRM includes enterprise-grade security features:

* Password Hashing
* Role-Based Access Control (RBAC)
* Secure Authentication
* Protected Routes
* Activity Auditing
* Audit Logs
* Session Management

---

# Roadmap

Planned Features

* Email Integration
* Calendar Management
* Microsoft Outlook Integration
* Microsoft Teams Integration
* WhatsApp Integration
* SMS Gateway
* Workflow Automation
* Client Portal
* Document Management
* Electronic Signatures
* Multi-Tenant / Multi-Company Support
* Public REST API
* Mobile Applications (iOS & Android)

---

# Contributing

We welcome contributions from the community.

1. Fork the repository.
2. Create a feature branch:

```bash
git checkout -b feature/my-feature
```

3. Commit your changes:

```bash
git commit -m "feat: add new feature"
```

4. Push your branch:

```bash
git push origin feature/my-feature
```

5. Open a Pull Request.

Please review **CONTRIBUTING.md** before contributing.

---

# License

Safron CRM is proprietary software owned by **Horsemen Technologies (Pty) Ltd**.

Unauthorized copying, distribution, modification, reverse engineering, or resale is prohibited without prior written permission.

Copyright © 2026 Horsemen Technologies (Pty) Ltd.

All Rights Reserved.

---

# Support

* 🌐 Website: https://horsementech.com
* 📧 General Enquiries: [info@horsementech.com](mailto:info@horsementech.com)
* 🛠 Technical Support: [support@horsementech.com](mailto:support@horsementech.com)
* 🔒 Security: [security@horsementech.com](mailto:security@horsementech.com)

For assistance, please refer to **SUPPORT.md** and **SECURITY.md**.

---

# Developed By

## Horsemen Technologies (Pty) Ltd

**Enterprise Software • Cloud Solutions • Infrastructure • Cybersecurity**

<p align="center">
Built with ❤️ by Horsemen Technologies
</p>
