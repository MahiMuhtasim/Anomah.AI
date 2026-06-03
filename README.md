# ✨ Anomah Ai — OpenRouter-Powered AI Assistant

A sleek, modern **Bengali-first AI chat interface** powered by OpenRouter. Anomah Ai is a progressive web app (PWA) that brings intelligent conversations to your device—with offline support, local data privacy, and customizable AI models.

**Live:** [mahimuhtasim.github.io/Anomah.AI](https://mahimuhtasim.github.io/Anomah.AI/)

---

## 🎯 Features

### 🧠 AI & Models
- **Multi-model support** via OpenRouter API
  - OpenAI GPT-4o Mini
  - Anthropic Claude 3.5 Sonnet
  - Meta Llama 3.1 (70B)
  - Google Gemini 1.5 Pro
  - Mistral 7B
  - Custom models via API

- **Customizable system prompts** — tailor AI behavior to your needs
- **Temperature control** (0.0–1.5) — balance creativity vs. precision
- **Streaming responses** — watch AI think in real-time

### 🔒 Privacy & Security
- **100% local data** — all chat history and settings stored in browser only
- **No server tracking** — your conversations never leave your device
- **Per-user accounts** — isolated chat history for each user
- **Password-protected sessions** — simple, local authentication

### 📱 Progressive Web App (PWA)
- **Install as app** — one-click installation to home screen
- **Offline capable** — service worker for offline functionality
- **Works everywhere** — desktop, tablet, mobile
- **Responsive design** — optimized for all screen sizes

### 🎨 Modern UI
- **Dark theme** with accent gradients (teal & cyan)
- **Bengali-first interface** — fully localized labels & hints
- **Smooth animations** — polished micro-interactions
- **Real-time typing indicators** — see when AI is responding
- **Markdown support** — formatted responses with code blocks

### ⚙️ Customization
- **System prompt editor** — write custom AI instructions
- **Model selection** — switch between providers and models
- **API endpoint configuration** — use custom API gateways
- **Export conversations** — save chat as JSON
- **Clear chat history** — privacy-first design

---

## 🚀 Getting Started

### 1. **Get Your OpenRouter API Key**
- Visit [openrouter.ai/keys](https://openrouter.ai/keys)
- Create a free account (includes free credits)
- Copy your API key

### 2. **Open Anomah Ai**
- Go to [mahimuhtasim.github.io/Anomah.AI](https://mahimuhtasim.github.io/Anomah.AI/)
- Create an account or log in

### 3. **Configure Settings**
- Click the **Settings** icon in the sidebar
- Paste your OpenRouter API key
- Choose a model (GPT-4o Mini is recommended for free users)
- Optionally customize the system prompt & temperature

### 4. **Start Chatting!**
- Type your message in the input box
- Press **Enter** to send (Shift+Enter for new lines)
- Watch the AI respond in real-time

---

## 🏗️ Project Structure

```
Anomah.AI/
├── index.html          # Main application (HTML + CSS + JS bundled)
├── manifest.json       # PWA manifest configuration
├── sw.js              # Service worker for offline support
├── icon-192.png       # App icon (192×192)
├── icon-512.png       # App icon (512×512)
├── LICENSE            # Mozilla Public License 2.0
├── SECURITY.md        # Security policy
└── README.md          # This file
```

---

## 🔧 Installation & Development

### Run Locally
```bash
# Clone the repository
git clone https://github.com/MahiMuhtasim/Anomah.AI.git
cd Anomah.AI

# Serve with any local server (requires HTTPS for PWA features)
# Option 1: Python
python3 -m http.server 8000

# Option 2: Node.js (http-server)
npx http-server -p 8000 --cors

# Open https://localhost:8000 in your browser
```

> **Note:** PWA features (service worker, installation) require HTTPS. For local development, use `localhost` or enable insecure contexts in your browser.

### Build & Deploy
- No build step required — this is a single-file PWA
- Deploy to GitHub Pages, Vercel, Netlify, or any static host
- Ensure HTTPS is enabled for PWA features

---

## 🔐 Security & Privacy

### Data Storage
- **Browser LocalStorage** — user credentials and settings stored locally
- **No backend server** — all data stays on your device
- **IndexedDB** — chat history (future expansion)
- **No cookies/tracking** — clean and private by default

### Password Security
- **Client-side hashing** — passwords are hashed before storage (not transmitted)
- **Per-user isolation** — each user's chat is private
- **Logout clears API key** — security-first session management

### API Security
- **Your API key stays in your browser** — never sent to third parties
- **HTTPS-only communication** — encrypted requests to OpenRouter
- **No key logging** — transparent, auditable code

---

## 🎮 User Guide

### Chat Interface
| Action | Keyboard |
|--------|----------|
| Send message | `Enter` |
| New line | `Shift + Enter` |
| Focus input | `Ctrl/Cmd + L` |

### Sidebar Settings
- **Account** — View logged-in user and log out
- **API Connection** — Configure OpenRouter endpoint and key
- **Model Selection** — Choose from 6+ available AI models
- **Customization** — Edit system prompt and temperature
- **Actions** — Clear chat or export as JSON

### PWA Installation
- **Desktop** — Look for "Install" button in address bar
- **Mobile (iOS)** — Tap Share → "Add to Home Screen"
- **Mobile (Android)** — Tap menu → "Install app"

---

## 📊 Supported AI Models

| Model | Provider | Use Case |
|-------|----------|----------|
| GPT-4o Mini | OpenAI | Fast, balanced responses (recommended) |
| Claude 3.5 Sonnet | Anthropic | Long-form writing, reasoning |
| Llama 3.1 (70B) | Meta | Open-source, privacy-friendly |
| Gemini 1.5 Pro | Google | Multi-modal, creative tasks |
| Mistral 7B | MistralAI | Lightweight, efficient |

---

## 🌍 Localization

### Current Languages
- **Bengali (বাংলা)** — Full UI, prompts, and help text
- **English** — In code and technical documentation

### Adding New Languages
Edit the HTML to replace Bengali text with your language:
```html
<!-- Example: Change "লগইন" to your language -->
<button class="auth-tab active" id="tabLogin" onclick="switchAuthTab('login')">Login</button>
```

---

## 🐛 Known Limitations

- **No chat history sync** — history stays on device (by design)
- **No collaborative features** — single-user per account
- **Limited to OpenRouter models** — uses OpenRouter API exclusively
- **Offline responses** — not available (requires API connection)

---

## 🤝 Contributing

Contributions welcome! Please:

1. **Fork** the repository
2. **Create a feature branch** (`git checkout -b feature/amazing-thing`)
3. **Test thoroughly** (especially on mobile)
4. **Submit a pull request** with description of changes

### Areas for Contribution
- [ ] Dark/light theme toggle
- [ ] Additional language support (Hindi, Urdu, etc.)
- [ ] Chat folders or organization
- [ ] Mobile app wrapper (React Native/Flutter)
- [ ] Enhanced markdown editor
- [ ] Voice input/output support

---

## 📜 License

This project is licensed under the **Mozilla Public License 2.0** — see [LICENSE](LICENSE) for details.

**TL;DR:** You can use, modify, and distribute this software freely, but you must include the license and source code when distributing modifications.

---

## 🛡️ Security & Responsible Use

See [SECURITY.md](SECURITY.md) for:
- Vulnerability disclosure guidelines
- Privacy commitment
- Terms of use with OpenRouter API

---

## 💬 Support & Feedback

- **GitHub Issues** — Report bugs or request features
- **Discussions** — Share ideas and ask questions
- **Email** — Contact the author

---

## 📚 Tech Stack

- **Frontend:** Vanilla JavaScript, HTML5, CSS3
- **APIs:** OpenRouter REST API
- **Storage:** Browser LocalStorage + Service Worker
- **PWA:** Manifest.json + Service Worker (`sw.js`)
- **Design:** Custom CSS with CSS Grid/Flexbox

---

## 🎓 Learning Resources

- [OpenRouter API Docs](https://openrouter.ai/docs)
- [MDN Web Docs (PWA)](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps)
- [Service Worker API](https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API)
- [Web Storage API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Storage_API)

---

## 🙏 Acknowledgments

- **OpenRouter** — Unified API for multiple LLMs
- **Marked.js** — Markdown parsing and rendering
- **Google Fonts** — Sora, Hind Siliguri, JetBrains Mono typography

---

## 🚀 Future Roadmap

- [ ] Chat history backup to cloud (encrypted)
- [ ] Real-time chat sharing with links
- [ ] Custom model fine-tuning
- [ ] Voice interface (Whisper + TTS)
- [ ] Web search integration
- [ ] Plugin ecosystem for tools/integrations

---

**Made with ❤️ by [Mahi Muhtasim](https://github.com/MahiMuhtasim)**

---

<div align="center">

⭐ If you find this useful, please star the repository!

</div>
