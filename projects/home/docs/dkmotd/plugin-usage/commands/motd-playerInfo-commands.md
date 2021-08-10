---
title: Motd playerinfo Commands
---

# Motd playerinfo Commands

This page describes the usage and permissions of the Motd commands. The motd command always
starts with `/motd <name> playerInfo`, while `<name>` is the name of the motd template.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/motd <name> playerInfo add <line>```](#motd-name-playerinfo-add-line)
* [```/motd <name> playerInfo remove <index>```](#motd-name-playerinfo-remove-index)
* [```/motd <name> playerInfo set <line>```](#motd-name-playerinfo-set-line)
* [```/motd <name> playerInfo modify <index> <line>```](#motd-name-playerinfo-modify-index-line)
* [```/motd <name> playerInfo clear```](#motd-name-playerinfo-clear)
***

## **```/motd <name> playerInfo add <line>```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `<name>` the name of motd template
* `<line>` the new line to be added

This command adds a new line to the player info

***

## **```/motd <name> playerInfo remove <index>```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `<name>` the name of motd template
* `<index>` the index to remove

This command removes a new line of the player info by the index of the player info.

***

## **```/motd <name> playerInfo set <line>```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `<name>` the name of motd template
* `<line>` the line to set

This command sets the line of the player info and removes all other player info lines.

***

## **```/motd <name> playerInfo modify <index> <line>```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `<name>` the name of motd template
* ``<index>`` the index to modify
* `<line>` the modified line

This command modifies the line of the ``<index>`` to `<line>`.

***

## **```/motd <name> playerInfo clear```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `<name>` the name of motd template

This command clears the player info of the motd template.

***