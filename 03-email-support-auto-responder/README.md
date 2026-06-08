# Email Support Auto-Responder

## Demo Video

Short walkthrough of the workflow and how it operates.

👉 [Watch Demo Video](PASTE_YOUR_LOOM_LINK_HERE)

---

## Problem

Handling repetitive support emails manually can slow down communication and increase response times.

Many requests contain similar questions that can be identified and answered automatically.

This workflow generates draft responses while keeping human review before sending.

---

## Workflow Overview

When a new email is received:

1. Gmail triggers the workflow.
2. OpenAI analyzes the email content.
3. The request is classified.
4. A draft response is generated.
5. The workflow routes the email according to its category.
6. A Gmail draft is created for review.

---

## Architecture

Gmail → OpenAI → JSON Parse → Router → Gmail Draft

---

## Technologies Used

- Make.com
- OpenAI
- Gmail
- JSON

---

## Email Categories

The workflow identifies:

- Support Request
- Pricing Inquiry
- Booking Request
- General Question

---

## Example Workflow

Incoming Email:

"How much does your service cost?"

Classification:

Pricing Inquiry

Generated Draft:

"Thank you for your inquiry. Pricing depends on the specific service requested. Please provide additional details and we will prepare a quote."

---

## What I Learned

- AI-powered email classification
- Draft response generation
- Workflow routing logic
- Gmail automation
- Structured data processing
- Human-in-the-loop automation

---

## Possible Improvements

- CRM integration
- Automatic follow-ups
- Sentiment analysis
- Priority scoring
- Multi-language support
- Knowledge base integration

---


## 📸 Screenshots

### Automation Architecture
![Architecture](screenshots/email-responder-automation-architecture.png)

### Router Logic
![Router](screenshots/email-responder-router-logic.png)

### Example Output (Gmail Draft)
![Output](screenshots/email-responder-gmail-draft.png)

