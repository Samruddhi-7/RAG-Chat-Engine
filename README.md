# 🤖 RAG Chat Engine

An intelligent chat engine powered by Retrieval-Augmented Generation (RAG) that enables natural conversations with your documents. Built with Python, it combines LLM technology with vector search to provide accurate, context-aware responses from your knowledge base.

## ✨ Features

- **Smart Document Retrieval** - Semantic search using vector embeddings
- **Context-Aware Responses** - Accurate answers grounded in your documents
- **Multi-Format Support** - Process PDFs, text files, and more
- **Conversation Memory** - Maintains chat history for coherent dialogues
- **Flexible Configuration** - Customizable LLM and embedding models

## 🚀 Quick Start

### Installation

```bash
# Clone the repository
git clone https://github.com/Samruddhi-7/RAG-Chat-Engine.git
cd RAG-Chat-Engine

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Configuration

Create a `.env` file in the root directory:

```env
OPENAI_API_KEY=your_api_key_here
EMBEDDING_MODEL=text-embedding-ada-002
LLM_MODEL=gpt-3.5-turbo
CHUNK_SIZE=1000
TOP_K_RESULTS=5
```

### Usage

```bash
cd src
python main.py
```

## 📁 Project Structure

```
RAG-Chat-Engine/
├── src/
│   ├── main.py              # Main application
│   ├── chat_engine.py       # Core chat logic
│   ├── document_loader.py   # Document processing
│   ├── embeddings.py        # Embedding utilities
│   └── vector_store.py      # Vector database ops
├── data/
│   └── documents/           # Your documents here
├── .env                     # Environment variables
└── requirements.txt         # Dependencies
```

## 💡 Basic Usage

```python
from src.chat_engine import RAGChatEngine

# Initialize and load documents
chat_engine = RAGChatEngine()
chat_engine.load_documents("data/documents/")

# Chat with your documents
response = chat_engine.chat("What is this document about?")
print(response)
```

## 🛠️ Tech Stack

- **Python 3.8+**
- **LangChain / LlamaIndex** - RAG framework
- **OpenAI API** - LLM and embeddings
- **ChromaDB / FAISS** - Vector database
- **PyPDF2** - Document processing

## ⚙️ Configuration Options

| Variable | Description | Default |
|----------|-------------|---------|
| `LLM_MODEL` | Language model to use | `gpt-3.5-turbo` |
| `EMBEDDING_MODEL` | Embedding model | `text-embedding-ada-002` |
| `CHUNK_SIZE` | Document chunk size | `1000` |
| `TOP_K_RESULTS` | Retrieved contexts | `5` |
| `TEMPERATURE` | Response creativity | `0.7` |

## 🎯 Use Cases

- Document Q&A systems
- Enterprise knowledge bases
- Research paper analysis
- Customer support automation
- Educational assistants

## 🤝 Contributing

Contributions welcome! Fork the repo, create a feature branch, and submit a pull request.

## 📄 License

MIT License - see [LICENSE](LICENSE) file for details.

## 👤 Author

**Samruddhi** - [@Samruddhi-7](https://github.com/Samruddhi-7)

---

⭐ Star this repo if you find it helpful!
