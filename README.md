# upbeat

This a plugin for Slack's demonstration bot that plays a really basic RPG with anyone in the channel.

To run it, you need python-rtmbot: https://github.com/slackhq/python-rtmbot  Install and configure it as described in their docs. You'll need a Slack account and the ability to create a bot user to get very far.

Then install `rpgbot.py` from this repo in plugins/ or plugins/rpgbot/

It loads a config file called `gameconfig.json` in the rtmbot's working directory that should have the following stuff:
* RPGCHANNEL: the ugly Slack channel ID for the channel to use for the game (e.g. C123456789)
* DEBUG: true or false as you see fit
* SLACK_KEY: a Slack API key, preferably the same one you use for the rtmbot config
* IGNORELIST: [] of the user IDs (e.g. U123456789) you want to ignore. Sticking the bot's user ID in there is probably a good idea.


