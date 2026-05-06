# AI Content Generation Workflow

## 🎥 Demo Video

Short walkthrough of the workflow and how it operates.

👉 [▶️ Watch Demo Video](https://www.loom.com/share/ef67952808ef45ffab1025ac888e3695)



## Problem

Creating repetitive written content manually can take time and slow down publishing workflows, especially when content needs to follow a consistent structure or format.

This workflow was built to automate content generation and delivery using structured AI prompts and workflow automation.



## Workflow Overview

When a content request is submitted, the workflow sends the prompt to OpenAI for content generation.

The generated content is converted into structured output and routed through the workflow for formatting and delivery.

Completed content is then sent automatically through Telegram for review or publishing preparation.



## 🏗️ Architecture

Webhook → OpenAI → Data Processing → Formatter → Telegram Delivery

This workflow uses structured prompts and routing logic to automate content generation and organize delivery through Telegram.

Different workflow paths can be triggered depending on the requested content type or format.



## 🛠️ Tech Stack

- Make (Integromat)
- OpenAI API
- Telegram Bot API
- Webhooks



## 🚀 Key Features

- Automated AI content generation
- Structured content formatting
- Workflow routing for different content types
- Telegram delivery integration
- Automated content handling workflows



## Outcome

This workflow helps reduce repetitive content preparation tasks and supports faster content organization and delivery through automation.



## Possible Improvements

Future improvements could include:
- improved handling of unclear content requests
- additional formatting and content templates
- integration with publishing or CMS platforms
- stronger validation for generated outputs
- scheduling and approval workflows before publishing



## What I Learned

- Building AI-assisted content automation workflows
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
