# 🚇 Metro Ticket Generating System in ServiceNow

<p align="center">
  A digital metro ticket booking system built using <b>ServiceNow</b> with automated fare calculation, Flow Designer workflow, QR-based ticket generation, request tracking, and role-based access.
</p>

---

## 📌 Project Overview

The **Metro Ticket Generating System in ServiceNow** is designed to reduce manual metro ticket booking and provide a simple digital workflow for passengers and metro operations.

With this system, passengers can:

- Select **Source** and **Destination**
- Choose **Passenger Type**
- Enter **Number of Tickets**
- Get **Fare Calculation**
- Submit **Ticket Request**
- Receive a **QR Digital Ticket**
- Track **Request Status**
- Show the ticket for **Verification**

---

## ⚙️ Technologies Used

- **ServiceNow**
- **Service Catalog**
- **Flow Designer**
- **Service Portal**
- **Custom Tables**
- **UI Policies**
- **Catalog Client Scripts**
- **Roles & ACLs**
- **QR Code**
- **spModal**

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

🖼️ Project Visuals
Workflow 1
 
Workflow 2
 
If your folder name or image names are different, replace the paths with your exact file names.

✨ Key Features
- Digital Metro Ticket Booking
- Automated Fare Calculation
- Flow Designer Automation
- Custom Metro Database
- QR-Based Digital Ticket
- Request Status Tracking
- Role-Based Access
- ACL Security
- Workflow Debugging
🐞 Challenges Solved
- QR rendering issue in Service Portal
- Fare mismatch
- Variable-to-field mapping issues
- Flow Designer execution problems
- Dynamic form behaviour issues
QR Issue Solution
The QR rendering issue was solved using:
- Service Portal Widget
- spModal
- Portal-compatible QR rendering
🔮 Future Scope
- UPI / Payment Gateway Integration
- SMS Ticket Delivery
- Email Ticket Delivery
- WhatsApp Booking
- Travel Analytics Dashboard
- Monthly Passes
- Ticket Cancellation & Refund
👨‍💻 Developer
Veda Sarathi V
- Project: Metro Ticket Generating System in ServiceNow
- Platform: ServiceNow
⭐ Final Outcome
This project demonstrates a complete ServiceNow-based metro ticketing workflow from booking to verification, using low-code automation and structured digital processing.

## Small important note
In your screenshot, your image path currently looks like this:

```markdown
![Metro Ticket Workflow 1](./Result/Workflow - 1.png)
![Metro Ticket Workflow 2](./Result/Workflow - 2.png)

That is okay only if:
- folder name is exactly Result
- image names are exactly Workflow - 1.png and Workflow - 2.png
If your images are actually inside Workflows folder, then use:
![Metro Ticket Workflow 1](./Workflows/Workflow%20-%201.png)
![Metro Ticket Workflow 2](./Workflows/Workflow%20-%202.png)
