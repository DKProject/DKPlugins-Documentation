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

* [```/perms```](general-commands#perms)
* [```/perms info```](general-commands#perms-info)
* [```/perms sync```](general-commands#perms-sync)
* [```/perms migrate```](general-commands#perms-migrate-system)
* [```/perms groups```](general-commands#perms-groups)
* [```/perms group <group>```](general-commands#perms-group-group-)
* [```/perms user <user>```](general-commands#perms-user-player-)
* [```/perms track <track>```](general-commands#perms-track-track-)
* [```/perms analyse```](general-commands#perms-analyse-action)

## User commands
These commands are for manging user permissions, groups and metadata.

```<player> ``` The name or unique id of the player.

* [```/perms user <player> info```](user-commands#perms-user-player-info)
* [```/perms user <player> permission```](user-commands#perms-user-player-permission-)
* [```/perms user <player> meta```](user-commands#perms-user-player-meta-)
* [```/perms user <player> parent```](user-commands#perms-user-player-parent-)

## Group commands
Commands for manging groups. ```<group> ``` is the name of the group.

* [```/perms group <group> info```](group-commands#perms-group-group-create)
* [```/perms group <group> create```](group-commands#perms-group-group-create)
* [```/perms group <group> delete```](group-commands#perms-group-group-delete)
* [```/perms group <group> rename <newname>```](group-commands#perms-group-group-rename-newname)
* [```/perms group <group> copy <newname>```](group-commands#perms-group-group-copy-newname)
* [```/perms group <group> members [scope]```](group-commands#perms-group-group-rename-newname)
* [```/perms group <group> permission```](group-commands#perms-group-group-permission)
* [```/perms group <group> meta```](group-commands#perms-group-group-meta)
* [```/perms group <group> group```](group-commands#perms-group-group-group)
* [```/perms group <group> setPriority <priorit> ```](group-commands#perms-group-group-setpriority-priorit)

## Permission commands
Sub commands to assign permissions to users and groups.

* ```permission list [scope]```
* ```permission tree```
* ```permission show <permission> [scope]```
* ```permission set <permission> [action] [duration] [scope] [modifier]```
* ```permission unset <permission> [scope]```
* ```permission clear [scope]```
* ```permission check <permission> [scope]```


## Parent commands

Sub commands to assign parents (groups) to users and groups.

* [```parent set <parent> [action] [duration] [scope] [modifier]```](parrent-commands#-parent-action-duration-scope-modifier)
* [```parent add <parent> [action] [duration] [scope] [modifier]```](parrent-commands#-parent-action-duration-scope-modifier)
* [```parent remove <parent> [scope]```](parrent-commands#remove-parent-scope)
* [```parent clear [scope]```](parrent-commands#clear-scope)
* [```parent list [scope]```](parrent-commands#list-scope)
* [```parent tree [scope]```](parrent-commands#tree-scope)
* [```parent show <parent> [scope]```](parrent-commands#show-parent-scope)
* [```parent check <parent> [scope]```](parrent-commands#check-parent-scope)

## Meta commands

Sub commands to set meta values to users and groups.

* ```meta list [scope]```
* ```meta tree```
* ```meta show <key> [scope]```
* ```meta set <key> <value> [duration] [scope] ```
* ```meta unset <key> [scope]```
* ```meta clear [scope]```
* ```meta check <key> [scope]```



