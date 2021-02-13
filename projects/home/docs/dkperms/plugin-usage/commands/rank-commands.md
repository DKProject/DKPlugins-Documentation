---
title: Rank Commands
---

# Rank Commands

DKPerms provides a simplified rank command to assign groups to players.

Important things to remember:
* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```


#### Index

* [```/rank```](#rank)
* [```/rank <player> list```](#rank-player-list)
* [```/rank <player> add <group> [action] [duration] [scope] [modifier]```](#rank-player-add-group-action-duration-scope-modifier)
* [```/rank <player> set <group> [action] [duration] [scope] [modifier]```](#rank-player-set-group-action-duration-scope-modifier)
* [```/rank <player> remove <group> [scope]```](#rank-player-remove-group-scope)
* [```/rank <player> promote [track]```](#rank-player-promote-track)
* [```/rank <player> demote [track]```](#rank-player-demote-track)

***

## **```/rank```**

**Permission:** dkperms.rank<br/>
**Alias:**  <br/>
**Arguments:**

This command lists your ranks, pair and allow this command to players.

***

## **```/rank <player> list```**

**Permission:** dkperms.rank.see.other<br/>
**Alias:** l <br/>
**Arguments:**

* `<player>` The selected player

List all ranks of a player.

***

## **```/rank <player> add <group> [action] [duration] [scope] [modifier]```**

**Permission:** dkperms.rank.change, dkperms.rank.change.<rank>, Higher priority as the player to modify <br/>
**Alias:** add <br/>
**Arguments:**

* `<player>` The selected player
* `<group>` The name of the parent to add
* `[action]` The action that should be used for this parent assignment
* `[duration]` The duration of how long the object should be in this parent
* `[scope]` On which scope the parent should be assigned
* `[modifier]` An action, what should happen if the object is already in this group

This command adds a permission group to a player

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

## **```/rank <player> set <group> [action] [duration] [scope] [modifier]```**

**Permission:** dkperms.rank.change, dkperms.rank.change.<rank>, Higher priority as the player to modify <br/>
**Alias:** s <br/>
**Arguments:**

* `<player>` The selected player
* `<group>` The name of the parent to add
* `[action]` The action that should be used for this parent assignment
* `[duration]` The duration of how long the object should be in this parent
* `[scope]` On which scope the parent should be assigned
* `[modifier]` An action, what should happen if the object is already in this group

This command sets a permission group to a player

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

## **```/rank <player> remove <group> [scope]```**

**Permission:** dkperms.rank.change, dkperms.rank.change.<rank>, Higher priority as the player to modify <br/>
**Alias:** a <br/>
**Arguments:**

* `<player>` The selected player
* `<group>` The name of the parent to add
* `[scope]` On which scope the parent should be assigned

This command removes a permission group to a player

## **```/rank <player> promote [track]```**

**Permission:** dkperms.rank.change, dkperms.rank.change.<rank>, Higher priority as the player to modify <br/>
**Alias:** i <br/>
**Arguments:**

* `<player>` The selected player
* `[track]` The track to take the group oder from, if not specified the groups are ordered by priority

Promote a player to the next group.

***

## **```/rank <player> demote [track]```**

**Permission:** dkperms.rank.change, dkperms.rank.change.<rank>, Higher priority as the player to modify <br/>
**Alias:** i <br/>
**Arguments:**

* `<player>` The selected player
* `[track]` The track to take the group oder from, if not specified the groups are ordered by priority

Demote a player to the next group.
