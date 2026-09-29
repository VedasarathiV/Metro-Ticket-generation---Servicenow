# 🚇 Metro Ticket Generating System in ServiceNow

A digital metro ticket booking system built using **ServiceNow** with automated fare calculation, Flow Designer workflow, custom data storage, QR-based ticket generation, request tracking, and role-based access.


### Important before committing

Only change these two lines:

```markdown
![Metro Ticket Workflow 1](./Result/Workflow - 1.png)

![Metro Ticket Workflow 2](./Result/Workflow - 2.png)
---

## 📌 Project Overview

The main objective of this project is to reduce manual metro ticket booking and provide a simple digital workflow.

Passengers can:

- Select Source and Destination
- Choose Passenger Type
- Enter Number of Tickets
- Get Fare Calculation
- Submit Ticket Request
- Receive a QR Digital Ticket
- Track Request Status
- Show the ticket for verification

---

## ⚙️ Technologies Used

- ServiceNow
- Service Catalog
- Flow Designer
- Service Portal
- Custom Tables
- UI Policies
- Catalog Client Scripts
- Roles & ACLs
- QR Code
- `spModal`

---

## 🔄 Project Workflow

```text
Passenger
   ↓
ServiceNow Portal
   ↓
Metro Ticket Catalog
   ↓
Fare Calculation
   ↓
Flow Designer
   ↓
Request / RITM
   ↓
Metro Database
   ↓
QR Digital Ticket
   ↓
Station Verification



For your GitHub **About** section, use:

> **ServiceNow-based metro ticketing system with automated fare calculation, Flow Designer workflows, QR ticket generation, request tracking, and role-based access.**
