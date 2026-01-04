# 🐾 WWF Animal Identification Bot

A Telegram bot that uses Google Gemini AI to identify animal species from photos.

![Node.js](https://img.shields.io/badge/Node.js-18+-green)
![Telegram](https://img.shields.io/badge/Telegram-Bot-blue)
![Google Gemini](https://img.shields.io/badge/Google-Gemini%20AI-orange)

## ✨ Features

- 📸 Upload animal photos to identify species
- 🤖 AI-powered identification using Google Gemini
- 🔍 Get scientific names and common names
- 📱 Easy-to-use Telegram interface

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- Telegram account
- Google AI Studio API key

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/WWF-Animal-Identification.git
   cd WWF-Animal-Identification
   ```

2. **Install dependencies**
   ```bash
   cd backend/node
   npm install
   ```

3. **Create a Telegram Bot**
   - Open Telegram and search for `@BotFather`
   - Send `/newbot` and follow the prompts
   - Copy the bot token

4. **Get Google Gemini API Key**
   - Go to [Google AI Studio](https://aistudio.google.com/)
   - Create an API key

5. **Configure environment variables**
   ```bash
   cp .env.example .env
   ```
   Edit `.env` with your credentials:
   ```env
   TELEGRAM_BOT_TOKEN=your_telegram_bot_token
   GEMINI_API_KEY=your_gemini_api_key
   PORT=3001
   ```

6. **Start the bot**
   ```bash
   npm start
   ```

## 📖 Usage

1. Open Telegram and find your bot
2. Send `/start` to begin
3. Upload a photo of an animal
4. Send `/identify` to identify the species

**💡 Tip:** You can also send a photo with the caption `/identify` for instant identification!

## 🤖 Bot Commands

| Command | Description |
|---------|-------------|
| `/start` | Start the bot and see welcome message |
| `/help` | Get usage instructions |
| `/identify` | Identify the last uploaded animal photo |

## 🛠️ Tech Stack

- **Runtime:** Node.js
- **Bot Framework:** Telegraf
- **AI:** Google Gemini
- **Server:** Express.js

## 📁 Project Structure

```
backend/node/
├── bin/
│   └── www              # Entry point
├── src/
│   ├── app.js           # Express app setup
│   ├── bot.js           # Telegram bot logic
│   ├── Controller/
│   │   └── Identify/
│   │       └── identifyController.js
│   ├── routes/
│   │   └── identifyRoutes.js
│   ├── services/
│   │   └── animalIdentifier.js    # Gemini AI integration
│   └── utils/
│       └── fileHandler.js
├── .env                 # Environment variables (not committed)
└── package.json
```

## 🔒 Environment Variables

| Variable | Description |
|----------|-------------|
| `TELEGRAM_BOT_TOKEN` | Your Telegram bot token from BotFather |
| `GEMINI_API_KEY` | Google AI Studio API key |
| `PORT` | Server port (default: 3001) |

## 📝 License

This project is licensed under the MIT License.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---

Made with ❤️ for wildlife conservation
