# AI Content Generation Workflow

## 🎥 Demo Video

Short walkthrough of the workflow and how it operates.

👉 [▶️ Watch Demo Video](https://www.loom.com/share/ef67952808ef45ffab1025ac888e3695)



## Problem

Preparing repetitive content manually can slow down operational or marketing workflows, especially when content needs to follow a consistent structure and delivery process.


## Workflow Overview

When a content request is submitted, the workflow sends the prompt to OpenAI for content generation.

The response is processed and formatted automatically before being routed for delivery.

Completed content is then sent through Telegram for review or publishing preparation.


## 🏗️ Architecture

Webhook → OpenAI → Data Processing → Formatter → Telegram Delivery

This workflow uses automated routing and formatting steps to organize generated content before delivery through Telegram.

Different routing paths can be triggered depending on the type of content requested.



## 🛠️ Tech Stack

- Make (Integromat)
- OpenAI API
- Telegram Bot API
- Webhooks



## Key Workflow Functions

- Automated content generation using OpenAI
- Structured content formatting
- Routing logic for different content requests
- Telegram delivery integration



## Outcome

This workflow reduces repetitive content preparation tasks by automating content generation, formatting, and delivery into a structured process.



## Possible Improvements

Future improvements could include:
- improved handling of unclear content requests
- additional formatting and content templates
- integration with publishing or CMS platforms
- stronger validation for generated outputs
- scheduling and approval workflows before publishing



## What I Learned

- Building automated content workflows using OpenAI
- Structuring generated content into organized outputs
- Using routing logic for content handling processes
- Organizing automated delivery workflows



## 📸 Screenshots

### Automation Architecture
![Architecture](screenshots/content-generator-architecture.png)

### Content Processing Flow
![Processing](screenshots/content-generator-processing.png)

### Example Output
![Output](screenshots/content-generator-output.png)
