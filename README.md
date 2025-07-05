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

### Quick Start (Recommended)
```bash
vibetext
```

**Note:** The first startup will set up Ollama and download the model, which may take a few minutes.


The `vibetext` command automatically:
- ✅ Starts Ollama server
- ✅ Starts VibeText backend  
- ✅ Opens the VibeText app
- ✅ Gemma2:9b model is pre-installed during brew install

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
- **@slack** - Transform text into professional Slack messages with proper markdown formatting
  - Auto-adjusts tone based on audience (teammates, manager, client, etc.)
  - Applies technical formatting: `backticks` for code, **bold** for emphasis, _italics_ for quotes
  - Formats links as clickable: `<URL|link text>`
  - **Setup Required:** Enable "Format messages with markup" in Slack preferences
  - **[➜ Slack Setup Guide](https://slack.com/help/articles/360039953113-Set-your-message-formatting-preference)**
- **@email** - Enhance emails while keeping your natural voice (supports formality levels)
- **@linkedin** - Create engaging, human-sounding LinkedIn posts with tone-specific emojis

## Quick Examples

**Slack Message:**
```
Step 1: @slack having issues with lambda function, can't find backoff v2.2.1
Step 2: teammates
Result: "Hey team! 🤔 I'm having issues with the `Lambda` function - it can't find version 2.2.1 of `backoff`. 
Has anyone worked with this before? I think I might need to add the Python SDK as a layer."
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

## 🔧 **Slack Setup for Best Results**

To get proper code formatting with backticks in Slack messages, you need to enable markup formatting:

1. In Slack, click your **Profile picture** → **Preferences**
2. Go to **Advanced** → **Input Options**  
3. Check **"Format messages with markup"**

📖 **[➜ See Slack's Official Setup Guide](https://slack.com/help/articles/360039953113-Set-your-message-formatting-preference)**

Without this setting, backticks around technical terms will show as literal characters instead of code formatting.

## Features

✨ **Simple Commands** - Just type @ or / to see available commands  
🎨 **Beautiful UI** - Modern, clean interface built with React and Tauri  
🤖 **Powered by Gemma2:9b** - Advanced AI via Ollama  
⚡ **Fast & Local** - All processing happens on your machine  
🔒 **Privacy First** - Your text never leaves your computer  
💬 **Multi-Platform Writing** - Optimized for Slack, Email, and LinkedIn  
🎭 **Smart Tone Adaptation** - AI auto-determines appropriate tone based on context  
😊 **Emoji Integration** - Adds contextually relevant emojis to enhance communication  
🔧 **Technical Formatting** - Automatically formats code terms, links, and technical content for Slack  
📝 **Markdown Support** - Proper bold, italic, code block, and link formatting  

## Requirements

- macOS 10.15 or later
- ~5GB free space for AI model
- Ollama (automatically installed as dependency)

## Technology Stack

- **Frontend:** React + Tauri
- **Backend:** Go
- **AI Runtime:** Ollama

## Support

- **Issues:** [GitHub Issues](https://github.com/shaharkozi/VibeText/issues)
- **Email:** shaharkozi12@gmail.com
- **Developer:** [Shahar Kozi](https://github.com/shaharkozi)

## License

MIT License - see the [LICENSE](https://github.com/shaharkozi/VibeText/blob/main/LICENSE) file for details.

---

Made with ❤️ by [Shahar Kozi](https://github.com/shaharkozi)
