# Automated Hypixel Tourney Bot
## Badges
![Twitch Status](https://img.shields.io/twitch/status/Cryptizism?color=%239146FF&label=Twitch&logo=Twitch) ![GitHub all releases](https://img.shields.io/github/downloads/Cryptizism/Hypixel-Bedwars-Tourney-Bot/total) ![GitHub](https://img.shields.io/github/license/Cryptizism/Hypixel-Bedwars-Tourney-Bot) ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/Cryptizism/Hypixel-Bedwars-Tourney-Bot) ![GitHub top language](https://img.shields.io/github/languages/top/Cryptizism/Hypixel-Bedwars-Tourney-Bot) ![Discord](https://img.shields.io/badge/Discord-Cryptizism%232999-%237289DA?logo=Discord) ![Build Status](https://img.shields.io/badge/Build-W.I.P-red)
## Liability
By running this software you agree that Cryptizism or any other distributors are not held liable including but not limited to: punishment of any sort on the Hypixel Network or any other servers, failure to work, and more.
## Requirements
- Java (You will already have this if you can run Minecraft)
- [Node.js Version 12 or over](https://nodejs.org/en/)
- A Minecraft account
  - Must be able to join Hypixel
  - Person running the bot must have MVP++ for private
- Discord server
  - Must have Manage Server role
- A bot that you own [(Click here to create)](https://discord.com/developers/applications/)
- Participants must have access "Slash command" privilege
## To-Do list
- [ ] Link Discord and Minecraft account
  - [x] Get name from API and see if it matches that of the end-user
  - [x] Change nickname to Minecraft name
  - [ ] Make a JSON/DB (file) to link Discord names and Minecraft names so people can't change their nickname and exploit the system
  - [ ] Give role with their respected team name
  - [ ] Create a JSON/DB (file) to hold teams and team members so there aren't too many roles and bulk
- [ ] Let moderators assign teams a round to play in
- [ ] Alert players in Discord DMs, Minecraft and in the server to get them ready, this will be triggered by a command a moderator will say
- [ ] Party all particpants 
- [ ] Let the particpants request an invite if: they were not ready, didn't get an invite or any other reason
- [ ] (Optional) Output stats of all players after game and post them in the discord

## Discord Commands
#### Commands starting with "/" use the "slash command" feature. Example: [1](https://support.discord.com/hc/en-us/articles/1500000368501-Slash-Commands-FAQ), [2](https://i.imgur.com/nU1htR2.png)
Comamnd : Description

#### Participants

/verify : Links your Discord and Minecraft account

/help : Shows all commands

/creator : Sends my Discord (Cryptizism#2999)

/current : Sends how long till a game starts or if there is a game going on

/invite : Requests another invite for bot if their round is up!

#### Moderators

tb!setup : Starts the setup process

tb!assign [Team Name] [round] : Assigns people who are in a team a round role

tb!notify [time] [round] : Notifs people with a round role that they are going up in `x` amount of time

tb!staff [@role] : Sets staff role defaults to people with admin perms

tb!players [@role] : Sets player role for pings

## Config
*Try not to change the below during the process as it will make it unstable*<br>
`TOURNEY_NAME` = Current tourney name for naming scheme and output images [default: "Bedwars Tournament"]<br>
`GAMEMODE` = Current tourney gamemode, [solo,doubles,3s,4s]<br>
`PER_GAME` = Teams per game [solo/doubles: 1-8, 3-4s: 4]<br>
`OUTPUT_BOOLEAN` = Whether or not to ouput stats<br>
`OUTPUT_CHANNEL` = Where to ouput stats of the game if it true<br>
`ANNOUNCEMENT_CHANNEL` = Where the bot will ping for the tourney<br>
`BRACKET_BOOLEAN` = Whether or not to output a bracket image<br>
`BRACKET_CHANNEL` = Where to output the bracket image<br>
`BRACKET_BG` = Bracket background image<br>
`IMG_PATH` = The path that the auto generated bracket will be located [default: ./images/brackets/{TOURNEY_NAME}] <br>

## Installation
1. Install everything in [prequisites](https://github.com/Cryptizism/Hypixel-Bedwars-Tourney-Bot#requirements)
2. Go into the .env file and replace `CLIENT_ID_HERE` with your Client ID, `SERVER_ID_HERE` with the Server ID, `API_KEY_HERE` with your hypixel api key
3. Open the start.bat file [(This will npm install ect.)](https://github.com/Cryptizism/Hypixel-Bedwars-Tourney-Bot/blob/main/README.md#what-does-the-bat-do-)
4. Open up Minecraft and go onto Hypixel
5. Use the bot and it should work!
6. Try not to touch anything as it may disturb the process

## FAQ
#### *"How does it work?"* <br> 
**First off it gets all the details from the staff members and players! Then after that it will, on command, initate a round inviting all the people that was assigned to be playing in that round. The way it invites people is VIA macro which is where the bot get's use at ur own risk. For the stats it reads your latest.log file and parses it line by line!**
<br>
#### *"Why should I tust it?"* <br>
**All the code is open source and at the end it is not even in an exe you can still view the code :)**
<br>
#### *"I have a question about this project"* <br>
**Fire me a DM on [Twitter](https://twitter.com/cryptizism) or on Discord (Cryptizism#2999)**
<br>
#### *"What does the bat do?"* <br>
**The `start.bat` file installs all of the dependancies and makes it run, this is for less tech literate users 👍🏿**
## Bugs
#### Robustness
- [ ] If player disconnects/lags out the bot may break
