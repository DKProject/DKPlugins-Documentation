---
title: Punishment Commands
---

# Punishment Commands

This page describes the usage and permissions of the DKBans punishment commands.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index
Default punishment commands available by DKBans.
You can completely change them with your templates and the command config, so command may vary 
based on your configuration


* [```/ban <player> <template>```](#ban-player-template)
* [```/tempban <player> <duration> <reason>```](#tempban-player-duration-reason)
* [```/permaban <player> <reason>```](#permaban-player-reason) <br />
  Mute commands are similar! <br />


* [```/warn <player> <reason>```](#warn-player-reason)
* [```/kick <player> <reason>```](#kick-player-reason)

  Optionally, you can also configure templates for warning and kick.


* [```/punishInfo <player/id>```](#punishinfo-playerid)
* [```/banInfo <player/id>```](#punishinfo-playerid)

* [```/unban <player>```](#unban-player) <br />
  Mute commands are similar! <br />

* [```/bans <player> <page>```](#bans-player-page)
* [```/mutes <player> <page>```](#mutes-player-page)

***

## **```/ban <player> <template>```**
Mute commands are similar!

**Alias:** ban,mute <br/>
**Permission:** dkbans.ban<br />
**Arguments:**
* `<player>` The name of the player
* `<template>` The id or name of the template

Punish a player with a preconfigured punishment templates (See [here](../../plugin-setup/punishment-templates.md) for more information).

***

## **```/tempban <player> <duration> <reason>```**
Mute commands are similar!

**Alias:** temporaryban, tban <br/>
**Permission:** dkbans.command.punish.ban.temporary <br/>
**Arguments:**
* `<player>` The name of the player
* `<duration>` The duration of the punishment (e.g. 10d 8h)
* `<reason>` The reason for this punish

Ban or mute a player temporarily

***

## **```/permaban <player> <reason>```**
Mute commands are similar!

**Alias:** permaban, pban <br/>
**Permission:** dkbans.command.punish.ban.permanently <br/>
**Arguments:**
* `<player>` The name of the player
* `<reason>` The reason for this punish

Ban or mute a player permanently

***

## **```/warn <player> <reason>```**

**Permission:** dkbans.command.punish.warn<br/>
**Arguments:**
* `<player>` The name of the player
* `<reason>` The reason for this warn

Warn a player.

***

## **```/kick <player> <reason>```**

**Permission:** dkbans.command.punish.kick<br/>
**Arguments:**
* `<player>` The name of the player
* `<reason>` The reason for this kick

Kick a player from the network.

***

## **```/punishInfo <player/id>```**

**Alias:** baninfo, muteinfo, binfo, minfo <br/>
**Permission:** dkbans.command.punishInfo<br/>
**Arguments:**
* `<player/id>` The name of the player

Get information about an active punishment.

***

## **```/unban <player>```**

**Permission:** dkbans.command.punish.ban.unban<br/>
**Arguments:**
* `<player>` The name of the player

Unban or unmute a player.

***

## **```/bans <player> <page>```**

**Permission:** dkbans.command.punish.ban.list<br/>
**Arguments:**
* `<player>` The name of the player
* `<page>` The page

List all active bans.

***

## **```/mutes <player> <page>```**

**Permission:** dkbans.command.punish.mute.list<br/>
**Arguments:**
* `<player>` The name of the player
* `<page>` The page

List all active mutes.
