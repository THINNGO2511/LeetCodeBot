# LeetCode Discord Bot

A Discord bot coded up by me having a headache rn, designed to help me and friends practice 4 LeetCode problems every dyaconsistently. The bot sends daily problems across various topics and difficulty levels, helping users maintain a steady learning pace and track their progress.

## Features

- **Daily Problem Delivery**: Automatically sends curated LeetCode problems at 7 AM Eastern Standard Time
- **Topic Coverage**: Includes problems on:
  - Prefix Sum
  - Sliding Window
  - Binary Search
  - Linked Lists
  - Depth-First Search (DFS)
  - And many more algorithms
- **Admin Controls**:
  - Manual problem triggering
  - Topic management
  - Problem database expansion

## Commands

| Command | Description | Access Level |
|---------|-------------|--------------|
| `!next` | Triggers next day's problems | Admin |
| `!topics` | Lists all available problem topics | All Users |
| `!addproblem <topic> <title> <difficulty> <url>` | Adds new problem to database | Admin |

## Setup Instructions

### Prerequisites

- Python 3.8 or higher
- Discord Bot Token ([Create one here](https://discord.com/developers/applications))

### Installation Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/THINNGO2511/LeetCodeBot.git
   cd LeetCodeBot
   ```

2. Set up virtual environment (recommended):
   ```bash
   python -m venv venv
   # On Unix/macOS:
   source venv/bin/activate
   # On Windows:
   venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Configure environment variables:
   - Create a `.env` file in the project root
   - Add the following variables:
     ```plaintext
     DISCORD_TOKEN=your_discord_bot_token
     CHANNEL_ID=your_channel_id
     ```

5. Initialize problem database:
   - Ensure `problems.json` exists in the root directory
   - Verify it contains properly structured problem data

## Usage

1. Start the bot:
   ```bash
   python bot.py
   ```

2. The bot will:
   - Connect to Discord
   - Begin sending daily problems at 7 AM UTC
   - Monitor channels for commands
   - Log activities for troubleshooting

## Project Structure

```
LeetCodeBot/
├── venv                # virtual environment variables
├── your_aws_KV.pem     # Connect with AWS
├── bot.py              # Main bot logic
├── problems.json       # Problem database
├── requirements.txt    # Dependencies
├── .env                # Configuration
└── README.md           # Documentation
```

## Contributing

We welcome contributions! To contribute:

1. Fork the repository
2. Create a feature branch
3. Implement your changes
4. Submit a pull request with detailed descriptions

Please ensure your code follows our style guidelines and includes appropriate tests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [LeetCode](https://leetcode.com/) for providing the problem content
- [discord.py](https://discordpy.readthedocs.io/) for the Discord API wrapper
- All contributors who have helped improve problem list
- Me (edward)

---
*Note: For the latest updates and detailed API documentation, please check our [GitHub repository](https://github.com/THINNGO2511/LeetCodeBot).*
