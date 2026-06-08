# Support Ticket Routing System

## Demo Video

Short walkthrough of the workflow and how it operates.

👉 [Watch Demo Video](PASTE_YOUR_LOOM_LINK_HERE)

---

## Problem

Support teams often receive different types of customer requests.

Manually reviewing each request, assigning priorities, and routing tickets can be slow and inconsistent.

This workflow automatically classifies incoming support requests and routes them based on urgency and category.

---

## Workflow Overview

When a support request is submitted:

1. The workflow is triggered.
2. OpenAI analyzes the request.
3. The request is categorized.
4. A priority level is assigned.
5. The response is converted into structured JSON.
6. Ticket information is logged in Google Sheets.
7. An automated confirmation message is sent.

---

## Architecture

Tally Form → OpenAI → JSON Parse → Google Sheets → Email Notification

---

## Technologies Used

- Make.com
- OpenAI
- Tally Forms
- Google Sheets
- Gmail
- JSON

---

## Ticket Categories

The workflow classifies requests into categories such as:

- Technical Issue
- Billing
- Account Access
- General Inquiry

---

## Priority Levels

The workflow automatically assigns:

- High
- Medium
- Low

based on message content and urgency.

---

## Example Output

| Category | Priority |
|-----------|----------|
| Account Locked | High |
| Payment Question | Medium |
| General Information | Low |

---

## What I Learned

- AI-based ticket classification
- Structured JSON processing
- Automated ticket routing
- Workflow design in Make.com
- Data logging and tracking
- Building support automation systems

---

## Possible Improvements

- Airtable integration
- Slack notifications
- CRM integration
- Escalation workflows
- Ticket status tracking
- Multi-agent assignment

---

## Screenshots

### Workflow Architecture

![Architecture](support-ticket-architecture.png)

### Ticket Classification

![Classification](support-ticket-classification.png)

### Ticket Log

![Log](support-ticket-log.png)
