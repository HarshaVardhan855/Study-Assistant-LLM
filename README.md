# 🎓 Study Assistant LLM

> An intelligent AI-powered Study Assistant that breaks down complex concepts into simple, easy-to-understand explanations using Google Gemini API and Gradio.

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Google Gemini](https://img.shields.io/badge/Google-Gemini%20API-orange.svg)](https://ai.google.dev/)
[![Gradio](https://img.shields.io/badge/Gradio-Web%20UI-green.svg)](https://www.gradio.app/)

## ✨ Features

- 🤖 **AI-Powered Explanations** - Uses Google Gemini 2.5 Flash for intelligent responses
- 👥 **Multiple Personalities** - Choose between friendly or academic teaching styles
- 🎨 **Interactive Web Interface** - User-friendly Gradio interface
- 📚 **Clear Explanations** - Gets complex topics explained simply with analogies and real-world examples
- ❓ **Follow-up Questions** - AI asks questions to verify your understanding
- ⚡ **Fast & Reliable** - Quick response times with advanced LLM model

## 🎯 How It Works

```
┌─────────────────────────────────────────────────────────────┐
│                    User Question Input                       │
└────────────────────┬────────────────────────────────────────┘
                     │
                     ▼
┌─────────────────────────────────────────────────────────────┐
│              Select Learning Personality                     │
│  ┌──────────────────────────────────────────────────────┐   │
│  │ • Friendly: Simple & Encouraging Explanations       │   │
│  │ • Academic: Detailed & Professional Approach        │   │
│  └──────────────────────────────────────────────────────┘   │
└────────────────────┬──────��─────────────────────────────────┘
                     │
                     ▼
┌─────────────────────────────────────────────────────────────┐
│           Google Gemini 2.5 Flash API Processing            │
│  • Applies personality-specific system prompt               │
│  • Generates contextual and relevant explanations           │
│  • Includes analogies and real-world examples               │
└────────────────────┬────────────────────────────────────────┘
                     │
                     ▼
┌─────────────────────────────────────────────────────────────┐
│                    AI Response Display                       │
│  • Clear explanation with real-world examples               │
│  • Follow-up question to check understanding                │
│  • Formatted for easy reading                               │
└─────────────────────────────────────────────────────────────┘
```

## 📋 Prerequisites

Before you start, make sure you have:

- **Python 3.8 or higher** installed
- **Google Gemini API Key** ([Get it here](https://ai.google.dev/))
- **pip** (Python package manager)

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/HarshaVardhan855/Study-Assistant-LLM.git
cd Study-Assistant-LLM
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

**Dependencies:**
- `google-genai` - Google Generative AI Python SDK
- `gradio` - Web UI framework for ML models

### 3️⃣ Set Up Your API Key

Create a `.env` file in the project root:

```bash
echo "GEMINI_API_KEY=your_api_key_here" > .env
```

**Or** set it as an environment variable:

```bash
# Windows
set GEMINI_API_KEY=your_api_key_here

# macOS/Linux
export GEMINI_API_KEY=your_api_key_here
```

### 4️⃣ Run the Application

```bash
python app.py
```

The application will start and display:

```
Running on local URL:  http://127.0.0.1:7860
```

Open your browser and navigate to the URL to access the interactive interface.

## 💡 How to Use

1. **Enter Your Question** - Type your question in the text box
   - Example: "What is photosynthesis?"
   - Example: "Explain quantum computing"

2. **Select a Personality** - Choose your preferred learning style:
   - **Friendly** 👋 - Simple, encouraging, beginner-friendly
   - **Academic** 📖 - Detailed, professional, university-level

3. **Get Your Explanation** - The AI provides:
   - Clear, concise explanation
   - Real-world examples and analogies
   - Follow-up question to verify understanding

4. **Ask More Questions** - Keep learning and asking!

## 📁 Project Structure

```
Study-Assistant-LLM/
│
├── app.py                    # Main application file
├── requirements.txt          # Python dependencies
└── README.md                 # Project documentation
```

## 🔧 Configuration Details

### System Prompts by Personality

#### Friendly Personality
- Friendly, enthusiastic, and encouraging tone
- Breaks down complex concepts into simple explanations
- Uses analogies and real-world examples
- Beginner-friendly language

#### Academic Personality
- Strictly academic and professional tone
- Detailed explanations with formal terminology
- University-level complexity
- Structured and citation-ready responses

### Model Configuration

```python
Model: gemini-2.5-flash
Temperature: 0.4 (Balanced between creativity and consistency)
Max Output Tokens: 2000 (Comprehensive responses)
```

## 🎨 User Interface

The application uses **Gradio** to provide:

- **Simple Input** - Text area for question entry (4 lines)
- **Personality Selector** - Radio buttons for teaching style selection
- **Large Output Display** - 10-line text area for AI responses
- **Professional Design** - Clean, intuitive layout
- **Real-time Processing** - Instant feedback

## 🛠️ Troubleshooting

### Issue: "API Key Not Found"
**Solution:** Ensure your `GEMINI_API_KEY` environment variable is set correctly.

### Issue: Module Import Errors
**Solution:** Reinstall dependencies:
```bash
pip install --upgrade -r requirements.txt
```

### Issue: Slow Responses
**Solution:** This is normal for the first request. Subsequent requests are faster.

### Issue: Port Already in Use
**Solution:** Specify a different port:
```python
demo.launch(debug=True, server_port=7861)
```

## 🔐 Security Best Practices

- ✅ Never commit your `.env` file or API key to GitHub
- ✅ Add `.env` to `.gitignore` file
- ✅ Use environment variables for sensitive data
- ✅ Keep your dependencies updated

## 📈 Future Enhancements

- [ ] Add conversation history storage
- [ ] Support for multiple languages
- [ ] Add voice input/output support
- [ ] Implement user authentication
- [ ] Add quiz generation feature
- [ ] Support for file uploads (PDFs, images)
- [ ] Response customization options

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest features
- Submit pull requests

## 📄 License

This project is open source and available under the MIT License.

## 📞 Support

If you encounter any issues or have questions:
- Check the Troubleshooting section
- Review Google Gemini API documentation
- Open an issue on GitHub

## 🙏 Acknowledgments

- [Google Gemini API](https://ai.google.dev/) - For powerful AI capabilities
- [Gradio](https://www.gradio.app/) - For amazing web UI framework
- [Python](https://www.python.org/) - Programming language

---

**Happy Learning! 🚀**

*Built with ❤️ for students everywhere*
