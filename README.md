<div align="center">

⚡ AESUN AI ASSISTANT

Next-Generation Personal AI Command Center

An intelligent, agentic AI assistant built with Python, Gemini, Groq, LangChain, voice interaction, semantic memory, task automation, and a futuristic web interface.

<br/>








<br/>

🧠 Think. Remember. Act. Automate.

AESUN is designed to go beyond simple chatbot conversations by combining AI reasoning, memory, voice interaction, and productivity automation in one system.

</div>

🎮 Experience AESUN

AESUN is built as a personal AI command center rather than a basic chat application.

The system can understand normal conversations, use an agent for action-oriented requests, remember previous interactions through vector search, manage tasks and reminders, and interact through voice.

✨ Core Capabilities

Capability

What AESUN Does

🧠 AI Conversation

Generates contextual responses using Google Gemini

🤖 Agentic AI

Uses LangChain + Groq for action-oriented requests

🗂️ Task Management

Create, view, filter, and update task status

⏰ Smart Reminders

Schedule reminders and trigger them automatically

🎙️ Speech-to-Text

Accepts voice commands through microphone input

🔊 Text-to-Speech

Responds using voice output

🧩 Wake Word

Supports "Aesun" activation in continuous mode

🔎 Semantic Memory

Searches previous conversations using embeddings + FAISS

👤 User Context

Tracks preferences, frequent topics, and conversation history

🌐 Web Dashboard

Flask-powered futuristic AI interface

💾 Persistent Storage

Stores conversations, tasks, reminders, and vector data

🧠 How AESUN Works

                         ┌──────────────────────┐
                         │      USER INPUT      │
                         │   Text / Voice       │
                         └──────────┬───────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │    AESUN ENGINE      │
                         │  Input Processing    │
                         └──────────┬───────────┘
                                    │
                   ┌────────────────┴────────────────┐
                   │                                 │
                   ▼                                 ▼
          ┌──────────────────┐              ┌──────────────────┐
          │  Normal Query    │              │ Action / Memory │
          │     Gemini       │              │  Groq + Agent   │
          └────────┬─────────┘              └────────┬─────────┘
                   │                                 │
                   └────────────────┬────────────────┘
                                    ▼
                         ┌──────────────────────┐
                         │   Context + Memory   │
                         │ Sentence Transformer │
                         │       + FAISS        │
                         └──────────┬───────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │   RESPONSE / ACTION  │
                         │ Chat • Voice • Task  │
                         │ Reminder • Search    │
                         └──────────────────────┘

🚀 What Makes AESUN Different?

01 — Context-Aware Conversations

AESUN maintains a short conversational chain for follow-up interactions and stores conversations for later retrieval.

02 — Agentic Task Execution

Action-oriented requests can be routed through a LangChain ReAct agent powered by Groq.

The agent has tools for:

Add tasks

Get tasks

List tasks

Update task status

Add reminders

Get reminders

Search previous conversations

Retrieve user context

03 — Long-Term Semantic Memory

Conversation data is converted into embeddings using:

Sentence Transformers
        ↓
all-MiniLM-L6-v2
        ↓
FAISS Vector Index
        ↓
Semantic Conversation Search

This allows AESUN to retrieve conversations based on meaning, rather than relying only on exact keyword matching.

04 — Voice Interaction

AESUN supports:

🎙️ Speech recognition

🔊 Text-to-speech

🟢 Wake-word activation

😴 Sleep/deactivation command

🔄 Continuous listening mode

Wake word:

Aesun

Sleep command:

Aesun go back to sleep

🖥️ Tech Stack

AI / Machine Learning

Google Gemini

Groq

LangChain

Sentence Transformers

FAISS

Backend

Python

Flask

Flask-CORS

REST API

Voice

SpeechRecognition

PyAudio

pyttsx3

Data

Pandas

NumPy

Excel / XLSX

Pickle

FAISS index

Frontend

HTML5

CSS3

JavaScript

Glassmorphism / futuristic HUD UI

Neon gaming-style visual system

📁 Project Structure

Ai Assistent (AESUN)/
│
├── Aesun_ai.py
│   └── Core AI engine
│
├── app.py
│   └── Flask backend + REST APIs
│
├── requirements.txt
│   └── Python dependencies
│
├── .env
│   └── API credentials
│
├── Aesun_data/
│   ├── conversations.xlsx
│   ├── tasks.xlsx
│   ├── reminders.xlsx
│   ├── tasks.txt
│   ├── vector_db.pkl
│   └── faiss_index.idx
│
└── static/
    └── index.html

