# VibeText Homebrew Tap

🍺 Official Homebrew tap for [VibeText](https://github.com/shaharkozi/VibeText) - Your AI-powered text assistant.

## Installation

```bash
# Add the tap
brew tap shaharkozi/homebrew-formulas https://github.com/shaharkozi/homebrew-formulas.git

# Install VibeText
brew install shaharkozi/homebrew-formulas/vibetext
```

## 🚀 Launch VibeText

### Option 1: Quick Start (Recommended)
```bash
vibetext
```

### Option 2: Add to Applications
**📱 For easier access, drag the app to Applications:**
```bash
# This opens Finder and highlights the app - just drag it to Applications!
open -R $(brew --prefix)/Cellar/vibetext/*/*.app
```

> **Note:** If you see a permission error when installing, you can manually drag the app from the Homebrew directory to your Applications folder, or run it directly using the `vibetext` command.

The `vibetext` command automatically:
- ✅ Starts Ollama server
- ✅ Starts VibeText backend  
- ✅ Opens the VibeText app
- ✅ Llama 3 model is pre-installed during brew install

**To stop everything:**
```bash
killall vibetext-backend ollama
```

### Manual Setup (if needed)
```bash
vibetext-backend    # Start backend only
ollama serve        # Start Ollama only
```

## What is VibeText?

VibeText is an intelligent desktop application that helps you improve your writing with powerful AI commands:

### 📝 **Text Enhancement**
- **@prettier** - Polish and improve text quality
- **@fixGrammar** - Fix grammatical errors
- **@rephrase** - Rewrite in different styles  
- **@changeTone** - Adjust tone (formal, casual, friendly, etc.)

### 💼 **Professional Communication**
- **@slack** - Transform text into professional Slack messages (auto-adjusts tone based on audience)
- **@email** - Enhance emails while keeping your natural voice (supports formality levels)
- **@linkedin** - Create engaging, human-sounding LinkedIn posts with tone-specific emojis

## Quick Examples

**Slack Message:**
```
Step 1: @slack hey can u send me that file asap thx
Step 2: teammates
Result: "Hi! Could you send me that file when you get a chance? Thanks!"
```

**LinkedIn Post:**
```
Step 1: @linkedin just shipped our new feature after months of work
Step 2: excited  
Result: "Just shipped something I've been working on! 🚀 It's been a wild ride but totally worth it..."
```

**Email Enhancement:**
```
Step 1: @email hi john, can you review this code when u get a chance
Step 2: semi-formal
Result: "Hi John, Could you please review this code when you have time? Thanks, [Your name]"
```

## Features

✨ **Simple Commands** - Just type @ or / to see available commands  
🎨 **Beautiful UI** - Modern, clean interface built with React and Tauri  
🤖 **Powered by Llama 3** - Advanced AI via Ollama  
⚡ **Fast & Local** - All processing happens on your machine  
🔒 **Privacy First** - Your text never leaves your computer  
💬 **Multi-Platform Writing** - Optimized for Slack, Email, and LinkedIn  
🎭 **Smart Tone Adaptation** - AI auto-determines appropriate tone based on context  
😊 **Emoji Integration** - Adds contextually relevant emojis to enhance communication  

## Requirements

- macOS 10.15 or later
- ~4GB free space for AI model
- Ollama (automatically installed as dependency)

## Technology Stack

- **Frontend:** React + Tauri
- **Backend:** Go
- **AI Runtime:** Ollama
- **AI Model:** Llama 3

## Support

- **Issues:** [GitHub Issues](https://github.com/shaharkozi/VibeText/issues)
- **Email:** shaharkozi12@gmail.com
- **Developer:** [Shahar Kozi](https://github.com/shaharkozi)

## License

MIT License - see the [LICENSE](https://github.com/shaharkozi/VibeText/blob/main/LICENSE) file for details.

---

Made with ❤️ by [Shahar Kozi](https://github.com/shaharkozi)
