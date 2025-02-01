# Caption & Hashtag Recommender Bot 🤖

The **Caption & Hashtag Recommender Bot** is a Telegram bot that helps users generate captions and hashtags for their social media posts. Users can send either a text description or an image, and the bot will provide relevant hashtags and captions using the **Groq API** and **Groq Vision**.

This project is containerized using **Docker** for easy deployment and scalability.

---

## Features 🌟
- **Text Input**: Generate hashtags for a text description.
- **Image Input**: Generate captions and hashtags for an image.
- **AI-Powered**: Uses Groq API for text and image analysis.
- **Dockerized**: Easy to deploy using Docker.

---

## Tech Stack 🛠️
- **Python**: Backend logic.
- **Groq API**: For AI-based text and image analysis.
- **python-telegram-bot**: To interact with Telegram's API.
- **Docker**: For containerization and deployment.

---

## Prerequisites 📋
1. **Telegram Bot Token**: Create a bot using [BotFather](https://core.telegram.org/bots#botfather) and get the token.
2. **Groq API Key**: Sign up for [Groq API](https://groq.com/) and get your API key.
3. **Docker**: Install Docker from [here](https://docs.docker.com/get-docker/).

---

## How to Use 🚀

### 1. Clone the Repository
```bash
git clone https://github.com/We4TechAI/Caption-Hashtag-Recommender.git
cd Caption-Hashtag-Recommender
```

### 2. Set Up Environment Variables
Create a `.env` file in the root directory and add the following:
```env
TELEGRAM_BOT_TOKEN=your_telegram_bot_token
GROQ=your_groq_api_key
```

### 3. Build the Docker Image
```bash
docker build --tag caption_hashtag_recommender:latest .
```

### 4. Run the Docker Container
```bash
docker run -d --name caption_hashtag_recommender caption_hashtag_recommender:latest
```

---

## Bot Commands 🤖
1. **/start**: Start the bot and see a welcome message.
2. **Text Input**: Send a text description, and the bot will generate hashtags.
   - Example: `"Just had an amazing coffee at a cozy café!"`
   - Bot Response: `Generated Hashtags: #coffee #café #cozyvibes #coffeelover #coffeetime`
3. **Image Input**: Send an image, and the bot will generate a caption and hashtags.
   - Example: Send an image of a sunset.
   - Bot Response: `Caption and Hashtags: Beautiful sunset over the horizon. #sunset #nature #photography #sunsetlover #naturelover`

---

## Project Structure 📂
```
Caption-Hashtag-Recommender/
├── Dockerfile
├── README.md
├── requirements.txt
├── caption_hashtag_recommender.py
├── .env
```

### File Descriptions
- **Dockerfile**: Configuration for Docker container.
- **README.md**: This file.
- **requirements.txt**: Python dependencies.
- **bot.py**: Main bot logic.
- **.env**: Environment variables for API keys.







## Contributing 🤝
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeatureName`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeatureName`).
5. Open a pull request.





## Acknowledgments 🙏
- [Groq API](https://groq.com/) for providing the AI capabilities.
- [python-telegram-bot](https://python-telegram-bot.org/) for the Telegram bot framework.
- [Docker](https://www.docker.com/) for containerization.


Enjoy using the **Caption & Hashtag Recommender Bot**! 🎉
