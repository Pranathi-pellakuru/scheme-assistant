# 🇮🇳 SchemeSahayak - Government Scheme Assistant

AI-powered assistant to help Indians discover and apply for government schemes and benefits.

![SchemeSahayak](https://img.shields.io/badge/AI-Powered-blue)
![Status](https://img.shields.io/badge/Status-Live-success)
![License](https://img.shields.io/badge/License-MIT-green)

## 🌟 Features

- **15+ Government Schemes** - Agriculture, Healthcare, Education, Business, Housing
- **AI-Powered Search** - Smart recommendations using Ollama (Llama 3.2)
- **Vector Database** - ChromaDB for semantic search
- **Beautiful UI** - Modern, responsive chat interface
- **100% Free** - No API costs, runs locally
- **Privacy First** - Your data stays on your machine

## 🚀 Live Demo

**Frontend:** [Your Railway/Render URL will go here]  
**API Docs:** [Your Railway/Render URL]/docs

## 📸 Screenshots

[Add screenshots here after deployment]

## 🛠️ Tech Stack

**Backend:**
- FastAPI - REST API framework
- Ollama (Llama 3.2) - Local LLM
- ChromaDB - Vector database
- LangChain - AI orchestration

**Frontend:**
- HTML5/CSS3/JavaScript
- Modern responsive design
- Real-time chat interface

**DevOps:**
- Docker & Docker Compose
- GitHub Actions (coming soon)
- Railway/Render deployment

## 💻 Local Installation

### Prerequisites
- Python 3.11+
- Ollama installed
- Git

### Quick Start

1. **Clone the repository**
```bash
git clone https://github.com/YOUR_USERNAME/scheme-assistant.git
cd scheme-assistant
```

2. **Create virtual environment**
```bash
python -m venv venv

# Windows
venv\Scripts\activate

# Mac/Linux
source venv/bin/activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Install Ollama and pull model**
```bash
# Install from https://ollama.com
ollama pull llama3.2
```

5. **Load schemes into database**
```bash
python src/scraper.py
python src/database.py
```

6. **Start the API server**
```bash
python src/api.py
```

7. **Open the frontend**
- Open `frontend/index.html` in your browser
- Or visit `http://localhost:8000` if serving

## 🐳 Docker Deployment

### Using Docker Compose (Recommended)
```bash
docker-compose up -d
```

Access at: `http://localhost:8000`

### Manual Docker Build
```bash
# Build image
docker build -t scheme-assistant .

# Run container
docker run -p 8000:8000 scheme-assistant
```

## 📚 API Documentation

Once running, visit `http://localhost:8000/docs` for interactive API documentation.

### Example API Call
```bash
curl -X POST "http://localhost:8000/chat" \
  -H "Content-Type: application/json" \
  -d '{"message": "I am a farmer, what schemes can help me?"}'
```

## 🗂️ Project Structure
```
scheme-assistant/
├── data/
│   └── schemes_data.json       # Government schemes database
├── frontend/
│   └── index.html              # Chat UI
├── src/
│   ├── database.py             # Vector database setup
│   ├── agent.py                # AI agent logic
│   ├── api.py                  # FastAPI server
│   └── scraper.py              # Scheme data collection
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
└── README.md
```

## 🎯 Roadmap

- [ ] Add 100+ government schemes
- [ ] Multilingual support (Hindi, Tamil, Telugu, etc.)
- [ ] WhatsApp bot integration
- [ ] User authentication
- [ ] Application tracking
- [ ] SMS/Email notifications
- [ ] Mobile app (React Native)
- [ ] Voice assistant integration

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Varun Bhargav**
- LinkedIn: [LinkedIn](https://www.linkedin.com/in/varun-bhargav-moori-90337a186)

## 🙏 Acknowledgments

- Government of India for scheme information
- Anthropic for Claude AI assistance
- Ollama for local LLM capabilities
- FastAPI community

## 📞 Support

For support open an issue on GitHub.

---

**Made with ❤️ for India**
