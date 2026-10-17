# Ollama Conversational Chatbot

A command-line AI chatbot built with Python, Ollama, and the Qwen 3.5 (0.8B) language model. The chatbot maintains conversation history to provide context-aware responses throughout a session.

## Features

- Interactive terminal-based conversation.
- Local AI inference using Ollama.
- Conversation history maintained during the session.
- Simple, clear, and informative responses.
- Configurable response temperature.
- Type `exit` to end the conversation.

## Technologies Used

- Python
- Ollama
- Qwen 3.5 (0.8B)
- Ollama Python client

## Prerequisites

- Python installed on your computer.
- Ollama installed and running.
- The `qwen3.5:0.8b` model downloaded locally.

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/ollama-conversational-chatbot.git
cd ollama-conversational-chatbot
```

Replace `YOUR-USERNAME` with your GitHub username.

### 2. Install the Python dependency

```bash
pip install -r requirements.txt
```

### 3. Install and prepare Ollama

Download Ollama from https://ollama.com/download.

Pull the model:

```bash
ollama pull qwen3.5:0.8b
```

Ensure the Ollama service is running before starting the chatbot.

### 4. Run the chatbot

```bash
python chatbot.py
```

### 5. Start chatting

Enter a question when prompted. Continue asking questions to maintain the conversation, or type `exit` to quit.

## Project Structure

```text
ollama-conversational-chatbot/
├── chatbot.py
├── requirements.txt
├── README.md
└── .gitignore
```

## How It Works

1. Connects to the local Ollama service.
2. Initializes the system instruction and conversation history.
3. Accepts user messages in a loop.
4. Sends the conversation history to the Qwen model.
5. Displays the generated answer.
6. Adds the assistant response to the history for subsequent messages.

## Learning Objectives

- Integrate Python with a local language model.
- Use the Ollama chat API.
- Maintain conversation context using message history.
- Build an interactive command-line application.
- Understand model generation settings.

## Limitations

- Ollama must be installed and running locally.
- The selected model must be downloaded.
- Response quality and speed depend on the model and computer hardware.
- Conversation history is stored in memory and is lost when the program exits.

## Author

Add your name and GitHub profile here.
