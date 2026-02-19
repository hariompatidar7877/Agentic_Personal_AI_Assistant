 Setup Guide

This guide explains how to set up and run the Agentic Personal AI Assistant using n8n.

---

 Prerequisites

Before starting, make sure you have:

- n8n installed (Cloud or Self-hosted)
- OpenAI API key
- Gmail account
- Google Cloud project with:
  - Gmail API enabled
  - Google Sheets API enabled
  - Google Calendar API enabled
- Telegram Bot Token

---

 Step 1: Install or Access n8n

You can either:

- Use n8n Cloud
OR
- Run locally using Docker or Node.js

Example (Docker):

```bash
docker run -it --rm \
  -p 5678:5678 \
  n8nio/n8n
