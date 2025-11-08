# 🤖 AI Chat + OCR Assistant

A powerful and versatile application that combines intelligent chat capabilities with advanced document processing. Built with Ollama, FastAPI, and Streamlit, this platform enables seamless conversations while extracting and analyzing text from various document formats.

## ✨ Features

- 💬 **Smart Chat Interface**
  - Real-time AI conversations
  - Persistent chat history
  - Dynamic session management
  - Automatic chat naming

- 📑 **Document Processing**
  - Images (JPG, PNG)
  - PDF documents
  - Word files (.docx)
  - AI-powered text summarization

- 🛠️ **Technical Stack**
  - Frontend: Streamlit
  - Backend: FastAPI
  - AI: Ollama
  - OCR: EasyOCR + Tesseract
  - Real-time processing

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- Tesseract-OCR (Windows users)
- Ollama

### Setup Steps

1. **Install Requirements**
   ```bash
   pip install -r requirements.txt
   ```

2. **Start Ollama**
   ```bash
   ollama serve
   ollama pull llama3
   ```

3. **Launch Backend**
   ```bash
   uvicorn backend:app --reload
   ```

4. **Start Frontend**
   ```bash
   streamlit run app.py
   ```

Visit `http://localhost:8501` to access the application.

## 💡 Key Features

- **Smart Document Processing**: Extract text from images, PDFs, and Word documents
- **Dual OCR Engine**: Combines EasyOCR and Tesseract for improved accuracy
- **AI-Powered Summaries**: Automatic summarization of extracted content
- **Interactive Chat**: Natural conversations with AI
- **Session Management**: Organize and maintain multiple chat sessions
- **Real-time Processing**: Instant feedback and responses

## 🔧 Configuration

### Environment Variables
- `OLLAMA_URL`: Ollama API endpoint (default: http://localhost:11434/api/generate)
- `MODEL_NAME`: AI model selection (default: llama3)

### Windows-specific Setup
For Windows users, ensure Tesseract-OCR is installed and configured:
```python
pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"
```

## 📖 Usage

1. Start a new chat session
2. Upload documents for analysis (supported formats: JPG, PNG, PDF, DOCX)
3. Receive AI-generated summaries
4. Continue conversation with context-aware responses

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report issues
- Submit pull requests
- Suggest improvements
- Share feedback

## 📄 License

This project is licensed under the MIT License.

---

Built with ❤️ using Ollama, FastAPI, and Streamlit
