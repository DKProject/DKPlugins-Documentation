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
Default punishment commands available by DKBans.
You can completely change them with your templates and the command config, so command may vary
based on your configuration


* [```/ban <player> <template>```](punishment-commands.md#ban-player-template)
* [```/tempban <player> <duration> <reason>```](punishment-commands.md#tempban-player-duration-reason)
* [```/permaban <player> <reason>```](punishment-commands.md#permaban-player-reason) <br />
  Mute commands are similar! <br />


* [```/warn <player> <reason>```](punishment-commands.md#warn-player-reason)
* [```/kick <player> <reason>```](punishment-commands.md#kick-player-reason)

  Optionally, you can also configure templates for warning and kick.


* [```/punishInfo <player/id>```](punishment-commands.md#punishinfo-playerid)
* [```/banInfo <player/id>```](punishment-commands.md#punishinfo-playerid)

* [```/unban <player>```](punishment-commands.md#unban-player) <br />
  Mute commands are similar! <br />

* [```/bans <player> <page>```](punishment-commands.md#bans-player-page)
* [```/mutes <player> <page>```](punishment-commands.md#mutes-player-page)

## Report commands
Commands for players to report other players.

* [```/report <player> <template>```](report-commands.md#report-player-template)
* [```/report <player> <reason>```](report-commands.md#report-player-reason)
* [```/report accept <player>```](report-commands.md#report-accept-player)
* [```/report decline <player>```](report-commands.md#report-decline-player)
* [```/report take <player>```](report-commands.md#report-take-player)
* [```/report list```](report-commands.md#report-list)
* [```/report login/logout/toggle```](report-commands.md#report-loginlogouttoggle)

## Ip commands
Commands to view ip information of the player

* [```/ipInfo <player>```]()
* [```/ipInfo <address>```]()
* [```/ipInfo <address> details```]()
  
* [```/ipblock <address> <reason> template <template> ```]()
* [```/ipblock <address> <reason> temporary  ```]()
* [```/ipblock <address> <reason> permanently ```]()

* [```/ipunblock <address> ```]()

## History commands
Commands to view the player history.

* [```/history <player>```](history-commands.md#history-player)
* [```/history <player> <entryId>```](history-commands.md#history-player-entryid)
* [```/history <player> <entryId> changes```](history-commands.md#history-player-entryid-changes)
* [```/history <player> <entryId> <versionId>```](history-commands.md#history-player-entryid-versionid)

* [```/resetHistory <player>```](history-commands.md#resethistory-player)
* [```/resetHistory <player> last <amount/duration>```](history-commands.md#resethistory-player-last-amountduration)
* [```/resetHistory <player> by <staff>```](history-commands.md#resethistory-player-by-staff)

* [```/MyHistoryPoints```](history-commands.mdUp#myhistorypoints)


## Player commands
Player management commands.

* [```/playerInfo <player>```](player-commands.md#playerinfo-player)
* [```/playerSessions <player>```](player-commands.md#playersessions-player)
* [```/onlineTime [player]```](player-commands.md#onlinetime-player)
* [```/jumpto <player>```](player-commands.md#jumpto-player)
* [```/ping [player]```](player-commands.md#ping-player)
* [```/playerNotes <player> [list]```](player-commands.md#playernotes-player-list)
* [```/playerNotes <player> add <message>```](player-commands.md#playernotes-player-add-message)
* [```/playerNotes <player> clear```](player-commands.md#playernotes-player-clear)


## Filter commands
Commands to operate the filter system.

* [```/filter list```]()
* [```/filter add <area> <value> [operation]```]()
* [```/filter remove <id>```]()

## Broadcast commands
Commands to operate the broadcast system.

* [```/broadcast ...```](broadcast-commands.md)
* [```/broadcastGroup ...```](broadcast-group-commands.md)

## Additional commands
Additional commands provided by DKBans.

* [```/joinme```](additional-commands.md#joinme)
* [```/chatClear [local/global]```](additional-commands.md#chatclear-localglobal)
* [```/teamChat <login/logout/toggle/message>```](additional-commands.md#teamchat-loginlogouttogglemessage)
* [```/chatlog player <player>```](additional-commands.md#chatlog-player-player)
* [```/chatlog server <server>```](additional-commands.md#chatlog-server-server)
* [```/notify <login/logout/toggle>```](additional-commands.md#notify-loginlogouttoggle)
* [```/punishNotify <login/logout/toggle>```](additional-commands.md#punishnotify-loginlogouttoggle)
* [```/help```](additional-commands.md#help)

