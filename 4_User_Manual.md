# User Manual & Quick Start Guide
**KWS AI Dual Thinking Resoning Hyper Engine v9.0**

## Introduction
Welcome to KWS AI v9.0! This advanced artificial intelligence assistant features a Hyper Dual Think Engine with live internet searching capabilities, long-term memory (RAG), and a sleek internal user interface. All core thought processing happens right on your device for absolute privacy.

## 1. Installation & Setup
1. **Download the Release Build:** Locate the provided `KWS_AI_v9.0.exe` executable file or standard release folder.
2. **Execute:** Double click the `KWS_AI_v9.0.exe` to launch the application. 
3. **Initialization:** The AI engine will boot up in the background. A progress screen will load, importing the AI core model. Depending on your system hardware, this initial load might take anywhere from 10 to 45 seconds.
4. **Interface:** Once loaded, the application will automatically open a local web-view window utilizing eel/chrome rendering.

*Note: No complex Python installations are required if you are using the compiled `.exe` build.*

## 2. Interface Overview
- **Sidebar (Left):** View your past sessions and chats. Hover over a session to Pin or Lock it (with a password).
- **Chat Area (Center):** The main display for the AI's responses, web search results, media cards, and your messages.
- **Input Bar (Bottom):** Type your prompts here. Includes buttons for File Uploads (Paperclip icon) and Voice Input (Mic icon).
- **Performance Monitor (Top Right):** View your CPU and RAM usage in real-time.

## 3. Core Features & Usage

### 3.1 Standard Chat & Prompts
Simply type your question or request into the input bar and press Enter. The AI will stream its answer to you in real-time.

### 3.2 Deep Thinking Mode
If you need complex logic, mathematical reasoning, or profound problem resolution, ask the bot to think deeply. The Hyper Dual Think Engine will spawn a background "thinking" routine, displaying steps before finalizing the answer.

### 3.3 Active Web Search
Ask the AI for live information (e.g., "What is the weather today?" or "Show me video tutorials on Python"). The AI will automatically route your request to the Specialized Search Engine, retrieve live Google/DuckDuckGo results, parse them, and present an integrated answer complete with source citations, images, and video thumbnails.

### 3.4 RAG Memory & Document Upload
1. Click the **Paperclip icon** in the input bar.
2. Select a PDF, TXT, source code file, or image.
3. The AI will ingest the file into its "Local File Memory". 
4. You can immediately ask questions about the document. The memory persists locally in your `%APPDATA%`!

### 3.5 Stop Generation
If the AI is generating a long response or taking too long to search, click the **Stop button (Square icon)** next to the input field to halt generation instantly.

### 3.6 Internet Learner Background Agent
Toggle this background agent in the settings or via specific chat commands. When active, it will periodically crawl reliable sources based on your interests and silently encode them into the Vector Database so the AI is smarter the next time you ask related questions.

## 4. Managing Your Data
To clear your chat logs and AI memory entirely:
1. Press `Win + R` and type `%APPDATA%`, press Enter.
2. Locate the folder `KWS_AI_v9.0_Data`.
3. Delete or rename the contents inside `memory_db` and `chat_history.db`.

## 5. Support
For issues or deeper technical questions:
- **Email:** info@kavindawebservice.site
- **Phone:** +94765388360
- **Website:** ai.kavindawebservice.site
