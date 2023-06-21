# OpenAI (ChatGPT) Discord Chat Bot

This repo is a Discord chat bot that uses OpenAI's GPT-3.5-turbo model to generate responses to user messages. In order to trigger the bot use '*' followed by the actual message

### Installation

Clone the repository to your local machine using git clone: 
	
    `git clone https://github.com/githmin/gpt-3.5-discord-chat-bot.git`

Install the required dependencies with: 
   	
    `npm install`

Create a `.env` file in the root of the project and set the following environment variables
	 
    `Discord_Token=<YOUR_DISCORD_TOKEN>`
	    
	`OpenAI_API=<YOUR_OPENAI_API_KEY>`

    
4.  Start the bot by running the following command:
    
    `node index.js`
    

### Dependencies

-   `dotenv` - To load environment variables from the `.env` file.
-   `discord.js` - To interact with the Discord API.
-   `openai` - To access the OpenAI GPT-3.5-turbo model API.

### Usage

The bot listens to messages in a specific Discord channel identified by `Channel_ID` environment variable. It generates a response to any message that starts with the "!" character. The bot generates the response using the OpenAI GPT-3.5-turbo model and sends it as a reply to the user who sent the message. The bot has access to last 20 messages to build a context.
