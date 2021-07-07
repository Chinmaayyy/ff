# Online-Forever
Make your Discord Account Online 24/7!

----

A Code written in Python that helps you to keep your account 24/7.

The [main.py](https://github.com/SealedSaucer/Online-Forever/blob/main/main.py) is the main file. [keep_alive.py](https://github.com/SealedSaucer/Online-Forever/blob/main/keep_alive.py) prevents your repl from going to sleep. (If you have a replit hacker plan, then you can delete [this file](https://github.com/SealedSaucer/Online-Forever/blob/main/keep_alive.py) and paste this code inside the [main.py](https://github.com/SealedSaucer/Online-Forever/blob/main/main.py) file : 

</br>

```py
import discord, os, asyncio, datetime, requests

from discord.ext import tasks, commands

client = commands.Bot(
  command_prefix=':',
  self_bot=True
)

async def on_ready():
    client.remove_command('help')
    await client.change_presence(status=discord.Status.online, activity=discord.Game("TEST"))
client.run(os.getenv("TOKEN"), bot=False)
```

Put your token instead of `TOKEN` in [main.py](https://github.com/SealedSaucer/Online-Forever/blob/main/main.py) and run the file.

**DO NOT GIVE YOUR TOKEN TO OTHERS!**

Use [uptimerobot.com](https://uptimerobot.com) to make your repl online 24/7.

----

> Online Forever © 2021 by SealedSaucer is licensed under Attribution 4.0 International 
