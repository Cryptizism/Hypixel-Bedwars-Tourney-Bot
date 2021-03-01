# Hypixel-Bedwars-Tourney-Bot [W.I.P]
## Liability
By running this software you agree that Cryptizism or any other distributors are not held liable if you are banned on the Hypixel network for using this.
## Badges
![Twitch Status](https://img.shields.io/twitch/status/Cryptizism?color=%239146FF&label=Twitch&logo=Twitch) ![GitHub all releases](https://img.shields.io/github/downloads/Cryptizism/Hypixel-Bedwars-Tourney-Bot/total) ![GitHub](https://img.shields.io/github/license/Cryptizism/Hypixel-Bedwars-Tourney-Bot) ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/Cryptizism/Hypixel-Bedwars-Tourney-Bot) ![GitHub top language](https://img.shields.io/github/languages/top/Cryptizism/Hypixel-Bedwars-Tourney-Bot) ![Discord](https://img.shields.io/badge/Discord-Cryptizism%232999-%237289DA?logo=Discord) ![Build Status](https://img.shields.io/badge/Build-W.I.P-red)
## Requirements
- Java (You will already have this if you can run Minecraft)
- Node.js Version 12 or over
- A Minecraft account
  - Must be able to join Hypixel
- Forge installed
  - Chattriggers mod installed
- Discord server
  - Must have Manage Server role
- A bot that you own [(Click here to create)](https://discord.com/developers/applications/)
- Participants must have access "Slash command" privilege
## To-Do list
- [ ] Link Discord and Minecraft account
  - [x] Get name from API and see if it matches that of the end-user
  - [x] Change nickname to Minecraft name
  - [ ] (Optional) Make a JSON file to link Discord names and Minecraft names so people can't change their nickname and exploit the system
  - [ ] Give role with their respected team name
  - [ ] (Optional) Create a JSON file to hold teams and team members so there aren't too many roles and bulk
- [ ] Let moderators assign teams a round to play in
- [ ] Alert players in Discord DMs and in Minecraft to get them ready, this will be triggered by a command a moderator will say
- [ ] Party all particpants 
- [ ] Let the particpants request an invite if: they were not ready, didn't get an invite or any other reason
- [ ] (Optional) Output stats of all players after game and post them in the discord
## Usage
#### Commands starting with "/" use the "slash command" feature. Example: [1](https://support.discord.com/hc/en-us/articles/1500000368501-Slash-Commands-FAQ), [2](https://i.imgur.com/nU1htR2.png)
Comamnd : Description

#### Participants

/verify : Links your Discord and Minecraft account

/help : Shows all commands

/creator : Sends my Discord (Cryptizism#2999)

/current : Sends how long till a game starts or if there is a game going on

#### Moderators

tb!around [Team Name] : Assigns people who are in a team a round role

tb!notify [time] [round] : Notifs people with a round role that they are going up in `x` amount of time

tb!stats [Y/N] : Toggles stats output after game (For this all players must turn kill message to default)

## Method
1. Install everything in requirements
2. Unzip the folder into C:\Users\[UR USER HERE]\AppData\Roaming\.minecraft\config\ChatTriggers\modules
3. Go into the .env file and replace `CLIENT_ID_HERE` with your Client ID and `Server_ID` with the Server ID
4. Open the start.bat file
5. Click on the link that has been outputed to your console
6. Open up Minecraft and go onto Hypixel
7. Use the bot and it should work!
