🤖 Agentic Personal AI Assistant (n8n + OpenAI)
An advanced multi-agent personal AI assistant built using n8n that integrates OpenAI, Gmail, Google Sheets, Google Calendar, and Telegram.

This system is designed using a modular agent architecture where a main AI assistant intelligently routes user requests to specialized sub-agents for email handling and calendar management.

🚀 Key Features
📩 Send, read, and draft emails via Gmail
📅 Create and retrieve Google Calendar events
📇 Contact verification using Google Sheets database
🎙 Voice message transcription support
💬 Context-aware conversations with memory
🔁 Modular multi-agent workflow design
🛡 Error-safe contact validation before execution
🧠 System Architecture
The system follows a multi-agent orchestration model:

Main Assistant

Receives user input from Telegram (text or voice)
Uses OpenAI for reasoning and intent classification
Routes tasks to appropriate sub-agents
Email Agent

Handles email-related actions
Integrates with Gmail API
Fetches contact details from Google Sheets before sending
Calendar Agent

Handles event scheduling and retrieval
Integrates with Google Calendar API
Automatically assumes 60-minute duration if not specified
🛠 Tech Stack
n8n (Workflow Automation)
OpenAI (GPT-4.1-mini)
Gmail API
Google Sheets API
Google Calendar API
Telegram Bot API
📂 Project Structure
personal-ai-assistant-n8n/ │ ├── README.md | | │ ├── workflows/ │ ├── main-assistant.json │ ├── email-agent.json │ └── calendar-agent.json │ ├── docs/ │ ├── system-design.md │ ├── tools-used.md │ └── setup-guide.md │ └── assets/ ├── main-workflow.png ├── email-agent.png └── calendar-agent.png

⚙️ How It Works
User sends a message via Telegram.
The Main Assistant processes the input.
The system verifies contact information (if required).
The appropriate sub-agent executes the task:
Email Agent → Gmail actions
Calendar Agent → Event scheduling
Response is returned to the user.
🔐 Setup Instructions
Import all workflows from the /workflows folder into n8n.
Configure credentials for:
OpenAI
Gmail OAuth2
Google Sheets OAuth2
Google Calendar OAuth2
Telegram Bot
Activate all workflows.
Start interacting via Telegram.
📌 Design Principles
Modular architecture
Tool-based reasoning
Contact validation before execution
Error prevention and professional communication
Clean separation of responsibilities between agents
👨‍💻 Author
Hariom Patidar

📜 License
This project is for educational and demonstration purposes.
