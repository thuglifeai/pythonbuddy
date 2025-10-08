# 🐍 PythonBuddy

[![Python](https://img.shields.io/badge/Python-3.11-blue.svg)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-3.0-green.svg)](https://flask.palletsprojects.com/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**Your AI-powered Python coding companion - Learn, code, and debug with instant help!**

PythonBuddy is a beginner-friendly Python learning assistant that combines rule-based keyword matching for instant responses with DeepSeek AI for complex questions. Perfect for Python learners of all levels!

![PythonBuddy Interface](https://img.shields.io/badge/Status-Production%20Ready-success)

## ✨ Features

### 🤖 Hybrid AI System
- **Rule-based responses** for 17+ Python topics (instant, no API cost)
- **DeepSeek AI integration** for complex questions, debugging, and custom requests
- Smart context-aware responses with chat history

### 💬 Chat Management
- **Multiple chat sessions** - Organize your learning by topic
- **Rename chats** - Customize names for different subjects (✏️ pencil icon)
- **Persistent storage** - All chats saved in localStorage (no login required)
- **Share conversations** - Generate shareable links for your chats
- **Export to .txt** - Download chat conversations as formatted text files

### 🎨 User Experience
- **Theme switcher** - Light/Dark/System modes with auto-detection
- **Responsive design** - Mobile-first, optimized for all devices
- **Clean interface** - ChatGPT-style chat experience
- **Quick-start buttons** - 6 example topics to get started instantly

### 🔒 Security & Performance
- **XSS protection** - escapeHtml() sanitization on all user inputs
- **Input validation** - Character limits and message caps
- **localStorage quota management** - Auto-cleanup to keep 5 most recent chats
- **No-cache headers** - Always serves latest updates
- **Debug mode OFF** - Production-ready deployment

## 📚 Python Topics Covered

- Print statements & output
- Variables & data types
- User input
- Error handling (try/except)
- Classes & OOP
- Imports & modules
- List operations (reverse, sort)
- File I/O (read/write)
- Loops (for, while)
- Functions
- Lists & dictionaries
- Strings & conditionals (if/else)
- **...and more with AI assistance!**

## 🚀 Quick Start

### Prerequisites
- Python 3.11+
- Flask
- OpenAI-compatible API (DeepSeek)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/thuglifeai/pythonbuddy.git
cd pythonbuddy
```

2. Install dependencies:
```bash
pip install flask gunicorn openai
```

3. Set up environment variables:
```bash
export DEEPSEEK_API_KEY="your-api-key-here"
export SESSION_SECRET="your-secret-key"
```

4. Run the application:
```bash
python app.py
```

5. Open your browser and navigate to:
```
http://localhost:5000
```

## 🏗️ Project Structure

```
pythonbuddy/
├── app.py              # Flask web server with share endpoints
├── main.py             # PythonBuddy class with keyword detection
├── templates/
│   ├── index.html      # Main chat interface
│   └── shared.html     # Public shared chat view
├── replit.md           # Project documentation & architecture
└── README.md           # This file
```

## 🛠️ Tech Stack

- **Backend:** Flask (Python 3.11)
- **AI:** DeepSeek API (OpenAI-compatible)
- **Frontend:** Vanilla JavaScript, CSS3
- **Storage:** localStorage (client-side)
- **Deployment:** Gunicorn (autoscale)

## 🎯 How It Works

1. **Keyword Detection:** User questions are scanned for Python-related keywords
2. **Rule-based Response:** If matched, instant code examples are provided
3. **AI Fallback:** Complex questions route to DeepSeek AI with chat context
4. **Smart Context:** Chat history maintains conversation flow
5. **Auto-naming:** First question becomes chat title automatically

## 🔑 Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `DEEPSEEK_API_KEY` | DeepSeek API key for AI responses | Yes |
| `SESSION_SECRET` | Flask session secret key | Yes |

## 📖 Usage Examples

**Basic Questions (Rule-based - Instant):**
- "How do I print Hello World?"
- "How do I create a variable?"
- "How do I reverse a list?"

**Complex Questions (AI-powered):**
- "Debug this code: [paste your code]"
- "Explain decorators with examples"
- "How do I build a REST API in Python?"

## 🌐 Deployment

### Production Deployment with Gunicorn

```bash
gunicorn --bind 0.0.0.0:5000 --reuse-port app:app
```

### Deploy on Replit
1. Import this repository to Replit
2. Add secrets: `DEEPSEEK_API_KEY`, `SESSION_SECRET`
3. Click "Run" - it's configured for autoscale deployment!

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new Python topics
- Improve the AI prompts
- Enhance the UI/UX

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Python community for inspiration
- DeepSeek for AI capabilities
- Flask framework for simplicity
- Replit for hosting platform

## 📧 Contact

**ThugLife.AI** - Building AI-powered learning tools

- GitHub: [@thuglifeai](https://github.com/thuglifeai)
- Project: [PythonBuddy](https://github.com/thuglifeai/pythonbuddy)

---

**Made with ❤️ for Python learners worldwide** 🐍✨