⚠️ Do not commit .env, API keys, personal conversation data, or generated database files to a public repository.

⚙️ Installation

1. Clone the repository

git clone https://github.com/YOUR_USERNAME/AESUN-AI-ASSISTANT.git
cd AESUN-AI-ASSISTANT

2. Create a virtual environment

Windows

python -m venv venv
venv\Scripts\activate

macOS / Linux

python3 -m venv venv
source venv/bin/activate

3. Install dependencies

pip install -r requirements.txt

Depending on your operating system, PyAudio may require additional system-level audio dependencies.

🔐 Environment Variables

Create a .env file in the project root:

GEMINI_API_KEY=your_gemini_api_key
GROQ_API_KEY=your_groq_api_key

Never expose API keys

Do not put real API keys directly inside:

Aesun_ai.py

app.py

index.html

GitHub commits

Recommended .gitignore:

.env
venv/
__pycache__/
*.pyc

Aesun_data/*.xlsx
Aesun_data/*.pkl
Aesun_data/*.idx

▶️ Run AESUN

Start the Flask server:

python app.py

The backend runs on:

http://localhost:4000

Open the AESUN interface in your browser:

http://localhost:4000

🔌 API Endpoints

Method

Endpoint

Purpose

POST

/api/conversation

Process AI conversation

GET

/api/tasks

Retrieve tasks

POST

/api/tasks

Create a task

PUT

/api/tasks/update

Update task status

GET

/api/tasks/all

Retrieve all tasks

GET

/api/reminders

Retrieve reminders

POST

/api/reminders

Create reminder

GET

/api/conversations

Retrieve conversation history

POST

/api/search

Semantic conversation search

GET

/api/status

System status

POST

/api/voice/process

Voice processing endpoint

GET

/api/user-context

Retrieve user context

💬 Example Commands

Try asking AESUN:

Hello Aesun

Create a task to finish my AI project

Show my pending tasks

Mark task 1 as completed

Remind me to attend the meeting at 18:30

What did we discuss about my previous project?

Search my previous conversations about machine learning

🧩 Agent Tools

AESUN's agent can interact with its internal productivity and memory tools:

┌─────────────────────────────┐
│       AESUN AGENT           │
├─────────────────────────────┤
│ add_task                    │
│ get_tasks                   │
│ list_tasks                  │
│ update_task                 │
│ add_reminder                │
│ get_reminders               │
│ search_conversations        │
│ get_user_context            │
└─────────────────────────────┘

This enables AESUN to take actions, not just generate text.

💾 Data & Memory

AESUN persists information using local files.

Conversations

Aesun_data/conversations.xlsx

Tasks

Aesun_data/tasks.xlsx

Reminders

Aesun_data/reminders.xlsx

Semantic Memory

Aesun_data/vector_db.pkl
Aesun_data/faiss_index.idx

This allows the assistant to preserve useful information between application sessions.

🎨 Interface

The web interface is designed as a futuristic AI command center with:

⚡ Neon gaming aesthetics

🔮 Animated AI core

🧊 Glassmorphism panels

🎙️ Voice interaction indicator

📊 System metrics

📋 Live task panel

🚨 Priority reminder panel

🌌 Dark cyber interface

Tip: Add your best UI screenshot/GIF here after uploading it to the repository.

![AESUN Dashboard](./assets/aesun-dashboard.png)

🛡️ Security Notes

AESUN uses external AI services and local persistent data.

Before publishing the repository:

Remove all real API keys.

Add .env to .gitignore.

Do not upload private conversation history.

Do not upload personal reminders/tasks.

Do not publish private credentials.

Regenerate any API key that has accidentally been exposed.

🗺️ Future Improvements

Potential upgrades for the next version:

Streaming AI responses

Real-time WebSocket communication

Authentication & user profiles

Cloud database

Better multilingual voice support

Advanced memory management

Mobile application

Desktop application

More agent tools

Calendar integration

Email automation

Smart home integrations

Local LLM support

RAG document assistant

GPU-accelerated local inference

👨‍💻 Developer

<div align="center">

Ashwin Kumar

AI/ML Engineer • Full-Stack Developer

Building intelligent systems that combine AI, automation, voice interaction, and modern web technologies.

<br/>




</div>

<div align="center">

⚡ AESUN

"Think. Remember. Act. Automate."

⭐ If you find this project interesting, consider giving it a star!

</div>
