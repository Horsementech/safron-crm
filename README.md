# EVO CRM - Financial Services CRM Platform

<p align="center">
  <img src="public/logo.png" alt="EVO CRM Logo" width="180">
</p>

<p align="center">

![Next.js](https://img.shields.io/badge/Next.js-16-black?logo=next.js)
![React](https://img.shields.io/badge/React-19-61DAFB?logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?logo=typescript)
![Prisma](https://img.shields.io/badge/Prisma-ORM-2D3748?logo=prisma)
![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?logo=mysql)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-v4-38B2AC?logo=tailwind-css)
![License](https://img.shields.io/badge/License-Private-red)

</p>

---

## Overview

**EVO CRM** is a modern Customer Relationship Management platform built specifically for **financial services companies**.

The platform enables consultants, managers, executives, and support teams to manage:

- Clients
- Deals
- Claims
- Queries
- SLA Monitoring
- Reporting
- Notifications
- Role Based Access
- Client 360°
- Activity Auditing

Designed with scalability in mind, EVO CRM can be deployed on:

- Docker
- Ubuntu
- Debian
- AlmaLinux
- Rocky Linux
- cPanel Servers
- VPS
- Dedicated Servers
- Cloud Platforms

---

# Technology Stack

| Technology | Version |
|------------|---------|
| Next.js | 16 (App Router) |
| React | 19 |
| TypeScript | Latest |
| Tailwind CSS | v4 |
| shadcn/ui | Latest |
| Prisma ORM | Latest |
| MySQL | 8+ |
| NextAuth.js | Credentials Provider |
| Zod | Latest |
| React Hook Form | Latest |
| Recharts | Latest |
| Sonner | Latest |
| Lucide Icons | Latest |

---

# Features

## Executive Dashboard

- Executive KPI Cards
- Revenue Dashboard
- Deal Pipeline
- Monthly Performance
- SLA Metrics
- Recent Activities
- Consultant Performance

---

## Client Management

- Client 360°
- Client Profiles
- Contact Information
- Revenue Tracking
- Satisfaction Score
- Risk Score
- Assigned Consultant
- Assigned Manager

---

## Deal Management

- Complete CRUD
- Kanban Board
- List View
- Deal Stages

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

- Deal Value
- Expected Close Date
- Priority
- Activity Timeline
- Notes
- Attachments
- Conversation History

---

## Claims Management

Automatic Claim Numbers

```
CLM-2026-000001
```

Features

- SLA Tracking
- Escalation
- Attachments
- Conversation Log
- Audit History
- Activity Timeline
- Notifications

---

## Query Management

Automatic Query Numbers

```
QRY-2026-000001
```

Features

- SLA Monitoring
- Escalation
- Internal Notes
- Attachments
- Conversation History

---

## Notifications

- In-App Notifications
- SLA Alerts
- Assignment Notifications
- Claim Notifications
- Query Notifications

---

## Reporting

- Revenue Reports
- Consultant Performance
- SLA Compliance
- CSV Export
- Executive Dashboard Reports

---

## User Management

Supported Roles

- SUPER_ADMIN
- EXECUTIVE
- MANAGER
- CONSULTANT
- SUPPORT_AGENT

Role Based Access Control (RBAC) is implemented throughout the application.

---

# Installation

## Clone Repository

```bash
git clone https://github.com/sya-one/evo-crm.git

cd evo-crm
```

---

## Install Dependencies

```bash
npm install
```

---

## Configure Environment

Copy the example file

```bash
cp .env.example .env
```

Update

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

## Push Database

```bash
npx prisma db push
```

---

## Seed Database

```bash
npx tsx prisma/seed.ts
```

---

## Start Development

```bash
npm run dev
```

Application

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

Logs

```bash
docker compose logs -f
```

---

# Default Login Credentials

| Role | Email | Password |
|------|-------|----------|
| Super Admin | admin@evofs.co.za | Admin@123456 |
| Executive | executive@evofs.co.za | Admin@123456 |
| Manager | manager@evofs.co.za | Admin@123456 |
| Consultant 1 | consultant1@evofs.co.za | Admin@123456 |
| Consultant 2 | consultant2@evofs.co.za | Admin@123456 |
| Support Agent | support@evofs.co.za | Admin@123456 |

> Change all default passwords immediately after the first login.

---

# Project Structure

```
src/

├── app/
│
├── (dashboard)
│   ├── dashboard
│   ├── deals
│   ├── claims
│   ├── queries
│   ├── clients
│   ├── users
│   ├── reports
│   ├── notifications
│   └── settings
│
├── api
├── login
├── layout.tsx
│
├── components
│   ├── ui
│   ├── dashboard
│   ├── forms
│   └── shared
│
├── lib
│   ├── auth.ts
│   ├── prisma.ts
│   ├── permissions.ts
│   └── utils.ts
│
├── hooks
│
├── types
│
└── prisma
```

---

# Security

- Password Hashing
- Role Based Access Control
- Secure Authentication
- Protected Routes
- Audit Logs
- Activity Tracking
- Session Management

---

# Roadmap

Upcoming Features

- Email Integration
- Calendar
- Outlook Integration
- Microsoft Teams Integration
- WhatsApp Integration
- SMS Gateway
- Workflow Automation
- Client Portal
- Document Management
- Electronic Signatures
- Multi-Company Support
- API Access
- Mobile Application

---

# Contributing

1. Fork the repository

2. Create a feature branch

```bash
git checkout -b feature/my-feature
```

3. Commit changes

```bash
git commit -m "Added new feature"
```

4. Push

```bash
git push origin feature/my-feature
```

5. Open a Pull Request

---

# License

This project is proprietary software.

Unauthorized copying, distribution, modification, or resale is prohibited without written permission.

© 2026 EVO Financial Services.

All Rights Reserved.

---

# Developed By

**Horsemen Technologies (Pty) Ltd**

Enterprise Software • Cloud Solutions • Infrastructure • Cyber Security

Website:
https://horsementech.com

Support:
support@horsementech.com

Email:
info@horsementech.com

---

<p align="center">
Built with ❤️ by Horsemen Technologies
</p>