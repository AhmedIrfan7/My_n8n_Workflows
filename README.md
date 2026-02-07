# Customer Support Automation (n8n)

This workflow automates customer support form handling using n8n by collecting user queries, storing them in Google Sheets, and notifying the support team via email.

## 🚀 Overview

The workflow starts with a public **Contact Form** where users submit their details and issue.  
Once submitted:
1. The data is saved automatically in a **Google Sheet**
2. A notification email is sent to the support team with the issue details

This removes manual work and ensures no customer query is missed.

## 🧩 Workflow Nodes

### 1. Contact Form (Form Trigger)
- Collects the following fields:
  - First Name
  - Last Name
  - Email
  - Issue Description
  - Course Type (n8n / Make / Zapier)
- Acts as the entry point of the workflow

### 2. Google Sheets – Append Row
- Appends each form submission as a new row
- Stores:
  - User details
  - Course type
  - Issue description
  - Submission timestamp
- Useful for tracking and analytics

### 3. Gmail – Send Message
- Sends an email notification to the support email address
- Includes:
  - User name
  - Issue description
- Ensures instant awareness of new submissions

## 🛠️ Requirements

- n8n (self-hosted or cloud)
- Google Sheets OAuth credentials
- Gmail OAuth credentials
- A Google Sheet with matching column headers

## 📥 Setup Instructions

1. Import the workflow JSON into n8n
2. Configure Google Sheets credentials
3. Configure Gmail credentials
4. Verify column names in the Google Sheet
5. Activate the workflow
6. Share the form URL with users

## ✅ Use Cases

- Customer support ticket collection
- Course inquiry management
- Lead capture and follow-ups
- Internal issue reporting

## 🔒 Notes

- Make sure OAuth permissions are granted correctly
- Keep the Google Sheet private
- Update email address if the support contact changes

---

**Author:** Ahmed Irfan  
**Built with:** n8n, Google Sheets, Gmail
