# Binance Moonbix-BOT

Binance Moonbix is an automated script for playing the Moon-bix game on the Binance platform. This bot is designed to automatically complete tasks, play the game, and collect tickets.

## Features

- Automatic task completion
- Automated Moonbix game play
- Proxy support
- Support multi accounts

## Requirements

- Node.js (version 14 or later)
- NPM (Node Package Manager)
- A Binance account with access to the Moon-bix game

## Registration

To participate in the Moon-bix game, you need to register using the following link:

[Register for Moonbix](https://t.me/Binance_Moonbix_bot/start?startApp=ref_6944804952&startapp=ref_6944804952&utm_medium=web_share_copy)

After registration, you will receive a queryString that you'll need to use with this bot.

## Installation

1. Clone this repository:

   ```
   git clone https://github.com/Galkurta/Moonbix-BOT.git
   ```

2. Navigate to the project directory:

   ```
   cd Moonbix-BOT
   ```

3. Install the required dependencies:
   ```
   npm install
   ```

## Configuration

1. Edit `data.txt` file in the project root directory and enter the Telegram queryString for each account on separate lines. You can obtain this queryString after registering and starting the game through the Telegram bot.

2. If you want to use a proxy, edit `config/config.json` file with your proxy configuration:
   ```json
   {
     "useProxy": true,
     "proxyProtocol": "http",
     "proxyHost": "your-proxy-host",
     "proxyPort": "your-proxy-port",
     "proxyAuth": {
       "username": "your-username",
       "password": "your-password"
     }
   }
   ```

## Usage

Run the bot with the command:

```
node main.js
```

The bot will prompt you whether you want to use a proxy or not. After that, it will start processing each account in `data.txt`.

## Warning

The use of this bot may violate Binance's Terms of Service. Use at your own risk. The author is not responsible for any consequences that may arise from using this bot.

## Contributing

Contributions are always welcome. Please make a pull request or open an issue for any suggestions and improvements.

## License

[MIT License](LICENSE)
