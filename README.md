# 🎥 ClipNotes

> Transform videos into searchable knowledge with AI.

ClipNotes is an AI-powered Video Intelligence Platform that converts YouTube videos and uploaded media into structured knowledge. It automatically transcribes audio, generates concise summaries, extracts key action items, and enables semantic question answering using Retrieval-Augmented Generation (RAG).

---

## ✨ Features

- 🎥 Analyze YouTube videos via URL
- 📁 Upload local MP3/MP4/WAV files
- 🎙️ Automatic speech-to-text transcription using Whisper
- 📝 AI-generated summaries
- ✅ Action item extraction
- 💬 Chat with your videos using RAG
- 🔍 Semantic search across transcripts
- 📄 Export summaries and transcripts
- ⚡ Fast vector search powered by ChromaDB

---

## 🏗️ Architecture

```text
          YouTube URL / MP3 / MP4
                    │
                    ▼
            Audio Processing
                    │
                    ▼
       Whisper Speech Transcription
                    │
                    ▼
        Text Chunking & Embeddings
                    │
                    ▼
              ChromaDB Vector Store
                    │
        ┌───────────┴───────────┐
        ▼                       ▼
 AI Summarization         RAG Question Answering
        │                       │
        └───────────┬───────────┘
                    ▼
           Searchable Knowledge Base
```

---

## 🛠️ Tech Stack

### Backend

- Python
- LangChain
- LangGraph
- FastAPI

### AI & NLP

- OpenAI Whisper
- Mistral AI
- Hugging Face Embeddings

### Vector Database

- ChromaDB

### Processing

- yt-dlp
- FFmpeg
- PyDub

### Frontend

- Streamlit

---

## 📂 Project Structure

```text
ClipNotes/
│
├── app.py
├── requirements.txt
├── .env
│
├── data/
├── downloads/
├── chroma_db/
│
├── utils/
│   ├── audio_processor.py
│   ├── transcriber.py
│   ├── summarizer.py
│   ├── embeddings.py
│   ├── rag.py
│   └── exporter.py
│
├── prompts/
│
└── assets/
```

---

## 🚀 Getting Started

### Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/clipnotes-ai.git

cd clipnotes-ai
```

### Create Virtual Environment

```bash
python -m venv venv
```

### Activate Environment

Windows

```bash
venv\Scripts\activate
```

Linux / macOS

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Configure Environment Variables

Create a `.env` file

```env
MISTRAL_API_KEY=your_api_key
```

### Run the Application

```bash
streamlit run app.py
```

---

## 📖 Workflow

1. Enter a YouTube URL or upload a video/audio file.
2. Audio is extracted and processed.
3. Whisper generates the transcript.
4. Transcript is chunked and embedded.
5. Embeddings are stored in ChromaDB.
6. AI generates:
   - Summary
   - Action Items
   - Key Insights
7. Ask questions using natural language powered by RAG.

---

## 💡 Future Improvements

- Speaker diarization
- Meeting analytics dashboard
- Multi-language support
- Timeline generation
- PDF & DOCX exports
- Team collaboration
- Cloud deployment
- User authentication

---

## 📸 Screenshots

> Screenshots and demo GIFs will be added soon.

---

## 🤝 Contributing

Contributions are welcome!

If you'd like to improve ClipNotes, feel free to fork the repository and submit a pull request.

---

## 📜 License

This project is licensed under the MIT License.

---

## ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub!

---

## 👨‍💻 Author

**Subhayan Mitra**

Final Year Computer Science Engineering Student

GitHub: https://github.com/OfficialSubhayan
