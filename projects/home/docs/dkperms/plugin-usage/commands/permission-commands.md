---
title: Permission Commands
---

# Permission Commands

This page describes the usage of DKPerms **permission-commands**. Those commands are sub commands of [user](user-commands.md) and
[group](group-commands.md) commands.

Important things to remember:
* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```set <permission> [action] [duration] [scope] [modifier]```](#set-permission-action-duration-scope-modifier)
* [```unset <permission> [scope]```](#unset-permission-scope)
* [```clear [scope]```](#clear-scope)
* [```list [scope]```](#list-scope)
* [```tree [scope]```](#tree-scope)
* [```show <permission> [scope]```](#show-permission-scope)
* [```check <permission> [scope]```](#check-permission-scope)


***

## **```set <permission> [action] [duration] [scope] [modifier]```**

**Permission:** dkperms.admin<br/>
**Alias:** s, add, a <br/>
**Arguments:**

* `<permission>` The permission to set
* `[action]` The action that should be used for this permission
* `[duration]` The duration of how long the object is permitted to this permission
* `[scope]` On which scope the permission should be assigned
* `[modifier]` An action, what should happen if the object already has this permission

This command sets a permission to a player, or a group.

**Available actions:**

* `+` Permits the player to this permission (default)
* `++` Permits the player always to this permission (Ignore hierarchy priorities)
* `-` Disallow the player to this permission(negative)
* `--` Disallow the player always to this permission (Ignore hierarchy priorities)

**Available modifiers:**

* `r` Replace the existing entry with the new configuration
* `f` Ignore and print an error message
* `a` accumulate the duration with the existing duration and keep the configuration.
* `l` Take the longest duration and keep the configuration.

***

## **```unset <permission> [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** u <br/>
**Arguments:**

* `<permission>` The permission to unset
* `[scope]` On which scope the permission should be removed

This command removes an assigned permission from a user or group.


***

## **```clear [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** c <br/>
**Arguments:**

* `[scope]` On which scope the group should be removed

Clear all permissions from a user or group.

***

## **```list [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** l <br/>
**Arguments:**

* `[scope]` The scope to list

List all permissions of a user or group.

***

## **```tree [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** t <br/>
**Arguments:**

* `[scope]` The scope to start (if missing, the root scope is taken).

List the permission tree of a player or group.

***

## **```show <permission> [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** s, get, g <br/>
**Arguments:**

* `<permission>` The name of the parent to show
* `[scope]` On which scope the permission should be showed

Show the current assignment configuration of a permission.

***

## **```check <permission> [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** c, test <br/>
**Arguments:**

* `<permission>` The name of the permission to check
* `[scope]` The lowest scope to be checked (if missing, the current scope is taken)

Check if the permission is allowed or disallowed (The check tests each level and gives feedback on the status).
