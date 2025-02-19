Here's your updated **README** with the new section added at the top, ensuring correct Markdown formatting:  

---

# Razor: AI-Powered Personal Task Manager

## Overview
Razor is a personal AI-driven task manager designed to help efficiently manage daily tasks through natural language interactions. It provides a seamless experience where users can inquire about, edit, organize, and track tasks categorized by different contexts without disrupting their workflow.

## Motivation
I often find myself deep in the flow, encountering bugs or enhancements that need attention ASAP. But stopping to log them disrupts my momentum. Razor serves as an AI-powered assistant that allows me to:

- **Bark out annoying tasks I know I need to do later—without breaking focus**
- **Ask about tasks at any time**
- **Manage a structured database of tasks categorized by context**
- **Quickly add, edit, update, and reorganize tasks**
- **Filter tasks by specific dates or categories**

## Features
- **Natural language interaction**: Query and update tasks using conversational commands.
- **Task categorization**: Organize tasks under different categories for better tracking.
- **Status management**: Easily update task statuses (`pending`, `in_progress`, `completed`).
- **Daily focus mode**: Get a snapshot of tasks relevant to the current day.
- **Database-backed storage**: Uses SQLite to store and persist task data.

## Technology Stack
- **SQLite**: Lightweight and efficient database storage.
- **n8n Workflow Automation**: Orchestrates task management and processing.
- **Ollama**: AI model integration to facilitate natural language understanding.
- **Custom AI Prompts**: Defines Razor’s role as an intelligent task manager.

## Getting Started
### Prerequisites
- n8n (workflow management)
- Vosk (speech-to-text translation)
- Node.js
- SQLite3
- Ollama LLM (local AI model hosting, initially)

### Setup
1. Clone this repository:
   ```sh
   git clone <repo-url>
   cd jarvis-task-manager
   ```
2. Install dependencies (if applicable).
3. Set up the SQLite database:
   ```sh
   sqlite3 jarvis.db < schema.sql
   ```
4. Configure n8n workflows to interact with the database.
5. Start using Razor to manage your tasks!

## Usage Examples
- **Adding a Task:**
  ```
  "Razor, add a new task to the 'Development' category: Fix login authentication bug."
  ```
- **Checking Tasks for Today:**
  ```
  "Razor, what are my tasks for today?"
  ```
- **Updating a Task’s Status:**
  ```
  "Razor, mark the task 'Fix login authentication bug' as completed."
  ```

## Roadmap
- [ ] Improve AI contextual understanding
- [ ] Add voice command support
- [ ] Implement task prioritization and scheduling
- [ ] Expand integrations with external project management tools
- [ ] Enhance UI for task visualization


## License
MIT License
