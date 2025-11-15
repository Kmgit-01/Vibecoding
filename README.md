# Vibecoding Assistant

## Overview

**Vibecoding Assistant** is a cross-platform intelligent voice-controlled assistant built for both web and desktop (Electron) environments. It combines voice recognition, AI-powered natural language understanding, speech synthesis, customizable settings, and advanced features such as application control and external API integrations (like joke generation).

---

## ✨ Key Features

- **Voice Control:**  
  - Start/Stop listening with a microphone button
  - Real-time speech-to-text transcription
  - Continuous listening mode option

- **Intelligent AI Understanding:**  
  - Natural language request handling (powered by Claude API)
  - Context-aware conversations, multi-turn dialogs
  - Handles complex questions and requests

- **Speech Synthesis:**  
  - Assistant speaks responses back using customizable voices
  - Adjustable voice speed and pitch

- **Customizable Settings Panel:**  
  - Multiple language support (English, Spanish, French, German, Hindi, Chinese, etc.)
  - Choice of different voices
  - Mute/unmute audio
  - Clear conversation history

- **App & System Control (Desktop):**  
  - Launch applications by voice (e.g., "Open Spotify", "Open Calculator", "Start VS Code")
  - Open files/folders
  - Basic system actions ("Mute volume", "Take screenshot", "Lock computer")
  - Security gating for sensitive actions

- **Browser Control (Web):**  
  - Open websites in new tabs ("Open GitHub")
  - Close active tab (where permitted by browser)

- **Conversation Management:**  
  - Full scrollable chat history with timestamps
  - Clear/copy history option

- **Random Joke Generator:**  
  - Ask for a joke and get one in real-time via JokeAPI

---

## 🌐 Platform Support

- **Web:** Chrome, Edge (best support for Web Speech, Text-to-Speech APIs)
- **Desktop:** Electron-powered (supports all web features plus native OS actions)

---

## 🔧 Getting Started

### Web

1. **Clone this repository**
2. **Open `public/index.html` in a supported browser**
3. **Grant microphone permission** when prompted

### Desktop (Electron)

1. **Install dependencies:**  
   `npm install`
2. **Start the app:**  
   `npm start`
3. **Grant microphone permission on first use**

---

## 🛡️ Privacy Note

- **Web:** All voice processing is done in your browser. Only transcribed text is sent to the AI API.
- **Desktop:** App/system actions require explicit opt-in via the settings panel. Sensitive actions (like locking or launching apps) may ask for confirmation.

---

## 🧩 Extending

- **Add new application controls:** See `src/desktop/ElectronAppControl.js`
- **Add new AI skills/commands:** Extend `src/common/IntentParser.js`
- **Add new conversation features or plugins:** UI and backend are modular and extensible.

---

## 🙋 Example Commands

- "Tell me a joke"
- "Open the calculator"
- "Mute volume"
- "What's the weather?"
- "Explain quantum physics simply"
- "Show my Downloads folder"
- "Open GitHub in a new tab"
- "Clear history"

---

## ✍️ Contributing

See the `CONTRIBUTING.md` for guidelines.  
Bug reports, suggestions, and pull requests are welcome!

---

## 📜 License

MIT License. See `LICENSE` for details.
