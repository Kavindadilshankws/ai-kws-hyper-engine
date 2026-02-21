# System Requirements
**KWS AI Dual Thinking Resoning Hyper Engine v9.0**

To ensure smooth operation, stable response times, and uninterrupted functionality for the KWS AI v9.0 client, your machine should meet or exceed the following specifications.

## Minimum System Requirements
- **Operating System:** Windows 10 (64-bit) or Windows 11
- **Processor (CPU):** Intel Core i5 (6th Gen) / AMD Ryzen 3 or equivalent (4 cores minimum)
- **Memory (RAM):** 8 GB RAM (Crucial for handling the Local LLM in memory)
- **Storage:** 4 GB of available disk space (SSD highly recommended for fast model loading)
- **Internet Connection:** Required only for Web Search, Voice Recognition (STT), and Internet Learner features.

## Recommended System Requirements
*For the best experience utilizing Deep Thinking and high-speed RAG inference:*
- **Operating System:** Windows 10/11 (64-bit, latest updates)
- **Processor (CPU):** Intel Core i7 / AMD Ryzen 5 or higher (8+ cores)
- **Memory (RAM):** 16 GB RAM or higher
- **Graphics (GPU):** While primarily CPU-bound in default offline modes, modern NVIDIA/AMD GPUs will greatly accelerate rendering if GPU layers are enabled.
- **Storage:** NVMe M.2 SSD with at least 10 GB of free space for caching and expansive Vector DB memories.
- **Internet:** High-speed broadband connection for instantaneous web results and rapid multimedia scraping.

## Software Dependencies (If running from Source Code)
If you are strictly running the pre-packaged `KWS_AI_v9.0.exe`, no external software is required. The build is entirely portable. 

If executing from raw Python source, you will need:
- **Python:** v3.10.x to v3.11.x (Add Python to PATH)
- **Compiler Tools:** Visual Studio C++ Build Tools (Required for compiling local C bindings).
- **Core Library Packages:**
  - `Flask==3.0.0`
  - `requests==2.31.0`
  - `beautifulsoup4`, `duckduckgo-search`, `googlesearch-python`
  - `SpeechRecognition`, `pyttsx3`
  - `Eel` (for GUI rendering)

## Supported Browsers (For Internal UI Rendering)
The application relies on `Eel` which utilizes Chromium architecture to display the User Interface. 
- Google Chrome (Latest Version)
- Microsoft Edge (Latest Version)
