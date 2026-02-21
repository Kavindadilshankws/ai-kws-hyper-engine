# Troubleshooting Guide & FAQ
**KWS AI Dual Thinking Resoning Hyper Engine v9.0**

## Frequently Asked Questions

**Q: Do I need an internet connection to use KWS AI?**
**A:** No, the core generation, "Deep Thinking," and data analysis off local documents work entirely offline. However, features like "Web Search", live news scraping, and Voice input (STT) require an active internet connection.

**Q: Where is my data stored?**
**A:** All chats and AI memories are stored on your local hard drive at `%APPDATA%/KWS_AI_v9.0_Data`. No text data is sent to KWS servers.

**Q: Can I share the software with others?**
**A:** Please refer to the End-User License Agreement (EULA). Generally, distribution of the proprietary executable without KWS permission is prohibited.

---

## Common Errors & Solutions

### 1. "Failed to start: kws_core.bin not found"
**Issue:** The application launches but immediately errors out stating it cannot find the AI model file.
**Solution:** The core AI brain file is missing from the compiled package or the `assets/models/` directory. Ensure that `kws_core.bin` is placed correctly before building, or if you downloaded the application, ensure your antivirus didn't accidentally quarantine the file. Re-install or extract the application zip again.

### 2. High Memory/RAM Usage
**Issue:** Windows task manager shows the app consuming 4GB to 8GB of RAM.
**Solution:** This is normal. The local AI engine (`kws_core`) loads directly into your system RAM to process responses quickly. If your PC slows down considerably, ensure you are not running heavy background applications simultaneously or close unused tabs in your browser.

### 3. Web Search is Unresponsive or "Timed Out"
**Issue:** Asking the AI to search the web results in long load times or a timeout error.
**Solution:** 
- Check your internet connection. 
- You may have hit a rate limit with Google or DuckDuckGo if you have made too many search requests rapidly. Wait 5-10 minutes and try again.
- Sometimes search providers change their page structures; if it remains broken for days, await an update patch from KWS.

### 4. Application Window Does Not Open
**Issue:** You double-click the `.exe` file, a process starts in task manager, but no interface appears.
**Solution:** KWS AI uses a local Flask server running on port 5000. 
1. Check if another application (like another web server or Spotify background service) is using port 5000. 
2. Verify you have Google Chrome or Microsoft Edge installed on your PC, as Eel relies on these engines to render the UI.
3. Open a browser and manually type `http://127.0.0.1:5000/`.

### 5. Chat DB or VectorStore Corrupted
**Issue:** Past sessions aren't loading, or throwing SQLite database lock errors.
**Solution:** 
1. Close the application completely.
2. Press `Win + R`, type `%APPDATA%`, and hit Enter.
3. Locate `KWS_AI_v9.0_Data`. 
4. You can backup and then delete `chat_history.db` and the `memory_db` folder to completely reset the application.

### 6. Voice Recognition Not Working
**Issue:** The microphone icon clicks but speech is not converted to text.
**Solution:** Ensure your default microphone is properly configured in Windows Settings. Navigate to Windows Settings > Privacy & security > Microphone, and assure desktop applications are allowed to access your microphone.

## Further Support
If these steps do not resolve your issue, please contact us:
- **Email:** info@kavindawebservice.site
- **Phone:** +94765388360
