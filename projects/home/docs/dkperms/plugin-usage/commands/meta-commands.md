---
title: Meta Commands
---

# Meta Commands

This page describes the usage of DKPerms **meta-commands**. Those commands are sub commands of [user](user-commands.md) and
[group](group-commands.md) commands.

Important things to remember:
* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```


**Default keys for groups**

* ```description <string>``` The description of the group (Showed in /team).
* ```default <boolean>``` If the group is default assigned to players.
* ```team <boolean>``` Shows that the group belongs to the server team.
* ```color <string>``` The color of the group. The color is displayed for example in ```/perms groups```. You can find the color codes on this website: https://www.digminecraft.com/lists/color_list_pc.php (replace § to &)
* ```chat <string>``` The chat format of the group.
* ```prefix <string>``` The tablist prefix of the group. The prefix is shown in front of the player name. This cannot be longer than 16 characters.
* ```suffix <string>``` The tablist suffix of the group. The suffix is displayed after the player name. This cannot be longer than 16 characters.

**Default keys for user**

* ```color <string>``` The color of the player.  (Normally taken from the group)
* ```chat <string>`` The chat format of the player (Normally taken from the group).
* ```prefix <string>``` The tablist prefix of the user. The prefix is shown in front of the player name. This cannot be longer than 16 characters (Normally taken from the group)
* ```suffix <string>``` The tablist suffix of the user. The suffix is displayed after the player name. This cannot be longer than 16 characters (Normally taken from the group)


#### Index

* [```set <key> <value> [duration] [scope]```](#set-key-value-duration-scope)
* [```unset <key> [scope]```](#unset-key-scope)
* [```show <key> [scope]```](#show-key-scope)
* [```clear [scope]```](#clear-scope)
* [```list [scope]```](#list-scope)
* [```tree [scope]```](#tree-scope)


***

## **```set <key> <value> [duration] [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** s <br/>
**Arguments:**

* `<key>` The name of the parent to show
* `[value]` On which scope the permission should be showed

Show the current assignment configuration of a permission.

***

## **```unset <key> [scope]```**
Remove a meta from a group/player.

***

## **```show <key> [scope]```**
Shows information about the set meta.

***

## **```clear [scope]```**
Clear all added metas.

***

## **```list [scope]```**
List all added metas of the scope.

***

## **```tree [scope]```**
List all added metas.

