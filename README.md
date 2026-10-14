🎥 Video Agent
An AI-powered Video Intelligence System that transforms YouTube videos into searchable knowledge.

Video Agent automatically downloads video audio, generates transcripts, creates concise summaries, extracts key insights, and enables Retrieval-Augmented Generation (RAG) based question answering over video content.

Built using Python, LangChain, ChromaDB, Whisper, Sarvam AI, and modern LLM workflows.

🌟 Key Features
📥 Video Processing
Download audio from YouTube videos
Support for long-form content such as podcasts, webinars, lectures, and interviews
Automatic audio extraction and preprocessing
🎙️ Speech-to-Text
English transcription using Whisper
Hindi/Hinglish transcription using Sarvam AI
Language-aware transcription pipeline
📝 AI Summarization
Generate concise summaries
Long-video summarization support
Structured output generation
🔍 Information Extraction
Extract:

Key Insights
Important Takeaways
Action Items
Decisions & Recommendations
🧠 Retrieval Augmented Generation (RAG)
Intelligent document chunking
Embedding generation
ChromaDB vector storage
Context retrieval
Natural language question answering
💬 Conversational Querying
Ask questions directly about the video content:

Q: What are the benefits of RAG?

A: RAG improves factual accuracy by retrieving
relevant context from external knowledge sources
before generating a response.
🏗️ System Architecture
YouTube Video
      │
      ▼
Audio Download
      │
      ▼
Transcription
      │
      ▼
Text Processing
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
RAG-Based Q&A
📂 Project Structure
VIDEO AGENT/
│
├── core/
│   ├── __init__.py
│   ├── extractor.py
│   ├── rag_engine.py
│   ├── summarizer.py
│   ├── transcriber.py
│   └── vector_store.py
│
├── utils/
│   ├── __init__.py
│   ├── app.py
│   ├── audio_processor.py
│   └── main.py
│
├── Screenshots/
│
├── vector_db/
│
├── downloades/
│
├── test.py
├── README.md
├── Requirements.txt
├── .gitignore
└── .env
⚙️ Tech Stack
Programming Language
Python
AI & LLM Frameworks
OpenAI
Ollama
LangChain
Speech Processing
OpenAI Whisper
Sarvam AI Speech-to-Text
Vector Database
ChromaDB
Embeddings
HuggingFace Embeddings
🚀 Installation
Clone Repository
git clone https://github.com/YOUR_USERNAME/VIDEO-AGENT.git
cd VIDEO-AGENT
Create Virtual Environment
python -m venv .venv
Activate Environment
Windows
.venv\Scripts\activate
Linux/Mac
source .venv/bin/activate
Install Dependencies
pip install -r Requirements.txt
🔑 Environment Variables
Create a .env file in the root directory.

OPENAI_API_KEY=your_openai_key
SARVAM_API_KEY=your_sarvam_key
▶️ Usage
Update the source video URL:

source = "https://www.youtube.com/watch?v=VIDEO_ID"
language = "hinglish"
Run:

python test.py
or

python utils/main.py
depending on your workflow.

📸 Screenshots
Application Workflow
![Workflow](Screenshots/Screenshot%202026-10-13%201# Video Processing

![Processing](Screenshots/Screenshot%202026-10-13

Summary Generation
![Summary](Screenshots/Screenshot%202026-10-.png

RAG Question Answering
RAG

��� Use Cases

Education
Lecture Summaries
Study Notes Generation
Revision Material Creation
Business
Meeting Summaries
Action Item Tracking
Knowledge Management
Content Analysis
Podcast Summarization
Webinar Insights
Interview Analysis
Enterprise Search
Internal Knowledge Base
Semantic Search
AI Assistants
🔒 Security
Excluded from version control:

.env
.venv/
vector_db/
downloades/
__pycache__/
This prevents:

API key exposure
Large file uploads
Generated vector database storage
Temporary processing files
📈 Future Enhancements
Streamlit Web Interface
Multi-Video Processing
Speaker Diarization
PDF Report Generation
Real-Time Transcription
Multi-Language Support
Azure OpenAI Integration
Advanced Analytics Dashboard
👩‍💻 Author
Priyanshi Gupta
Engineering Intern

Built with:

Python
LangChain
ChromaDB
Whisper
Sarvam AI
OpenAI
Ollama
