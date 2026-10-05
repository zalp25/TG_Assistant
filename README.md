# AI Assistant Workflow in n8n
<img width="1672" height="645" alt="image" src="https://github.com/user-attachments/assets/ad832a05-a7ee-485f-babb-ea43397c6d93" />

This project is a smart Telegram-based personal assistant built inside n8n. It connects a chat interface, AI reasoning, personal memory, and real-world tools like Google Calendar, Google Tasks, Gmail, and PostgreSQL.

In simple terms, this is not just a chatbot. It is a workflow that can actually act: it understands messages, processes voice notes, remembers important user information, schedules events, manages tasks, and helps with email-related actions.

This project is especially strong for a portfolio because it demonstrates a practical combination of:

- automation
- AI integration
- workflow orchestration
- API connectivity
- real productivity use cases

---

## What this project does

The assistant can:

- receive messages from Telegram;
- understand text and voice inputs;
- transcribe voice notes using OpenAI;
- store and retrieve user profile information from PostgreSQL;
- create, update, and manage Google Tasks;
- create and manage calendar events;
- read, search, and reply to Gmail messages;
- respond inside Telegram in a natural and helpful way.

This turns a normal messaging app into a personal productivity assistant.

---

## Why this is impressive

A lot of AI demos stop at “chat with the model.” This project goes further.

It connects AI with tools and real data, which is where automation becomes genuinely useful. Instead of only generating text, the assistant can act on the user’s behalf:

- schedule something for later;
- remember personal context;
- manage tasks;
- look up relevant information;
- reply to emails;
- process voice messages into usable content.

That is the difference between a simple chatbot and an intelligent workflow.

---

## Project overview

The workflow is built around a Telegram trigger, an AI Agent, and connected tools.

When a user sends a message, the system checks whether it is a text message or a voice note. If it is a voice note, the audio is downloaded and transcribed. Then the text is passed into the AI agent, which decides what the best action is.

The AI agent can then:

- answer directly;
- ask a clarifying question;
- fetch memory from the database;
- update profile data if the user asks for it;
- create a task;
- create or update a calendar event;
- search Gmail and reply to emails.

---

## How it works

### 1. Telegram receives the user input
The workflow starts when a message arrives in Telegram.

### 2. The system identifies the message type
It checks whether the input is:

- a normal text message;
- a voice message.

### 3. Voice messages are converted into text
If the user sends a voice note, the system downloads the file, sends it to OpenAI for transcription, and turns it into text that the AI can process.

### 4. The AI agent decides what to do
The AI evaluates the request and chooses the best path. It may:

- answer a question;
- request missing details;
- check user data;
- run a Google tool;
- update the database.

### 5. The assistant executes the right tool
Depending on the task, it can use:

- PostgreSQL for profile memory;
- Google Tasks for task management;
- Google Calendar for scheduling;
- Gmail for message actions.

### 6. The result is sent back to the user
Finally, the assistant responds in Telegram with the result.

---

## Key features

### Personal memory
The assistant stores user-specific information in PostgreSQL so it can remember important context over time. This makes interactions more personal and useful.

### Voice-first interaction
Voice notes are not ignored. They are transcribed and used like regular input, which makes the assistant feel more natural and modern.

### Task and calendar management
The workflow can manage daily productivity actions without requiring the user to open another platform.

### Email assistance
The assistant can search messages, get context, and reply to emails when relevant.

### AI-driven decision making
The biggest value is not just in the tools themselves but in the fact that the AI decides which tool to use and when.

---

## Example user journeys

### Example 1: Meeting planning
User: “Schedule a meeting tomorrow at 4 PM with my team.”

The system:

- interprets the request;
- creates a calendar event;
- confirms the result back to the user.

### Example 2: Voice assistant
User sends a voice note: “Remind me to finish the proposal before Friday.”

The system:

- transcribes the voice note;
- detects the task request;
- creates a task in Google Tasks;
- replies with confirmation.

### Example 3: Personal memory
User: “Remember that I study computer science and live in Kyiv.”

The system:

- stores the information in PostgreSQL;
- uses it later when helping with context-aware responses.

### Example 4: Email workflow
User: “Find the email from the recruiter and reply politely.”

The system:

- searches Gmail;
- finds the message;
- reads the content;
- drafts or sends a reply.

---

## What makes this project valuable

This workflow is valuable because it shows real-world AI automation in action.

It demonstrates that AI is not only for generating text, but for connecting to systems and completing actions. That is one of the strongest capabilities in modern automation.

For a portfolio, this project presents a person who can build:

- AI-powered workflows;
- business automation;
- integrations across tools;
- practical, user-centered systems;
- end-to-end logic from trigger to action.

---

## Technical stack

- n8n
- Telegram API
- OpenAI
- PostgreSQL
- Google Tasks
- Google Calendar
- Gmail
- AI agent orchestration

---

## Final note

This project represents a practical AI assistant that can operate inside a messaging app and connect with real tools. It blends communication, automation, and intelligence into one workflow.

That combination is exactly what makes it interesting for both users and employers: it shows not just theoretical AI knowledge, but the ability to design systems that solve actual problems in real environments.
