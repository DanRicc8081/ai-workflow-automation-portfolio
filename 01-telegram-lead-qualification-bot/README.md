# Telegram Lead Qualification Bot

## Demo Video

Short walkthrough of the workflow and how it operates.

👉 [Watch Demo Video](PASTE_YOUR_LOOM_LINK_HERE)

---

## Problem

Businesses often receive messages from potential customers through Telegram.

Manually reviewing every message, identifying customer intent, and responding can be time-consuming and inconsistent.

This workflow automates lead qualification and provides immediate responses while keeping all interactions logged for tracking.

---

## Workflow Overview

When a user sends a message to a Telegram bot:

1. The message triggers the workflow.
2. OpenAI analyzes the message.
3. The message is classified by intent.
4. The result is converted into structured JSON.
5. The lead is logged in Google Sheets.
6. A router sends the appropriate response back to the user.

---

## Architecture

Telegram Bot → OpenAI → JSON Parse → Google Sheets → Router → Telegram Reply

---

## Technologies Used

- Make.com
- OpenAI
- Telegram Bot API
- Google Sheets
- JSON

---

## Intent Classification

The workflow classifies incoming messages into the following categories:

- BOOKING
- PRICING
- SUPPORT
- OTHER

Examples:

| Message | Intent |
|----------|----------|
| I want to book a session | BOOKING |
| How much does it cost? | PRICING |
| I need help with my order | SUPPORT |
| Hello | OTHER |

---

## Example Responses

### BOOKING

Thank you for your interest.

Please provide your email address and preferred date so we can arrange a booking.

### PRICING

Thank you for your inquiry.

Our pricing depends on the service requested. Please provide additional details for an accurate quote.

### SUPPORT

Your request has been received.

A team member will review your message and follow up shortly.

### OTHER

Thank you for contacting us.

Please let us know how we can assist you.

---

## What I Learned

- Building AI-powered automation workflows
- Using OpenAI for intent classification
- Parsing structured JSON outputs
- Implementing routing logic in Make.com
- Integrating Telegram with external services
- Logging workflow data in Google Sheets

---

## Possible Improvements

- CRM integration
- Lead scoring
- Email notifications
- Airtable database integration
- Advanced qualification questions
- Multi-language support

---

## Screenshots

### Workflow Architecture

![Architecture](telegram-architecture.png)

### Router Logic

![Router](telegram-router.png)

### Example Lead Log

![Lead Log](telegram-google-sheets.png)
