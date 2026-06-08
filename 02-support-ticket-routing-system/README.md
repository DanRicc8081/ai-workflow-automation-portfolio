# AI Support Ticket Routing System

## Demo Video
Short walkthrough of the workflow and how it operates.

👉 Watch Demo Video: [paste Loom link here]

## Overview
This project is an AI-powered support operations workflow built with Make, OpenAI, Tally, Google Sheets, Gmail, and Telegram.

The system collects customer support requests through a Tally form, classifies each ticket using OpenAI, stores the structured ticket data in Google Sheets, sends the customer a confirmation email, and routes the ticket to the correct internal support path.

## Problem
Support teams often receive different types of customer issues through forms or inboxes.

Manually reviewing, categorizing, prioritizing, and routing each ticket takes time and can delay urgent cases.

## Solution
This workflow automates first-level ticket triage.

It classifies each request by:
- Category
- Urgency
- Priority score
- Summary
- Recommended action
- Route

The workflow then logs the ticket, sends a confirmation email, and alerts the correct internal team.

## Workflow
1. Customer submits a support request through Tally.
2. Make triggers the workflow.
3. OpenAI classifies the ticket into structured JSON.
4. JSON Parse extracts the AI-generated fields.
5. Google Sheets logs the ticket.
6. Gmail sends the customer a confirmation email.
7. Router sends the ticket to the correct support path.
8. Telegram sends an internal alert to the team.

## Architecture
Tally Form → OpenAI → JSON Parse → Google Sheets → Gmail → Router → Telegram Alerts

## Tools Used
- Make
- OpenAI
- Tally
- JSON Parse
- Google Sheets
- Gmail
- Telegram Bot

## Routing Logic
- `technical_support` → Technical Support alert
- `billing_support` → Billing Support alert
- `customer_support` → Customer Support alert
- `manual_review` → Fallback/manual review alert

## Ticket Categories
The workflow classifies requests into categories such as:

- Technical issue
- Billing question
- Account access
- Feature request
- General question
- Unknown

## Priority Levels
The workflow assigns:

- High
- Medium
- Low

It also generates a priority score from 1 to 10.

## Example Output

| Category | Urgency | Priority Score | Route |
|---|---:|---:|---|
| technical_issue | high | 9 | technical_support |
| billing_question | high | 8 | billing_support |
| general_question | low | 2 | customer_support |
| unknown | low | 1 | manual_review |

## Key Features
- Structured support ticket intake
- AI-based ticket classification
- JSON parsing
- Google Sheets ticket database
- Gmail confirmation email
- Router-based support paths
- Telegram internal alerts
- Fallback route for unclear tickets

## Skills Demonstrated
- Workflow automation
- Prompt design
- JSON parsing
- Router/filter logic
- Form intake automation
- Google Sheets database logging
- Gmail automation
- Telegram alerting
- Fallback handling

## Possible Improvements
- Airtable integration
- Slack notifications
- CRM integration
- Escalation workflows
- Ticket status tracking
- Multi-agent assignment

## Screenshots

### 1. Tally Support Form
![Tally Support Form](1-tally-support-form.png)

### 2. Full Make Workflow
![Full Make Workflow](2-full-workflow.png)

### 3. Google Sheets Ticket Database
![Google Sheets Ticket Database](3-google-sheets-ticket-database.png)

### 4. Router Logic and Telegram Alerts
![Router Logic and Telegram Alerts](4-router-telegram-alerts.png)
