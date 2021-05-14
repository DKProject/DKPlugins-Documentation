---
title: Player Commands
---

# Player Commands

This page describes the usage and permissions of the DKBans player commands.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/playerInfo <player>```](#playerinfo-player)
* [```/playerSessions <player>```](#playersessions-player)
* [```/onlineTime [player]```](#onlinetime-player)
* [```/jumpto <player>```](#jumpto-player)
* [```/ping [player]```](#ping-player)
* [```/playerNotes <player> [list]```](#playernotes-player-list)
* [```/playerNotes <player> add <message>```](#playernotes-player-add-message)
* [```/playerNotes <player> clear```](#playernotes-player-clear)
* [```/playerNotes <player> clear```](#playernotes-player-clear)

***

## **```/playerInfo <player>```**

**Alias:** pinfo <br/>
**Permission:** dkbans.command.playerInfo<br />
**Arguments:**
* `<player>` The name of the player

This command gives you an exact overview about a player. (ip, uuid, id, usw.)

***

## **```/playerSessions <player>```**

**Alias:** ccheat, cc <br/>
**Permission:** dkbans.command.playerSessions <br/>
**Arguments:**
* `<player>` The name of the player

Get exact information when the player was online.

***

## **```/onlineTime [player]```**

**Permission:** dkbans.command.onlinetime <br/>
**Arguments:**
* `<player>` The name of the player

Shows the online time of the player.

***

## **```/jumpto <player>```**

**Alias:** goto <br/>
**Permission:** dkbans.command.jumpto<br/>
**Arguments:**
* `<player>` The name of the player

Jump to a player on another server.

***

## **```/ping [player]```**

**Alias:** goto <br/>
**Permission:** 
  * dkbans.command.ping
  * dkbans.ping.other (Allows to show the ping of other players)
**Arguments:**
* `[player]` The name of the player

Get the ping of a player.

***

## **```/playerNotes <player> [list]```**

**Permission:** dkbans.command.playerNotes<br/>
**Arguments:**
* `<player>` The name of the player

List all internal notes of a player.

***

## **```/playerNotes <player> add <message>```**

**Permission:** dkbans.command.playerNotes<br/>
**Arguments:**
* `<player>` The name of the player
* `<message>` The message to add

Add a message to a player.

***

## **```/playerNotes <player> clear```**

**Permission:** dkbans.command.playerNotes<br/>
**Arguments:**
* `<player>` The name of the player

Clear all notes of a player.

***
