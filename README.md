DayZ Modding Assistant Bot

A Discord bot powered by OpenAI GPT-4o, built specifically to help the DayZ modding community. It provides clear and detailed help with config files, Enforce Script, item retexturing and general modding workflows.

What It Can Do:

- Answer modding questions using !mod
- Provide guidance on config.cpp, mod.cpp and Enforce Script
- Help with item retexturing, texture formats, material config and more
- Offer testing and setup advice
- Strictly focused on DayZ modding practices

Bot Commands:

!mod <question>      Ask a DayZ modding question  
!modhelp             Show command list  
!modping             Confirm bot is running  
!modabout            Info about this bot  

Example:
!mod how do I retexture the M65 jacket?

How to Use This Bot on Your Own Server:

You must host your own copy of this bot and configure it with your own tokens.

Step 1: Create a Discord Bot

1. Go to the Discord Developer Portal: https://discord.com/developers/applications
2. Click "New Application"
3. Name it (e.g., DayZ Modding Assistant)
4. Go to the "Bot" tab and click "Add Bot"
5. Copy the Bot Token
6. Enable "Message Content Intent"

Step 2: Invite Your Bot to a Server

1. Go to "OAuth2 > URL Generator"
2. Select Scopes:
   - bot
   - applications.commands
3. Select Bot Permissions:
   - Read Messages/View Channels
   - Send Messages
   - Read Message History
   - Use Slash Commands (optional)
4. Copy the generated invite link
5. Open it in your browser and authorise the bot to join your server

Setting It Up on Replit:

1. Go to https://replit.com and sign in or create an account
2. Create a new Repl (choose Python as the language)
3. Copy all the files from this repository into your Repl:
   - main.py
   - .env.example
   - requirements.txt
4. Click the "Secrets" tab in the left sidebar (key icon)
5. Add the following environment variables:
   - DISCORD_TOKEN = your Discord bot token
   - OPENAI_API_KEY = your OpenAI key
6. Click the green "Run" button

Your bot will now come online and respond to commands like:
!mod how do I add a new backpack?

General Setup (If Not Using Replit):

1. Clone This Repository:

git clone https://github.com/YOUR_USERNAME/dayz-modding-bot.git
cd dayz-modding-bot

2. Install Requirements:

pip install -r requirements.txt

3. Create Your .env File:

Create a file named .env in the project root and add:

DISCORD_TOKEN=your_discord_bot_token_here  
OPENAI_API_KEY=your_openai_api_key_here

4. Run the Bot:

python main.py

Example Use:

!mod how do I add a custom suppressor?

Files Included:

main.py          - The bot logic  
.env.example     - Template for your API tokens  
README.md        - Setup instructions and bot info  
requirements.txt - Python packages needed to run the bot  

Support Policy:

This project is provided as-is. No support or assistance will be given.  
Use it at your own discretion. You’re free to fork, modify, and host your own copy.

Powered By:

OpenAI GPT-4o  
discord.py
