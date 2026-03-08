# Streamlit PDF Chatbot 🤖

An AI-powered chatbot built with Streamlit that allows users to upload PDF documents and have interactive conversations about their content using OpenAI and LangChain.

## Features

- **PDF Upload & Processing** — Upload single or multiple PDF files for analysis
- **Conversational Q&A** — Ask questions about your documents in natural language
- **Vector Search** — Uses FAISS for efficient semantic similarity search
- **Conversation Memory** — Maintains chat context across multiple questions
- **Animated UI States** — Visual feedback with animated states (reading, thinking, welcoming)

## Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)

- **LLM:** OpenAI GPT-3.5 Turbo
- **Embeddings:** OpenAI Embeddings
- **Vector Store:** FAISS
- **Text Processing:** LangChain CharacterTextSplitter
- **PDF Parsing:** PyPDF2
- **Framework:** Streamlit

## How It Works

```
PDF Upload → Text Extraction → Chunking → Embeddings → FAISS Vector Store
                                                            ↓
User Question → Semantic Search → Relevant Chunks → LLM → Answer
```

## Setup

1. Clone the repository
```bash
git clone https://github.com/nofaukost/Streamlit-Chatbot.git
cd Streamlit-Chatbot
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Set up environment variables
```bash
echo "OPENAI_API_KEY=your_api_key_here" > .env
```

4. Run the app
```bash
streamlit run app.py
```

## Project Structure

```
├── app.py              # Main Streamlit application
├── htmlTemplates.py    # HTML/CSS templates for chat UI
├── requirements.txt    # Python dependencies
├── *.gif               # Animated UI state indicators
└── .env                # Environment variables (not tracked)
```

## License

MIT
