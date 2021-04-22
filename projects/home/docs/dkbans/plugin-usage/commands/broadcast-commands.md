---
title: Broadcast Commands
---

# Broadcast Commands

This page describes the usage and permissions of the DKBans broadcast commands.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/broadcast <name> create <visibility> <text>```](#broadcast-name-create-visibility-text)
* [```/broadcast <name> delete```](#broadcast-name-delete)
* [```/broadcast <name> edit```](broadcast-edit-commands.md)
* [```/broadcast <name> direct```](#broadcast-name-direct)

***

## **```/broadcast <name> create <visibility> <text>```**

**Permission:** dkbans.command.broadcast<br />
**Arguments:**
* `<name>` The name of the broadcast
* `<visibility>` Display of the broadcast
* `text` The text to broadcast

This command creates a new broadcast with the given arguments.

Visibility:
* chat
* actionbar
* bossbar
* title

***

## **```/broadcast <name> delete```**

**Permission:** dkbans.command.broadcast<br />
**Arguments:**
* `<name>` The name of the broadcast

This command deletes the broadcast with the given ``name``.

***

## **```/broadcast <name> direct```**

**Permission:** dkbans.command.broadcast<br />
**Arguments:**
* `<name>` The name of the broadcast

This command broadcast the given broadcast directly to all players.