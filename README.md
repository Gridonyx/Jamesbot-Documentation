# Jamesbot
Jamesbot is a Discord bot created for the Aviencloud Discord server, the community server for the Aviencloud YouTube channel. Jamesbot originally started as a way to log server economy, but later evolved into a fully-fledged bot with moderator functionality and other useful utilities. The current Jamesbot is at version 2.

[Website](https://jamesbot.gridonyx.com/)

**Contents**

 - [Commands](#commands)
	 - [General](#general)
		 - [Avatar](#avatar)
		 - [Google](#google)
		 - [NSFW](#nsfw)
		 - [Poll](#poll)
		 - [Suggest](#suggest)
		 - [Urban](#urban)
		 - [YouTube](#youtube)
	 - [Economy](#economy)
		 - [Market](#market)
	 - [Events](#events)
		 - [Event](#event)
		 - [Eventcolor](#eventcolor)
	 - [Moderation](#moderation)
		 - [Ban](#ban)
		 - [Expmute](#expmute)
		 - [Expunmute](#expunmute)
		 - [Kick](#kick)
		 - [Mute](#mute)
		 - [Purge](#purge)
		 - [Refresh](#refresh)
		 - [Unmute](#unmute)
	 - [Utilities](#utilities)
		 - [Convert](#convert)
	 - [System](#system)
		 - [Help](#help)
		 - [Issue](#issue)
		 - [Mylevel](#mylevel)
		 - [Ping](#ping)
		 - [Set](#set)
		 - [Stats](#stats)

# Commands
The default command prefix for Jamesbot is %, but this can be customized.
All command arguments in **[ ]** (square brackets) are required, those in **{ }** (curly brackets) are optional.

## General
### Avatar
The Avatar command is used to retrieve your own, or someone else's, Discord avatar. 

**Command Use**

    %avatar {@user}
    %av {@user}

### Google
The Google command is used to retrieve the first result on Google for your included search terms.

**Command Use**

    %google [search]
    %g [search]

### NSFW
The NSFW command allows you to self-assign, or remove, the server's NSFW role, if that role does not exist this command will not work.

**Command Use**

    %nsfw

### Poll
The Poll command allows you to create a poll with up to ten options for people to select. **Please note that the quotation marks are required, and you must have at least two options.**

**Command Use**

    %poll "[question]" "[list,of,options,...]"
    %vote "[question]" "[list,of,options,...]"

### Suggest
The Suggest command allows you to create a suggestion that other people can vote on.

**Command Use**

    %suggest [suggestion]

### Urban
The Urban command is used to retrieve the first result on Urban Dictionary for your included search terms.

**Command Use**

    %urban [search]

### YouTube
The YouTube (YT) command is used to retrieve the first result on YouTube for your included search terms.

**Command Use**

    %yt [search]
    %youtube [search]

## Economy
### Market
The Market command is used to purchase monthly server roles. *Future expansion possible*.

**Command Use**

    %market role [rolename]
    %buy role [rolename]

## Events
### Event
The Event command is used by server staff to assign an event winner their appropriate role, while also removing the prior winner and custom role color (if changed by eventcolor command).

**Command Use**

    %event [art/karaoke/memes/music] [@user]
    %eventwinner [art/karaoke/memes/music] [@user]

### Eventcolor
The Eventcolor command is for event winners to change the color of their event role. **Please note, for the hexcode do not include the #.**

**Command Use**

    %eventcolor [hexcode]

## Moderation
### Ban
The Ban command is used by server staff to ban a member from the server.

**Command Use**

    %ban [@user] {reason}
    %kill [@user] {reason}

### Expmute
The EXPMute command is used by server staff to prevent a server member from earning Mee6 experience points. Can include optional duration (in minutes) and reason, default duration is 15 minutes.

**Command Use**

    %expmute [@user] {duration} {reason}

### Expunmute
The EXPUnmute command is used by server staff to manually remove an EXP Mute from a server member.

**Command Use**

    %expunmute [@user]

### Kick
The Kick command is used by server staff to kick a member from the server. Can include an optional reason.

**Command Use**

    %kick [@user] {reason}
    %boot [@user] {reason}

### Mute
The Mute command is used by server staff to mute a server member, which prevents them from sending messages. Can include optional duration (in minutes) and reason, default duration is 15 minutes.

**Command Use**

    %mute [@user] {duration} {reason}
    %silence [@user] {duration} {reason}
    %gag [@user] {duration} {reason}

### Purge
The Purge command is used by server staff to purge an included amount of messages from the server. Can optionally include a user to purge only their messages.

**Command Use**

    %purge [amount] {@user}
    %prune [amount] {@user}
    
### Refresh
The Refresh command is used by server staff to remove the monthly purchasable roles from all server members that have one.

**Command Use**

    %refresh
    %reset

### Unmute
The Unmute command is used by server staff to manually remove a Mute from a server member.

**Command Use**

    %unmute [@user]
    %ungag [@user]

## Utilities
### Convert
The Convert command is used to convert various units of measurement from the available list of units. Use %convert to get list of available units.

**Command Use**

    %convert
    %convert 12.2in
    %convert 164lb
    etc...

## System
### Help
The Help command is used to return a list of available commands a server member is able to use. You can include an optional command name to get specifics on the provided command.

**Command Use**

    %help {command}

### Issue
The Issue command is used by Server Administrators to report issues they may be experiencing with Jamesbot to the developer.

**Command Use**

    %issue [issue description]
    %botissue [issue description]
    %report [issue description]

### Mylevel
The Mylevel command returns your permissions level on the current server.

**Command Use**

    %mylevel
    
### Ping
The Ping command returns the ping and API latency times.

**Command Use**

    %ping

### Set
The Set command is used by Server Administrators to configure various server-specific settings like command prefix, welcome and leave channels, welcome and leave messages, role definitions, etc. To include a user ping in welcome and leave messages, please include *{{user}}*

**Command Use**

    %set [view / edit / reset] [key] [value]

**Available Keys**

    prefix, systemNotice, welcomeEnabled, leaveEnabled,
    adminRole, modRole, mutedRole, expMutedRole,
    modLogChannel, econLogChannel, welcomeChannel, welcomeMessage,
    leaveMessage

**Example**

    %set edit modLogChannel #mod-log

### Stats
The Stats command is used to return various information on the bot itself.

**Command Use**

    %stats
