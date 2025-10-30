# 🧾 Overdue Invoice Reminder Flow  
**BUSACT702 – Robotics Process Automation Assignment (University of Auckland)**  
**Student:** Suzzy Zhang | **Date:** 31 October 2025  

---

## 📌 Project Overview
This Power Automate flow automatically checks overdue invoices from an Excel table stored in OneDrive and sends reminder emails to clients.  
It helps the accounting team ensure timely payment follow-ups and reduces manual workload.

---

## ⚙️ Flow Logic
1. Trigger: **Scheduled Cloud Flow** – runs every day at 9:00 AM.  
2. Action: **Get Rows (Excel Online)** – retrieves invoice records.  
3. Condition: Checks if `DueDate < Today` AND `Status ≠ Paid`.  
4. If Yes → Sends reminder email via Outlook.  
5. Logs reminder actions back into Excel.

---

## 🧩 Key Files
| File | Description |
|------|--------------|
| `OverdueInvoiceReminder.docx` | Full report following BUSACT702 rubric |
| `InvoiceReminderFlow.zip` | Exported Power Automate package |
| `screenshots/` | Contains all workflow screenshots |

---

## 📸 Screenshots
| Step | Description | Preview |
|------|--------------|----------|
| Step 1 | Create Scheduled Flow | ![Create Flow](screenshots/Step1_CreateFlow.png) |
| Step 2 | Get Rows (Excel) | ![Get Rows](screenshots/Step2_GetRows.png) |
| Step 3 | Condition Logic | ![Condition](screenshots/Step4_Condition.png) |
| Step 4 | Send Email | ![Email Action](screenshots/Step5_EmailAction.png) |
| Step 5 | Test Run | ![Test Run](screenshots/Step7_TestRun.png) |

---

## 🧠 Reflection
Creating this automation improved my understanding of conditional logic and date comparisons in Power Automate.  
The process was easy to implement but still provided meaningful business value.  
Future improvements could include adding Teams notifications and integrating AI Builder for invoice scanning.

---

## 🧾 Academic Reference
- Microsoft. (2025). *Send an email when an Excel row meets a condition.* https://learn.microsoft.com/en-us/power-automate/  
- OpenAI. (2025). *ChatGPT-assisted RPA documentation workflow.* https://chat.openai.com  
