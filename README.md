# 🚇 Metro Ticket Generation System in ServiceNow

[![ServiceNow](https://img.shields.io/badge/Platform-ServiceNow-green.svg)](https://www.servicenow.com/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

A digital metro ticketing and automated workflow system built on the **ServiceNow Platform**. This solution replaces manual booking with a self-service digital workflow, automated fare calculation logic, dynamic QR ticket generation, and role-based access control.


<p align="center">
  <img src="Workflows/Workflow%20-%201.png" alt="Workflow 1" width="48%" />
  <img src="Workflows/Workflow%20-%202.png" alt="Workflow 2" width="48%" />
</p>


---

## 📌 Table of Contents
- [Project Overview](#-project-overview)
- [Key Features](#-key-features)
- [System Architecture & Workflow](#-system-architecture--workflow)
- [Project Visuals](#-project-visuals)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Implementation & Configuration](#-implementation--configuration)
- [Troubleshooting & Challenges Solved](#-troubleshooting--challenges-solved)
- [Future Scope](#-future-scope)
- [Author](#-author)

---

## 📌 Project Overview

The **Metro Ticket Generation System** streamlines public transit ticketing by leveraging ServiceNow’s low-code workflow automation capabilities. Passengers can request digital tickets via the Service Portal, receive instant fare quotes, and get a scannable QR ticket upon approval and processing.

---

## ✨ Key Features

- **Self-Service Booking Portal:** User-friendly Service Catalog interface for passengers to select stations, passenger types, and ticket counts.
- **Automated Fare Calculation:** Real-time dynamic price calculation using Catalog Client Scripts and UI Policies.
- **Workflow Automation:** End-to-end request handling via ServiceNow Flow Designer.
- **QR Code Digital Ticket:** Dynamic QR code generation rendered via custom Service Portal widgets (`spModal`).
- **Database & Record Management:** Structured custom tables (`u_metro_ticket_request`) for tracking RITMs and ticket states.
- **Role-Based Access Control (RBAC):** ACL rules ensuring passengers only see their tickets, while station managers retain verification privileges.

---

## 🔄 System Architecture & Workflow

```text
Passenger Request
       │
       ▼
Service Portal (Service Catalog)
       │
       ▼
Catalog Client Scripts / UI Policies (Dynamic Fare Calculation)
       │
       ▼
Flow Designer Execution (RITM & Database Entry)
       │
       ▼
QR Code Generation (Service Portal Widget via spModal)
       │
       ▼
Station Verification & Status Tracking

🖼️ Project Visuals
⚙️ Tech Stack
Platform: ServiceNow (Vancouver / Washington / Xanadu)
Interface: Service Portal, Service Catalog
Automation: Flow Designer, Business Rules
Frontend Logic: Catalog Client Scripts, UI Policies, Widget Client Controllers (spModal)
Database & Security: Custom Tables, Data Policies, Access Control Lists (ACLs)

📁 Project Structure
Plaintext
Metro-Ticket-generation---Servicenow/
├── 1. Ideation Phase/                  # Problem statements, empathy maps & brainstorming
├── 2. Requirement Analysis/           # Data Flow Diagrams, User Stories, Tech Stack docs
├── 3. Project Design Phase/           # Solution architecture & design templates
├── 4. Project Planning Phase/          # Logic planning & project execution timelines
├── 5. Project Development Phase/       # Performance testing reports, UAT logs & test cases
├── 6. Project Documentation/           # FSD documentation & final project report
├── 7. Project Demonstration/           # Demo notes & presentation files
├── Workflows/                          # Workflow diagrams & portal screenshots
│   ├── Workflow - 1.png
│   └── Workflow - 2.png
└── README.md                           # Main documentation file

🛠️ Implementation & Configuration
1. Catalog Item Setup
Create a new Service Catalog Item named Metro Ticket Booking.

Add variables: Source Station, Destination Station, Passenger Type, Number of Tickets, Calculated Fare.

2. Client Scripts & UI Policies
Add a Catalog Client Script on change of Destination Station or Number of Tickets to calculate total fare dynamically.

3. Flow Designer Workflow
Trigger: Service Catalog request submission.

Actions: Create Catalog Task / Update record status → Set state to Approved → Generate Ticket Record.

🔮 Future Scope
[ ] Payment Gateway Integration (UPI, Credit/Debit Cards)

[ ] WhatsApp & SMS Ticket Notification Delivery

[ ] Automated Refund and Cancellation Workflow

[ ] Travel Analytics Dashboard for Metro Authorities

[ ] Pass Management System (Daily / Monthly Passes)

👨‍💻 Author
Veda Sarathi V

ServiceNow Developer & System Designer

GitHub: @VedasarathiV

Repository: Metro-Ticket-generation---Servicenow
