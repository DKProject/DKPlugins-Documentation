---
title: Commands
---

# Commands

This page describes all available commands to operate DKPerms from the player chat and console.

Important things to remember about commands:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```
* Sub commands documented on another page are declared with ```...```

## General commands
These commands are used to operate DKPerms on your network or server.

* [```/perms```](general-commands.md#perms)
* [```/perms info```](general-commands.md#perms-info)
* [```/perms sync```](general-commands.md#perms-sync)
* [```/perms migrate```](general-commands.md#perms-migrate-system)
* [```/perms groups```](general-commands.md#perms-groups)
* [```/perms group <group>```](general-commands.md#perms-group-group-)
* [```/perms user <user>```](general-commands.md#perms-user-player-)
* [```/perms track <track>```](general-commands.md#perms-track-track-)
* [```/perms analyse```](general-commands.md#perms-analyse-action)

## User commands
These commands are for manging user permissions, groups and metadata.

```<player> ``` The name or unique id of the player.

* [```/perms user <player> info```](user-commands.md#perms-user-player-info)
* [```/perms user <player> permission```](user-commands.md#perms-user-player-permission-)
* [```/perms user <player> meta```](user-commands.md#perms-user-player-meta-)
* [```/perms user <player> parent```](user-commands.md#perms-user-player-parent-)

## Group commands
Commands for manging groups. ```<group> ``` is the name of the group.

* [```/perms group <group> info```](group-commands.md#perms-group-group-create)
* [```/perms group <group> create```](group-commands.md#perms-group-group-create)
* [```/perms group <group> delete```](group-commands.md#perms-group-group-delete)
* [```/perms group <group> rename <newname>```](group-commands.md#perms-group-group-rename-newname)
* [```/perms group <group> copy <newname>```](group-commands.md#perms-group-group-copy-newname)
* [```/perms group <group> members [scope]```](group-commands.md#perms-group-group-rename-newname)
* [```/perms group <group> permission```](group-commands.md#perms-group-group-permission)
* [```/perms group <group> meta```](group-commands.md#perms-group-group-meta)
* [```/perms group <group> group```](group-commands.md#perms-group-group-group)
* [```/perms group <group> setPriority <priorit> ```](group-commands.md#perms-group-group-setpriority-priorit)

## Permission commands
Sub commands to assign permissions to users and groups.

* [```permission set <permission> [action] [duration] [scope] [modifier]```](permission-commands.md#set-permission-action-duration-scope-modifier)
* [```permission unset <permission> [scope]```](permission-commands.md#unset-permission-scope)
* [```permission clear [scope]```](permission-commands.md#clear-scope)
* [```permission list [scope]```](permission-commands.md#list-scope)
* [```permission tree [scope]```](permission-commands.md#tree-scope)
* [```permission show <permission> [scope]```](permission-commands.md#show-permission-scope)
* [```permission check <permission> [scope]```](permission-commands.md#check-permission-scope)

## Parent commands

Sub commands to assign parents (groups) to users and groups.

* [```parent set <parent> [action] [duration] [scope] [modifier]```](parrent-commands.md#-parent-action-duration-scope-modifier)
* [```parent add <parent> [action] [duration] [scope] [modifier]```](parrent-commands.md#-parent-action-duration-scope-modifier)
* [```parent remove <parent> [scope]```](parent-commands.md#remove-parent-scope)
* [```parent clear [scope]```](parent-commands.md#clear-scope)
* [```parent list [scope]```](parent-commands.md#list-scope)
* [```parent tree [scope]```](parent-commands.md#tree-scope)
* [```parent show <parent> [scope]```](parent-commands.md#show-parent-scope)
* [```parent check <parent> [scope]```](parent-commands.md#check-parent-scope)

## Meta commands

Sub commands to set meta values to users and groups.

* [```set <key> <value> [duration] [scope]```](meta-commands.md#set-key-value-duration-scope)
* [```unset <key> [scope]```](meta-commands.md#unset-key-scope)
* [```show <key> [scope]```](meta-commands.md#show-key-scope)
* [```clear [scope]```](meta-commands.md#clear-scope)
* [```list [scope]```](meta-commands.md#list-scope)
* [```tree [scope]```](meta-commands.md#tree-scope)
* [```check <key> [scope]```](meta-commands.md#check-key-scope)

## Track commands

These commands are for manging group tracks.

* [```/perms track <name> create```](track-commands.md#perms-track-name-create)
* [```/perms track <name> delete```](track-commands.md#perms-track-name-delete)
* [```/perms track <name> rename <newName>```](track-commands.md#perms-track-name-rename-newname)
* [```/perms track <name> add <group>```](track-commands.md#perms-track-name-add-group)
* [```/perms track <name> insert <group> <position>```](track-commands.md#perms-track-name-insert-group-position)
* [```/perms track <name> remove <group>```](track-commands.md#perms-track-name-remove-group)
* [```/perms track <name> list```](track-commands.md#perms-track-name-list)

## Rank commands

Simplified commands to assign groups / ranks to players. You can permit your staff team to use these commands.

* [```/rank```](rank-commands.md#rank)
* [```/rank <player> list```](rank-commands.md#rank-player-list)
* [```/rank <player> add <group> [action] [duration] [scope] [modifier]```](rank-commands.md#rank-player-add-group-action-duration-scope-modifier)
* [```/rank <player> set <group> [action] [duration] [scope] [modifier]```](rank-commands.md#rank-player-set-group-action-duration-scope-modifier)
* [```/rank <player> remove <group> [scope]```](rank-commands.md#rank-player-remove-group-scope)
* [```/rank <player> promote [track]```](rank-commands.md#rank-player-promote-track)
* [```/rank <player> demote [track]```](rank-commands.md#rank-player-demote-track)


## Additional commands

Additional commands provided by DKPerms.

* ```/team``` Used to list all team members




