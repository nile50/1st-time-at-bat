# GPT Chatbot

A web-based chatbot powered by OpenAI's GPT models, built with Python (Flask).

## Setup

```bash
# 1. Install dependencies
pip install -r requirements.txt

# 2. Copy and fill in your API key
cp .env.example .env
# edit .env — set OPENAI_API_KEY

# 3. Run
python app.py
# Open http://localhost:5000
```

## Configuration (`.env`)

| Variable | Default | Description |
|---|---|---|
| `OPENAI_API_KEY` | *required* | Your OpenAI API key |
| `OPENAI_MODEL` | `gpt-4o-mini` | Model to use (e.g. `gpt-4o`) |
| `FLASK_SECRET_KEY` | `change-me-in-production` | Session signing key |
| `FLASK_DEBUG` | `false` | Enable Flask debug mode |
| `PORT` | `5000` | Port to listen on |
| `SYSTEM_PROMPT` | "You are a helpful assistant." | Bot persona / instructions |

## Features

- Typing indicator while the bot responds
- Full conversation history per browser session
- "New chat" button to reset the conversation
- Auto-growing textarea; Enter to send, Shift+Enter for newline
