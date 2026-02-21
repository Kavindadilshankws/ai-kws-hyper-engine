# Release Notes: KWS AI v9.0
**Product:** KWS AI Dual Thinking Resoning Hyper Engine  
**Version:** 9.0  
**Release Date:** 21st February 2026  
**Developer:** Hanwellage Kavinda Dilshan (KWS)  

---

##  What's New in Version 9.0

We are thrilled to announce the official release of KWS AI v9.0, branded the **Hyper Dual Think Engine**. This version is a massive leap forward from v8.0, entirely reforming how the AI handles complex logic, memory allocation, and UI/UX synchronization. 

### 1. The Hyper Dual Think Engine
- **Dedicated Deep Thinking Pipeline:** The core model logic has been refactored (`brain.dual_thinking.py`) to permit explicit "thought streams". For highly complex queries, the AI will evaluate intermediate logic steps, displaying them seamlessly on the UI, before emitting the conclusive answer.
- **Threaded Architecture (Anti-Freeze):** Rebuilt the Flask backend utilizing `threading` and Server-Sent Events (SSE). The user interface will no longer freeze during heavy local processing.

### 2. Upgraded Memory Systems (RAG)
- **Persistent Vector Store:** Memories, uploaded files, and parsed data are now structurally stored in an optimized local Vector Database targeting `%APPDATA%/KWS_AI_v9.0_Data`.
- **Identity Recall Boost:** Drastically improved the prompt-context builder to actively prioritize personal facts. The model is now hard-coded to intercept queries like "What is my name?" and override general processing with stored RAG attributes.

### 3. Comprehensive Internet & Media Upgrades
- **Specialized Web Search Engine:** Replaced the unreliable basic DuckDuckGo hooks. v9.0 now employs a multi-tiered query pipeline utilizing Google, DDG, and Wikipedia.
- **Media First Display:** Search results that contain images or videos are now injected as graphical cards at the top of the chat output, followed by AI explanation and text sources. Support for inline YouTube thumbnail display added via `yt-dlp`.

### 4. Enterprise-Grade Build and UI
- **Portable Executable Architecture:** Finalized the `KWS_AI_v9.0.spec` configuration. The entire AI application—comprising the logic, GUI, and local Python dependencies—are packed into a pristine `.exe` ready for cross-device USB distribution.
- **Local Sandbox Confinement:** Added `clean_data.py` logic. The executable prevents bundling local developer test data into the final distribution, dynamically recreating necessary folders for end-users securely.
- **User Interface Flourishes:** Improved the thinking animation timelines, enhanced the chat bubble formatting (WhatsApp-style aesthetics), and stabilized the background loop (`assets/back.gif`).

##  Bug Fixes
- Fixed an issue in v8.0 where the search engine would return YouTube URLs entirely irrespective of image search parameters.
- Fixed the chat overlay/startup overlap bug that populated duplicated historical messages upon Eel window refresh.
- Patched the Llama-CPP native library failure (`WinError 3`) that occurred when traversing different Windows 11 host machines, securing dependency mapping.
- Handled the UI lock-on "thinking..." state even if the model generation crashed or threw an exception.

##  Known Issues
- Very large PDF files (over 50 pages) uploaded via the paperclip icon might cause a brief application stutter as the `fitz` PyMuPDF parser embeds tokens.
- Audio Text-to-Speech (TTS) on initial launch may have a 2-second delay while the `pyttsx3` engine warms up in the background thread.

---
*For support or documentation, visit [ai.kavindawebservice.site](https://ai.kavindawebservice.site) or review the newly authored manual files accompanying this build.*
