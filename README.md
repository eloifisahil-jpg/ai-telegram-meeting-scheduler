# 🤖 AI Telegram Meeting Scheduler

An intelligent Telegram bot that automates meeting scheduling using Google Gemini AI, Google Calendar integration, and employee database management.

## ✨ Features

- **🗣️ Natural Language Processing**: Chat naturally with the bot using conversational language
- **📅 Google Calendar Integration**: Automatically creates and manages calendar events
- **📧 Email Notifications**: Sends meeting confirmations to attendees via Gmail
- **👥 Employee Database**: Integrates with Google Sheets for employee information lookup
- **🧠 Context Memory**: Maintains conversation history for better understanding
- **⚡ Real-time Processing**: Instant responses powered by Google Gemini 2.5

## 🛠️ Technology Stack

- **Automation Platform**: n8n workflow automation
- **AI Model**: Google Gemini 2.5 (via LangChain)
- **Messaging**: Telegram Bot API
- **Calendar**: Google Calendar API
- **Email**: Gmail API
- **Database**: Google Sheets API
- **Memory Management**: Buffer Window Memory (LangChain)

## 📋 Workflow Components

1. **Telegram Trigger**: Receives and processes incoming messages
2. **Google Gemini AI Agent**: Interprets user intent and generates responses
3. **Google Calendar Tool**: Creates and manages calendar events
4. **Gmail Tool**: Sends email notifications to meeting participants
5. **Google Sheets Tool**: Reads employee data for scheduling
6. **Memory Buffer**: Maintains conversation context

## 🚀 Use Cases

- Schedule meetings with team members via Telegram chat
- Set up reminders for upcoming events
- Query employee availability and contact information
- Automatically send meeting invitations and confirmations
- Manage calendar events through conversational interface

## 📦 Installation

### Prerequisites

- n8n instance (self-hosted or cloud)
- Telegram Bot Token
- Google Cloud Project with enabled APIs:
  - Gmail API
  - Google Calendar API
  - Google Sheets API
  - Google Gemini (PaLM) API

### Setup Steps

1. **Import Workflow**
   ```bash
   # Download the workflow JSON file
   # Import it into your n8n instance via Settings > Import Workflow
   ```

2. **Configure Credentials**
   - Telegram Bot API (create bot via @BotFather)
   - Google OAuth2 for Calendar, Gmail, and Sheets
   - Google Gemini API key

3. **Set Up Google Sheets Database**
   - Create a Google Sheet with employee information
   - Update the document ID in the workflow

4. **Activate Workflow**
   - Enable the workflow in n8n
   - Test with your Telegram bot

## 💬 Example Usage

**User**: Schedule a meeting with Alex tomorrow at 10 AM
**Bot**: Meeting with Alex scheduled for tomorrow at 10 AM. Notification sent.

**User**: Set a reminder for the team standup at 9 AM daily
**Bot**: Daily reminder set for team standup at 9 AM.

## 🔧 Customization

- Modify the AI system prompt to adjust bot personality
- Add additional tools for extended functionality
- Configure notification templates in Gmail tool
- Adjust memory window size for context retention

## 📝 License

MIT License - feel free to use and modify for your projects

## 👤 Author

**Eloi Fisahil**
- Automation Specialist & n8n Expert
- 🔗 [Gumroad](https://gumroad.com/eloifisahil)
- 💼 Available for freelance automation projects

## 🤝 Contributing

Feel free to submit issues, fork the repository, and create pull requests for any improvements.

---

*Built with ❤️ using n8n workflow automation*
