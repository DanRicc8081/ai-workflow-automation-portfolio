# AI Lead Qualification Workflow

## 🎥 Demo Video

Short walkthrough of the workflow and how it operates.

👉 [▶️ Watch Demo Video](https://www.loom.com/share/4f232efe06224b9abc1340f28c3114aa) 



## Problem

Businesses often receive many inbound leads through forms, chat systems, or APIs.

Reviewing and prioritizing leads manually can be slow and repetitive, especially when only a small percentage of leads require immediate attention.



## Workflow Overview

When a lead is received through a webhook, the workflow sends the message to OpenAI for classification.

The response is converted into structured data containing lead urgency, intent, and priority level.

A router then determines how the workflow should handle the lead:
- high-priority leads trigger Telegram alerts
- all leads are logged into Google Sheets for tracking



## 🏗️ Architecture

Webhook → OpenAI → JSON Parsing → Router → Google Sheets → Telegram

This workflow uses routing logic to separate high, medium, and low-priority leads into different automation paths.

High-priority leads trigger immediate notifications, while lower-priority leads are stored for tracking without interrupting the workflow.



## 🛠️ Tech Stack

- Make (Integromat)
- OpenAI API
- Google Sheets
- Telegram Bot API
- Webhooks



## 🚀 Key Features

- Automated lead classification
- Lead prioritization based on urgency and intent
- Routing logic for different lead types
- Real-time Telegram notifications
- Automated tracking in Google Sheets
- Structured JSON data handling



## Outcome

This workflow reduces repetitive manual lead review and helps prioritize important leads more efficiently.



## Possible Improvements

Future improvements could include:
- stronger validation for incomplete lead data
- retry handling for failed API responses
- additional routing conditions
- integration with CRM platforms

---

## What I Learned

- Building multi-step automation workflows
- Structuring AI responses into usable data
- Using routers to control workflow behavior
- Organizing automated notifications and tracking



## Screenshots

### Automation Architecture
![Architecture](screenshots/lead-qualification-automation-architecture.png)

### Router Logic
![Router](screenshots/lead-qualification-router-logic.png)

### Example Output
![Output](screenshots/lead-qualification-output-google-sheets.png)
