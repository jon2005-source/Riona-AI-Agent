
## Riona AI Agent 🌸

## Support the Project 🙌

### 🤝 **Open to Collaboration**
- [Twitter](https://twitter.com/david_patrick01)  - [Gmail](davidchuksdev@gmail.com)

If you'd like to support the development of Instagram-AI-Agent, please consider contributing to the following wallet addresses:

- **Bitcoin (BTC)**: 1GkWY6pjn7KoAkCnUab2MxnxeEQihknfUi
- **Ethereum (ETH-erc20)**: 0xabb45f4d85e7d9db5de684c35ccde7239a167cbb
- **Solana (SOL)**: EQV7fQ57zKNMFXy53WBfo2sCxtkRQVQLqj8sqWGnoyR

Your support helps keep this project running and growing! 🚀

Riona AI Agent is an AI-powered automation tool designed for **Instagram and Twitter** to automate social media interactions such as posting, liking, and commenting. It leverages advanced AI models to generate engaging content, automate interactions, and manage social media accounts efficiently.

Before using the automation features, you can personalize the agent by training with the following, including:
https://www.instagram.com/dreamlandofficial_1?igsh=NTZvcHRkNjlhYzhp
- **YouTube Video URL** 🎥
- **Audio File** 🎙️
- **Portfolio or Website Link** 🌐
- **File Formats Supported**: PDF, DOC, DOCX, TXT 📄

## Features

- **Instagram Automation**: Automatically log in, post photos, like posts, and leave thoughtful comments.
- **Twitter Automation**: Automatically tweet, retweet, and like tweets.
- **AI-Powered Content Generation**: Use Google Generative AI to create engaging captions and comments for Instagram and Twitter.
- **Proxy Support**: Use proxies to manage multiple accounts and avoid rate limits.
- **Cookie Management**: Save and load cookies to maintain sessions across restarts.

**Upcoming Features:**

GitHub automation is planned for future development.

## Installation

1. **Clone the repository**:

   ```sh
   git clone https://github.com/david-patrick-chuks/riona-ai-agent.git
   cd riona-ai-agent
   ```

2. **Install dependencies**:

   ```sh
   npm install
   ```

3. **Set up environment variables**:
   Rename `.env.example` to `.env` in the project root and fill your credentials.

   ```dotenv
   IGusername=your_instagram_username
   IGpassword=your_instagram_password

   Xusername=your_twitter_username
   Xpassword=your_twitter_password

   MONGODB_URI=mongodb://localhost:27017/instagram-ai-agent
   SESSION_SECRET=replace_with_a_random_secret
   ```

## Local run on Windows (Docker MongoDB + npm start)

1. **Start MongoDB in Docker Desktop**:

   ```powershell
   docker run -d -p 27017:27017 --name instagram-ai-mongodb mongodb/mongodb-community-server:latest
   ```

   Optional (with persistent volume):

   ```powershell
   docker run -d -p 27017:27017 --name instagram-ai-mongodb -v mongodb_data:/data/db mongodb/mongodb-community-server:latest
   ```

2. **Install packages**:

   ```powershell
   npm install
   ```

3. **Run the server**:

   ```powershell
   npm start
   ```

4. **Verify API health** (example):

   ```powershell
   curl http://localhost:3000/api
   ```

### Frontend behavior

This repository currently runs the backend API even when `frontend/dist/index.html` is absent.

- If `frontend/dist/index.html` exists, Express serves the static SPA.
- If it does not exist, the server logs a warning once and continues running API routes.
- Non-API routes return `404` with a JSON hint telling you to build/populate `frontend/dist`.

If you keep frontend in a separate repository, just run that frontend separately and point it to this API.

Useful Docker commands:

```powershell
docker ps
docker stop instagram-ai-mongodb
docker start instagram-ai-mongodb
docker rm instagram-ai-mongodb
docker rm -v instagram-ai-mongodb
```

## Usage

```sh
npm start
```

## Project Structure

- **src/client**: Contains the main logic for interacting with social media platforms like Instagram.
- **src/config**: Configuration files, including the logger setup.
- **src/utils**: Utility functions for handling errors, cookies, data saving, etc.
- **src/Agent**: Contains the AI agent logic and training scripts.
- **src/Agent/training**: Training scripts for the AI agent.
- **src/Agent/schema**: Schema definitions for AI-generated content and database models.
- **src/test**: Contains test data and scripts, such as example tweets.

## Logging

The project uses a custom logger to log information, warnings, and errors. Logs are saved in the [logs](http://_vscodecontentref_/3) directory.

## Error Handling

Process-level error handlers are set up to catch unhandled promise rejections, uncaught exceptions, and process warnings. Errors are logged using the custom logger.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Stargazers
Thank you to all our supporters!

[![Star History Chart](https://api.star-history.com/svg?repos=David-patrick-chuks/Riona-AI-Agent&type=Date)](https://www.star-history.com/#David-patrick-chuks/Riona-AI-Agent&Date)

## 

<p align="center">
Built with ❤️ by David Patrick 
</p>