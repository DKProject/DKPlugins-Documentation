---
title: Commands
---

# Commands

This page describes all available commands to operate DKCoins from the player chat and console.

Important things to remember about commands:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```
* Sub commands documented on another page are declared with ```...```

!!! note ""
All commands are customizable in commands.yml, therefore the commands may vary depending on your configuration.

## General commands
These commands are used to operate DKBans on your network or server.

* [```/dkbans```]()
* [```/dkbans info```]()
* [```/dkbans template```]()

## Punishment commands
Default punishment commands available by DKBans (You can completely change them with your templates and the command config)

* [```/ban <player> <template>```]()
* [```/tempban <player> <duration> <reason>```]()
* [```/permaban <player> <reason>```]()
  Mute commands are similar!
  

* [```/warn <player> <reason>```]()
* [```/kick <player> <reason>```]()

  Optionally, you can also configure templates for warning and kick.


* [```/punishInfo <player> <reason>```]()
* [```/banInfo <player> <reason>```]()

* [```/unpunish <player>```]()
* [```/unban <player>```]()

* [```/bans <player> <reason>```]()
* [```/mutes <player> <reason>```]()

## Report commands

* [```/report <player> <template>```]()
* [```/report take <player>```]()
* [```/report decline <player>```]()
* [```/report accept <player>```]()
* [```/report list```]()
* [```/dkbans login/logout```]()
* [```/dkbans template```]()

## Ip commands
These commands are used to operate DKBans on your network or server.

* [```/ipInfo <player>```]()
* [```/ipInfo <address>```]()
* [```/ipInfo <address> details```]()
  
* [```/ipblock <address> <reason> template <template> ```]()
* [```/ipblock <address> <reason> temporary  ```]()
* [```/ipblock <address> <reason> permanently ```]()

* [```/ipUnblock <address> ```]()

## History commands
* [```/history <player>```]()
* [```/history <player> <entryId>```]()
* [```/history <player> <entryId> changes```]()
* [```/history <player> <entryId> <versionId>```]()

* [```/resetHistory <player>```]()
* [```/resetHistory <player> last <amount/duration>```]()
* [```/resetHistory <player> by <staff>```]()
    
* [```/MyHistoryPoints```]()


## Player commands

* [```/playerInfo <player>```]()
* [```/playerSessions <player>```]()
* [```/onlineTime [player]```]()
* [```/jumpto <player>```]()
* [```/ping [player]```]()
* [```/playerNotes <player> [list]```]()
* [```/playerNotes <player> add <test>```]()
* [```/playerNotes <player> clear```]()


## Filter commands

* [```/filter list```]()
* [```/filter add <area> <value> [operation]```]()
* [```/filter remove <id>```]()

## Broadcast commands

* [```/broadcast ...```](broadcast-commands.md)
* [```/broadcastGroup ...```](broadcast-group-commands.md)

## Additional commands

* [```/joinme```]()
* [```/chatClear [local/global]```]()
* [```/teamChat <login/logout/toggle/message>```]()
* [```/chatlog player <player>```]()
* [```/chatlog server <server>```]()
* [```/help```]()
* [```/notify <login/logout/toggle>```]()
* [```/punishNotify <login/logout/toggle>```]()

