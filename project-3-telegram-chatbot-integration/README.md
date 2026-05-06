# Telegram AI Chatbot Workflow

## 🎥 Demo Video

Short walkthrough of the workflow and how it operates.

👉 [▶️ Watch Demo Video](https://www.loom.com/share/42a9d0174df54f97813f2abae811ca06)



## Problem

Handling repetitive user questions manually can slow down response times and create repetitive communication tasks.

This workflow was built to automate message handling and route responses based on user intent.



## Workflow Overview

When a user sends a message through Telegram, the workflow sends the content to OpenAI for intent classification.

The response is converted into structured data and routed through different workflow paths based on the detected intent.

Automated responses are then returned through Telegram based on the selected workflow route.



## 🏗️ Architecture

Telegram → OpenAI → Data Processing → Router → Telegram Response

This workflow uses routing logic to organize different types of user requests and automate response handling through Telegram.

Different workflow paths are triggered based on the detected intent.



## 🛠️ Tech Stack

- Make (Integromat)
- OpenAI API
- Telegram Bot API
- Webhooks



## 🚀 Key Features

- Automated intent classification
- Telegram chatbot integration
- Routing logic for different request types
- Structured message processing
- Automated response workflows



## Outcome

This workflow automates repetitive message handling and helps organize user interactions through structured routing and response automation.



## Possible Improvements

Future improvements could include:
- improved handling of unclear user requests
- memory and conversation history support
- additional routing conditions
- integration with external knowledge sources
- stronger validation for unexpected inputs



## What I Learned

- Building chatbot-based automation workflows
- Structuring AI responses into workflow actions
- Using routing logic for conversational flows
- Organizing automated user interaction processes




## 📸 Screenshots

### Automation Architecture
![Architecture](screenshots/telegram-chatbot-architecture.png)

### Router Logic
![Router](screenshots/telegram-chatbot-router.png)

### Example Output
![Output](screenshots/telegram-chatbot-output.png)
