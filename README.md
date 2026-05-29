# ST10482038_PROG_Part-2
# AEGIS — Cyber Sentinel (Chatbot GUI)

AEGIS is a WPF chatbot application focused on cybersecurity awareness. It demonstrates keyword recognition, random replies, basic sentiment detection, conversational context/memory, and a polished GUI.

Features
- Keyword recognition with multiple randomized responses
- Conversation memory and follow-up handling
- Basic sentiment detection that adjusts tone
- Session persistence (saves user name and preferences)
- Text-to-speech greeting and spoken replies (Windows SAPI)
- Polished WPF GUI with topics sidebar, quick tips, typing indicator, and animations

Quick start
1. Open the solution in Visual Studio 2022/2025/2026 and restore (no external NuGet required).
2. Build the solution (targeting .NET 10).
3. Run the application.

Usage
- On first run you'll be prompted for your name. The bot will greet you by name.
- Type a topic number (1–25) to view a summary on that topic.
- Type `menu` to list topics.
- Type `exit` to quit the app.
- Try keywords such as `password`, `phish`, `email`, `backup`, `malware`, `vpn`, `2fa` to see targeted responses.

Session persistence
- The app saves a small session JSON in %AppData%\AEGIS to remember your name and basic preferences across runs.

Extending or testing
- Chatbot logic is in Ageis/Chatbot.cs. Add keywords or expand responses in the _responseVariants dictionary.
- AudioPlayer (Ageis/AudioPlayer.cs) uses Windows SAPI.SpVoice for TTS. If SAPI is unavailable, audio is silently disabled.

Repository and releases
- Ensure you commit changes with descriptive messages. Create at least 3 tagged releases (v1.0, v1.1, v1.2) with release notes for grading.

Deliverables checklist
- README (this file)
- CHANGELOG.md (release notes)
- At least 6 descriptive commits
- Minimum 3 tagged releases (include links in README)
- YouTube demo link (place in README under "Presentation")

Presentation
- Record a short demo (5–10 minutes) showing: keyword recognition, follow-up handling, sentiment adaptation, memory recall, TTS greeting, and UI features. Add the YouTube link below.

Presentation link: <ADD_YOUR_YOUTUBE_LINK_HERE>

License
- MIT (add your own license file if required)
