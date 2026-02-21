# Privacy Policy
**KWS AI Dual Thinking Resoning Hyper Engine v9.0**

**Effective Date:** 21st February 2026

**KWS (Kavinda Web Service)** ("we", "our", or "us") respects your privacy and is committed to protecting your personal data. This Privacy Policy details how **KWS AI Dual Thinking Resoning Hyper Engine v9.0** ("the Software") handles data on your device.

## 1. LOCAL DATA PROCESSING & STORAGE
The Software operates with a strong emphasis on user privacy. Core AI processing and memory storage function predominantly offline:
- **Chat History & User Data:** All conversations, inputs, file uploads, and specific user settings are stored locally on your device's hard drive inside the `%APPDATA%/KWS_AI_v9.0_Data` directory.
- **AI Processing:** The AI model processes text internally on your machine. We do not transmit your local chat context or files uploaded for "Deep Thinking" or internal analysis to KWS remote servers.
- **RAG Memory:** Files, documents, and instructions provided to the AI to "learn" are stored in a local SQLite database and Vector Store. This data remains on your physical machine.

## 2. EXTERNAL COMMUNICATIONS (INTERNET FEATURES)
While the core intelligence is localized, the Software includes specific features that require internet access. By using these features, certain data may be sent to third-party services:
- **Web Search Module:** If you ask the AI to search the internet, your specific search query is sent to external search providers (e.g., Google, DuckDuckGo, Wikipedia) to retrieve live results. 
- **Voice Capabilities:** Text-to-Speech (TTS) and Speech-to-Text (STT) modules utilize third-party APIs (like Google Speech Recognition). Audio clips of your voice commands may be securely transmitted to process speech-to-text.
- **Media Scraping:** Downloading or analyzing YouTube videos or images interacts with external servers (like YouTube via `yt-dlp`).

**We do NOT intercept, store, or monitor any of these external requests.** The requests are made directly from your computer to the third-party provider. 

## 3. ANALYTICS AND TELEMETRY
We do not build telemetry, tracking software, or hidden analytics into the offline executables of the Software. Your usage of the application is your own.

## 4. DATA RETENTION & DELETION
Because your data is stored on your device, you have complete control over its retention. You can permanently delete all chat logs, vector memory, and uploaded files by:
1. Navigating to `%APPDATA%/KWS_AI_v9.0_Data` in your Windows file explorer.
2. Deleting the contents of that directory.

## 5. THIRD-PARTY LINKS & INTEGRATIONS
Our application may present links or information from the web. We are not responsible for the privacy practices or content of third-party websites retrieved by the search engine.

## 6. CHANGES TO THIS PRIVACY POLICY
We may update our Privacy Policy from time to time. We will notify you of any changes by posting the new Privacy Policy on our official web pages or accompanying documentation in future software updates.

## 7. CONTACT US
If you have any questions about this Privacy Policy, please contact us:
- **Developer:** Hanwellage Kavinda Dilshan
- **Email:** info@kavindawebservice.site
- **Phone:** +94765388360
- **Website:** [kavindawebservice.site](https://kavindawebservice.site)
