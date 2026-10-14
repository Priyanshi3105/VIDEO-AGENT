🎥 Video Agent
An AI-powered video intelligence system that downloads YouTube videos, transcribes audio, generates summaries, extracts insights, and enables question-answering through Retrieval-Augmented Generation (RAG).

🚀 Features
Download audio from YouTube videos
English transcription using Whisper
Hindi/Hinglish transcription using Sarvam AI
AI-generated summaries
Action item extraction
Key decision extraction
Semantic search using vector embeddings
RAG-based question answering
Support for long-form video content
📂 Project Structure
VIDEO AGENT/
│
├── .venv/
│
├── core/
│   ├── __init__.py
│   ├── extractor.py
│   ├── rag_engine.py
│   ├── summarizer.py
│   ├── transcriber.py
│   └── vector_store.py
│
├── downloads/
│
├── Screenshots/
│
├── utils/
│
├── vector_db/
│
├── .env
├── .gitignore
├── README.md
├── requirements.txt
└── test.py
🏗️ Workflow
YouTube URL
    │
    ▼
Audio Download
    │
    ▼
Speech-to-Text
    │
    ▼
Transcript Processing
    │
    ▼
Chunking
    │
    ▼
Embeddings
    │
    ▼
Vector Database
    │
    ▼
Summary Generation
    │
    ▼
RAG Question Answering
🛠️ Technologies Used
AI & LLMs
OpenAI
Ollama
LangChain
Speech Processing
Whisper
Sarvam AI
Vector Database
ChromaDB
Embeddings
HuggingFace Embeddings
Language
Python
⚙️ Setup Instructions
Clone Repository
git clone https://github.com/YOUR_USERNAME/video-agent.git

cd video-agent
Create Virtual Environment
python -m venv .venv
Activate Environment
Windows:

.venv\Scripts\activate
Install Dependencies
pip install -r requirements.txt
🔑 Environment Variables
Create a .env file in the project root:

OPENAI_API_KEY=your_openai_key
SARVAM_API_KEY=your_sarvam_key
▶️ Running the Application
python test.py
or whichever file is your entry point.

🧠 RAG Capabilities
The application:

Generates transcripts.
Splits text into semantic chunks.
Creates embeddings.
Stores embeddings in ChromaDB.
Retrieves relevant context.
Answers questions grounded in video content.
Example:

Question:
What are the benefits of RAG?

Answer:
RAG improves factual accuracy by retrieving
relevant information before generating a response.
📸 Screenshots
Add your screenshots inside the Screenshots folder and display them like:

Application Workflow
![Workflows/workflow.png

Summary Output
Screenshots/summary.png

RAG Q&A
![RAG](Screenshots/rag_
🎯 Use Cases
Lecture Notes Generation
Meeting Summaries
Podcast Analysis
Knowledge Retrieval
Training Video Search
Action Item Tracking
🔒 Security
The following are excluded from Git:

.env
.venv/
downloads/
vector_db/
__pycache__/
🚀 Future Improvements
Streamlit/Web UI
Speaker Diarization
PDF Export
Multi-Language Summaries
Real-Time Processing
Batch Video Processing
👩‍💻 Author
Priyanshi Gupta

Engineering Intern

Built using Python, LangChain, ChromaDB, Whisper, Sarvam AI, OpenAI, and Ollama.