---
title: Broadcast Edit Commands
---

# Broadcast Edit Commands

This page describes the usage and permissions of the DKBans broadcast edit commands.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/broadcast <name> edit name <name>```](#broadcast-name-edit-name-name)
* [```/broadcast <name> edit visibility <visibility>```](#broadcast-name-edit-visibility-visibility)
* [```/broadcast <name> edit property [list]```](#broadcast-name-edit-property-list)
* [```/broadcast <name> edit property add <key> <value>```](#broadcast-name-edit-property-add-key-value)
* [```/broadcast <name> edit property remove <key>```](#broadcast-name-edit-property-remove-key)

***

## **```/broadcast <name> edit name <name>```**

**Permission:** dkbans.command.broadcast<br />
**Arguments:**
* `<name>` The name of the broadcast

This command changes the name of the broadcast.

***

## **```/broadcast <name> edit visibility <visibility>```**

**Permission:** dkbans.command.broadcast<br />
**Arguments:**
* `<name>` The name of the broadcast
* ``visibility`` The new visibility of the broadcast

This command changes the visibility of the broadcast.

***

## **```/broadcast <name> edit property [list]```**

**Permission:** dkbans.command.broadcast<br />
**Arguments:**
* `<name>` The name of the broadcast

This command lists all properties of the given broadcast

***

## **```/broadcast <name> edit property add <key> <value>```**

**Permission:** dkbans.command.broadcast<br />
**Arguments:**
* `<name>` The name of the broadcast
* ``<key>`` The key of the property
* ``<value>`` The value of the property

This command adds a property to the broadcast.

Default properties:
- text
- stay (actionbar, title, bossbar)
- subtitle (title)
- fade-in (title)
- fade-out (title)
- bar-color (bossbar)
***

## **```/broadcast <name> edit property remove <key>```**

**Permission:** dkbans.command.broadcast<br />
**Arguments:**
* `<name>` The name of the broadcast
* ``<key>`` The key of the property

This command removes a property of the broadcast.
***