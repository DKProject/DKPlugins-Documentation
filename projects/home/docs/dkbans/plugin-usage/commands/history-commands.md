---
title: History Commands
---

# History Commands

This page describes the usage and permissions of the DKBans history commands.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/history <player>```](#history-player)
* [```/history <player> <entryId>```](#history-player-entryid)
* [```/history <player> <entryId> changes```](#history-player-entryid-changes)
* [```/history <player> <entryId> <versionId>```](#history-player-entryid-versionid)

* [```/resetHistory <player>```](#resethistory-player)
* [```/resetHistory <player> last <amount/duration>```](#resethistory-player-last-amountduration)
* [```/resetHistory <player> by <staff>```](#resethistory-player-by-staff)

* [```/MyHistoryPoints```](#myhistorypoints)

***

## **```/history <player>```**

**Permission:** dkbans.command.history<br />
**Arguments:**
* `<player>` The name of the player

View all historical punishments of this player.

***

## **```/history <player> <entryId>```**

**Permission:** dkbans.command.history <br/>
**Arguments:**
* `<player>` The name of the player
* `<entryId>` The name of the player

View details about a punishment.

***

## **```/history <player> <entryId> changes```**

**Permission:** dkbans.command.history <br/>
**Arguments:**
* `<player>` The name of the player
* `<entryId>` The name of the player

View changes of this punishment. DKBans has an integrated logging system to track changes of a punishment.

***

## **```/history <player> <entryId> <versionId>```**

**Permission:** dkbans.command.history<br/>
**Arguments:**
* `<player>` The name of the player
* `<entryId>` The name of the player
* `<versionId>` The id of the version

View an older change of a punishment

***

## **```/resetHistory <player>```**

**Permission:** dkbans.command.resethistory<br/>
**Arguments:**
* `<player>` The name of the player

Reset the history of a player.

***

## **```/resetHistory <player> last <amount/duration>```**

**Permission:** dkbans.command.resethistory<br/>
**Arguments:**
* `<player>` The name of the player
* `<amount/duration>` The amount of entries to delete or the duration

Reset the history of a player for a specified time period.

***

## **```/resetHistory <player> by <staff>```**

**Permission:** dkbans.command.resethistory<br/>
**Arguments:**
* `<player>` The name of the player
* `<staff>` The name of the staff

Reset the history of a player by a specific staff member.

***

## **```/MyHistoryPoints```**

**Permission:** dkbans.command.myhistorypoints<br/>

Player can view there history points with this command.

***
