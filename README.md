# 🎙️ Audio Notes Transcriber — Voice & Text RAG Chatbot

Upload or record audio, get instant speech-to-text transcription powered by Gemini's native audio understanding, then chat with your documents and voice notes using a RAG pipeline.

## What it does

- **🎤 Record voice** right in the browser (via a mic widget) — speech is transcribed with **Gemini 2.5 Flash's native multi-modal audio input**, no external speech-to-text service needed
- **📄 Upload PDFs / 🌐 crawl a website** to build a searchable knowledge base (ChromaDB + Gemini embeddings)
- **💬 Chat** with your knowledge base — answers are streamed live with sources cited
- **💾 Auto-saves** chats locally and caches answers for instant repeat lookups

## Tech stack

- Python, Streamlit
- Google Gemini 2.5 Flash (`google-genai` SDK) — native audio transcription + chat
- LangChain (text splitting, loaders) · LangChain-Google-GenAI (embeddings)
- ChromaDB vector store
- `streamlit-mic-recorder` for in-browser voice capture

## Run it

```bash
pip install -r requirements.txt

# Set your Gemini API key (get one free at https://aistudio.google.com/apikey)
export GOOGLE_API_KEY="your-key-here"

streamlit run app.py
```

## Credit

This project is an **extension of the open-source project [`voice_rag`](https://github.com/adnnaan/voice_rag) by [@adnnaan](https://github.com/adnnaan)**. The original repository ships with no license file.

Maintained/extended by **Muhammad Huzaifa Aqeel** ([@HuzaifaAqeel](https://github.com/HuzaifaAqeel)).
