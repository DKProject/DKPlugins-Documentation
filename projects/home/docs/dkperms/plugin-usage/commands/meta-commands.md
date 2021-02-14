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
* [```clear [scope]```](#clear-scope)
* [```list [scope]```](#list-scope)
* [```tree [scope]```](#tree-scope)
* [```show <key> [scope]```](#show-key-scope)
* [```check <key> [scope]```](#check-key-scope)


***

## **```set <key> <value> [duration] [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** s <br/>
**Arguments:**

* `<key>` The meta key (default or custom)
* `<value>` The value to set
* `[duration]` The duration of how long the value is set to this object
* `[scope]` On which scope the value is set

Sets a meta value (prefix, suffix etc.) to a user or group. 

***

## **```unset <key> [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** u <br/>
**Arguments:**

* `<key>` The meta key to remove
* `[scope]` On which scope the value should be removed

Removes a meta value from a user or group.

***

## **```clear [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** c <br/>
**Arguments:**

* `[scope]` On which scope the meta values should be cleared

Clears all meta values form a user or group

***


## **```list [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** l <br/>
**Arguments:**

* `[scope]` The scope to list

List all meta values of a user or group.

***

## **```tree [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** t <br/>
**Arguments:**

* `[scope]` The scope to start (if missing, the root scope is taken).

List the meta tree of a player or group.

***

## **```show <key> [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** s, get, g <br/>
**Arguments:**

* `<key>` The meta key to show
* `[scope]` On which scope the meta value should be showed

Show the current configuration of a meta value.

***

## **```check <key> [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** c, test <br/>
**Arguments:**

* `<key>` The name of the meta key to check
* `[scope]` The lowest scope to be checked (if missing, the current scope is taken)

Check which is the effected meta value (The check tests each level and gives feedback on the status).


