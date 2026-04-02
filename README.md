# Leave Approval Automation using n8n

## 📌 Project Overview
This project automates the **leave approval process** using **n8n, Google Forms, Google Sheets, and Gmail**.  
When an employee submits a leave request through a Google Form, the workflow automatically checks the number of leaves requested and sends an **approval or rejection email**.

The system reduces manual HR work and provides **instant responses to employees**.

---

## ⚙️ Tech Stack

- **n8n** – Workflow automation platform  
- **Google Forms** – Collect leave requests  
- **Google Sheets** – Store form responses and processed data  
- **Gmail API** – Send automated email notifications  

---

## 🔄 Workflow Process

1. Employee submits a leave request via **Google Form**
2. The response is stored in **Google Sheets**
3. **n8n Google Sheets Trigger** detects the new entry
4. An **IF condition** checks the number of leaves requested
5. If the leave count exceeds the allowed limit, the request is rejected
6. If the leave count is within the allowed limit, the request is approved
7. An **email notification** is sent to the employee
8. The result is logged back into **Google Sheets**

---

## 📊 Approval Logic

| Leaves Requested | Result |
|------------------|--------|
| ≤ 3 Leaves | Approved |
| > 3 Leaves | Not Approved |

---

## 🖼️ n8n Workflow Screenshot

Add your n8n workflow screenshot below.

![n8n Workflow](images/n8n-workflow.png)
<img width="1094" height="392" alt="image" src="https://github.com/user-attachments/assets/88ff6353-1651-4ac0-a564-7bb13c46d38d" />

---

## 📊 Dashboard Screenshot

Add your analytics or Google Sheets dashboard screenshot below.

![Dashboard Screenshot](images/dashboard.png)
<img width="799" height="445" alt="Screenshot 2026-04-01 155549" src="https://github.com/user-attachments/assets/a40c54da-970b-4617-a121-8c1e3c52af38" />

The dashboard can display:
- Total leave requests
- Approved leaves
- Rejected leaves
- Leave trends over time

---


---

## 🚀 Setup Instructions

### 1️⃣ Import Workflow
1. Open **n8n**
2. Click **Import Workflow**
3. Upload the `workflow.json` file

### 2️⃣ Connect Credentials
Configure the following credentials in n8n:

- Google Sheets OAuth2
- Gmail OAuth2

### 3️⃣ Connect Google Form
Ensure the Google Form is connected to the Google Sheet used in the workflow.

### 4️⃣ Activate Workflow
Turn on the workflow so n8n can monitor new entries.

---

## 💡 Future Improvements

### Manager Approval Step
Add an intermediate approval stage where a manager must approve the request before sending the final email.

### Leave Balance System
Track employee leave balances automatically and deduct approved leaves.

### Slack or Teams Notifications
Send notifications to HR or managers when a leave request is submitted.

### Advanced Dashboard
Create a detailed analytics dashboard using:
- Google Looker Studio
- Power BI
- Tableau

### Database Integration
Replace Google Sheets with a database such as:
- PostgreSQL
- MySQL
- Airtable

### Role-Based Leave Policies
Define different leave limits based on employee roles:
- Intern
- Employee
- Manager

### AI-Based Leave Analysis
Use AI tools to analyze leave patterns and predict absentee trends.

---

## 🎯 Benefits

- Automates HR leave approval process
- Instant employee notification
- Reduces manual work
- Easy to scale and modify
- Provides useful leave analytics

---

## 👨‍💻 Author

Built using **n8n workflow automation** to demonstrate HR process automation.
