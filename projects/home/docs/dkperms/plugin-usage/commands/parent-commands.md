---
title: Parent Commands
---

# Parent Commands

This page describes the usage of DKPerms **parent-commands**. Those commands are sub commands of [user](user-commands.md) and 
[group](group-commands.md) commands.

Important things to remember:
* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

!!! note ""
    Normally you use groups as parent (parent = group)

#### Index

* [```set <parent> [action] [duration] [scope] [modifier]```](#set-parent-action-duration-scope-modifier)
* [```add <parent> [action] [duration] [scope] [modifier]```](#add-parent-action-duration-scope-modifier)
* [```remove <parent> [scope]```](#remove-parent-scope)
* [```clear [scope]```](#clear-scope)
* [```list [scope]```](#list-scope)
* [```tree [scope]```](#tree-scope)
* [```show <parent> [scope]```](#show-parent-scope)
* [```check <parent> [scope]```](#check-parent-scope)

***

## **```set <parent> [action] [duration] [scope] [modifier]```**

**Permission:** dkperms.admin<br/>
**Alias:** s <br/>
**Arguments:**

* `<parent>` The name of the parent
* `[action]` The action that should be used for this parent assignment
* `[duration]` The duration of how long the object should be in this group
* `[scope]` On which scope the group should be assigned
* `[modifier]` An action, what should happen if the object is already in this group

This command sets a parent to a player, or a group, all assigned parents are removed from the player.

**Available actions:**

* `+` Allow the player to the group (default)
* `++` Allow the player always to the group (Ignore hierarchy priorities)
* `-` Disallow the player to the group (negative)
* `--` Disallow the player always to the group (Ignore hierarchy priorities)

**Available modifiers:**

* `r` Replace the existing entry with the new configuration
* `f` Ignore and print an error message
* `a` accumulate the duration with the existing duration and keep the configuration.
* `l` Take the longest duration and keep the configuration.

***

## **```add <parent> [action] [duration] [scope] [modifier]```**

**Permission:** dkperms.admin<br/>
**Alias:** a <br/>
**Arguments:**

* `<parent>` The name of the parent to add
* `[action]` The action that should be used for this parent assignment
* `[duration]` The duration of how long the object should be in this parent
* `[scope]` On which scope the parent should be assigned
* `[modifier]` An action, what should happen if the object is already in this group

This command adds a parent to a player or group, all assigned parents are kept.

**Available actions:**

* `+` Allow the player to the group (default)
* `++` Allow the player always to the group (Ignore hierarchy priorities)
* `-` Disallow the player to the group (negative)
* `--` Disallow the player always to the group (Ignore hierarchy priorities)

**Available modifiers:**

* `r` Replace the existing entry with the new configuration
* `f` Ignore and print an error message
* `a` accumulate the duration with the existing duration and keep the configuration.
* `l` Take the longest duration and keep the configuration.

***

## **```remove <parent> [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** c <br/>
**Arguments:**

* `<parent>` The name of the parent to remove
* `[scope]` On which scope the group should be removed

Remove an assigned parent from an object (user or group).

***

## **```clear [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** c <br/>
**Arguments:**

* `[scope]` On which scope the parents should be cleared

Clear all parent of an object (user or group). 

***

## **```list [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** l <br/>
**Arguments:**

* `[scope]` The scope to list

List all parents (groups) of an object.

***

## **```tree [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** t <br/>
**Arguments:**

* `[scope]` The scope to start (if missing, the root scope is taken).

List the parent tree of a player or group.

***

## **```show <parent> [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** s, get, g <br/>
**Arguments:**

* `<parent>` The name of the parent to show
* `[scope]` On which scope the parent should be showed

Show the current assignment configuration of an assigned parent.

***

## **```check <parent> [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** c, test <br/>
**Arguments:**

* `<parent>` The name of the parent to check
* `[scope]` The lowest scope to be checked (if missing, the current scope is taken)

Check if an object gets permissions from an assigned parent (The check tests each level and gives feedback on the status).
