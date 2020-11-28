# Discord-bot-making
A tutorial for making bots on discord
Readme:
# Discord-bot-making
 In this tutorial we will be learning to make discord bots step by step with python discord.py.
Previous knowledge:
If You know what is dicord developer portal then good and if no then search disocrd developer portal on google and click on the first site. On the top of the site you will get an option New Application. Click on it and write your project name.ON your left-hand-side you will get few options(Settings, OAUth2, Rich Presence and App whitelist).
Click on bot and you will get an option to reveal a token. Now click on OAuth2, scroll down and select bot. You'll get a link. Copy paste it to invite your bbot to your discord server. open command prompt and write pip install discord.py and open python.


Code:
import discord
from discord.ext import commands

client = discord.Bot(command_prefix='!') # You can give any prefix. Like the prefix of MEE6 is !

@client.event
async def on_ready():
    print('Bot is ready') # If this code comes it means your bot has no error
    
client.run('Your token here')# Copy paste the token you had recieved.
