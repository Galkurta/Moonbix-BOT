# Binance Moonbix BOT

Binance Game Bot is an automated script for playing the Moon-bix game on the Binance platform. This bot is designed to automatically complete tasks, play the game, and collect tickets.

## Features

- Automatic task completion
- Automated Moon-bix game play
- Proxy support
- Comprehensive logging for monitoring and debugging

## Requirements

- Node.js (version 14 or later)
- NPM (Node Package Manager)
- A Binance account with access to the Moon-bix game

## Registration

To participate in the Moonbix, you need to register using the following link:

[Register for Moonbix](https://t.me/Binance_Moonbix_bot/start?startApp=ref_6944804952&startapp=ref_6944804952&utm_medium=web_share_copy)

After registration, you will receive a queryString that you'll need to use with this bot.

## Installation

1. Clone this repository:

   ```
   git clone https://github.com/Galkurta/Moonbix-BOT.git
   ```

2. Navigate to the project directory:

   ```
   cd Moonbix
   ```

3. Install the required dependencies:
   ```
   npm install
   ```

## Configuration

1. Edit `data.txt` file in the project root directory and enter the Telegram queryString for each account on separate lines. You can obtain this queryString after registering and starting the game through the Telegram bot.

2. If you want to use a proxy, Edit `config/config.json` file with your proxy configuration:
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

## Error Codes and Troubleshooting

While using the bot, you may encounter various error codes. Here's what they mean and how to address them:

- **503 Service Unavailable**: This error indicates that the Binance server is temporarily unable to handle the request. This could be due to maintenance or high traffic. Wait for a few minutes and try again.

- **429 Too Many Requests**: This error occurs when you've made too many requests in a short period. The bot will automatically wait and retry. If this persists, try increasing the delay between requests.

- **401 Unauthorized**: This typically means your access token is invalid or has expired. Try refreshing your queryString in the `data.txt` file.

- **400 Bad Request**: This error suggests that the request sent to the server was invalid. Double-check your configuration and ensure your queryString is correct.

- **404 Not Found**: This error indicates that the requested resource doesn't exist. Ensure you're using the correct API endpoints.

- **500 Internal Server Error**: This is a generic error message when an unexpected condition was encountered by the server. If this persists, check Binance's status page or contact their support.

If you encounter persistent errors or need further assistance, please open an issue on the GitHub repository with the specific error message and any relevant log output.

## Warning

The use of this bot may violate Binance's Terms of Service. Use at your own risk. The author is not responsible for any consequences that may arise from using this bot.

## Contributing

Contributions are always welcome. Please make a pull request or open an issue for any suggestions and improvements.

## License

[MIT License](LICENSE)
