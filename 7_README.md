# KWS AI Dual Thinking Resoning Hyper Engine v9.0

**Developer:** Hanwellage Kavinda Dilshan  
**Company:** KWS (Kavinda Web Service)  
**Website:** [kavindawebservice.site](https://kavindawebservice.site)  
**Support Email:** info@kavindawebservice.site  

---

## Overview
**KWS AI Vish v9.0** is an advanced, offline-first artificial intelligence assistant that brings state-of-the-art computational reasoning directly to your Windows desktop. Designed for maximum privacy, the core cognitive engine runs locally, meaning your data, chat logs, and uploaded files never leave your computer unless you explicitly demand web-integrated functions.

Boasting the bespoke **Hyper Dual Think Engine**, the application seamlessly alternates between rapid conversational generation and deep logic traversal for complex queries.

## Key Features
- **Hyper Dual Think Engine:** Instruct the AI to "think deeply" on mathematical equations, coding architectural decisions, or logical puzzles. The AI parses the thought process before finalizing an answer.
- **Privacy-First Offline Core:** Loaded entirely in RAM, the proprietary `kws_core.bin` model executes offline. Information is stored in `%APPDATA%/KWS_AI_v9.0_Data`.
- **RAG Memory Integration:** Upload PDF documents, text files, or images. The Vector Store reads and memorizes the files, allowing the AI to recall them contextually in future conversations.
- **Robust Web Module:** Integrated with a Specialized Search Engine, the AI can query Google/DuckDuckGo for live facts, scrape Wikipedia, and embed YouTube videos directly into the chat interface.
- **Internet Learner background Process:** Opt-in to background automated scraping. The AI will autonomously learn and expand its knowledge base while sitting idle.
- **Voice Interactions:** Includes fluid Text-to-Speech (TTS) reading capabilities and Speech-to-Text (STT) mic interactions.

## Installation Instructions

### Pre-Compiled Executable (Recommended)
1. Download the `KWS_AI_v9.0.exe` file.
2. Double-click to run. No setup wizard is necessary.
3. Please allow 15-30 seconds for the AI model to allocate into your RAM on startup. The UI window will automatically open once initialised.

### Running from Source / Developers
Ensure you have Python 3.10+ installed.
1. Clone the repository / download the source bundle.
2. Install dependencies: `pip install -r requirements.txt`
3. Make sure the model `kws_core.bin` is placed in `assets/models/`.
4. Run the main server script: `python app.py`

## Architecture & Tech Stack
- **Backend:** Python, Flask, Flask-Cors
- **AI Core Interfacing:** `llama-cpp` / proprietary wrappers (GGUF structures).
- **GUI Engine:** `eel` (HTML/CSS/JS communicating seamlessly with Python backends)
- **Database:** SQLite (Chat Logs), Local VectorDB for embeddings.
- **Search Integrations:** `googlesearch-python`, `duckduckgo-search`, `yt-dlp`.

## Contact & Licensing
Proprietary Software by KWS. Please read the `EULA.md` and `Terms_of_Service.md` before commercial deployment. For inquiries, reach out to **+94765388360** or **info@kavindawebservice.site**.
