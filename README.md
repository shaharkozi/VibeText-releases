# VibeText 

🍺 Official Homebrew tap for [VibeText](https://github.com/shaharkozi/VibeText) - Your AI-powered text assistant.

## Installation

```bash
# Add the tap
brew tap shaharkozi/hombrew-formulas https://github.com/shaharkozi/hombrew-formulas.git

# Install VibeText
brew install shaharkozi/hombrew-formulas/vibetext
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

- **@prettier** - Polish and improve text quality
- **@fixGrammar** - Fix grammatical errors
- **@rephrase** - Rewrite in different styles  
- **@changeTone** - Adjust tone (formal, casual, friendly, etc.)
- **@summarize** - Create concise summaries
- **@translate** - Translate to different languages

## Features

✨ **Simple Commands** - Just type @ or / to see available commands  
🎨 **Beautiful UI** - Modern, clean interface built with React and Tauri  
🤖 **Powered by Llama 3** - Advanced AI via Ollama  
⚡ **Fast & Local** - All processing happens on your machine  
🔒 **Privacy First** - Your text never leaves your computer  

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