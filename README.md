<!-- Fancy banner -->
<p align="center">
  <img src="https://raw.githubusercontent.com/suzzyzhang/Overdue-Invoice-Reminder/main/screenshots/banner.png" width="100%">
</p>

<h1 align="center">💼 Overdue Invoice Reminder Flow</h1>

<p align="center">
  <b>University of Auckland | BUSACT702 – Robotics Process Automation Assignment</b><br>
  <i>Automate your accounting workflow with Microsoft Power Automate</i><br><br>
  <img src="https://img.shields.io/badge/Tool-Power%20Automate-blue?logo=microsoft&logoColor=white" />
  <img src="https://img.shields.io/badge/Language-Excel%20%7C%20Outlook-green?logo=microsoftexcel" />
  <img src="https://img.shields.io/badge/Version-2025-orange" />
</p>

---

## 🧩 Project Overview

This project automates **overdue invoice reminders** using Microsoft Power Automate.  
Every morning at 9:00 AM, the flow reads an Excel table stored in OneDrive,  
checks which invoices are **overdue and unpaid**, and automatically sends polite email reminders to clients.

🎯 **Goal:** Improve efficiency, reduce manual follow-ups, and maintain timely communication.

---

## ⚙️ Flow Logic Diagram

```mermaid
graph TD;
A[Start - Scheduled Flow] --> B[Get Rows from Excel Table];
B --> C{DueDate < Today AND Status ≠ Paid?};
C -->|Yes| D[Send Reminder Email via Outlook];
C -->|No| E[Skip];
D --> F[Log "Reminder Sent" to Excel];
F --> G[End];
