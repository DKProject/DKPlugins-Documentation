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

* [```/perms```](General-Commands#perms)
* [```/perms info```](General-Commands#perms-info)
* [```/perms sync```](General-Commands#perms-sync)
* [```/perms migrate```](General-Commands#perms-migrate-system)
* [```/perms groups```](General-Commands#perms-groups)
* [```/perms group <group>```](General-Commands#perms-group-group-)
* [```/perms user <user>```](General-Commands#perms-user-player-)
* [```/perms track <track>```](General-Commands#perms-track-track-)
* [```/perms analyse```](General-Commands#perms-analyse-action)

## User commands
These commands are for manging user permissions, groups and metadata.

```<player> ``` The name or unique id of the player.

* [```/perms user <player> info```](User-Commands#perms-user-player-info)
* [```/perms user <player> permission```](User-Commands#perms-user-player-permission-)
* [```/perms user <player> meta```](User-Commands#perms-user-player-meta-)
* [```/perms user <player> parent```](User-Commands#perms-user-player-parent-)

## Group commands
Commands for manging groups. ```<group> ``` is the name of the group.

* ```/perms group <group> info```
* ```/perms group <group> create```
* ```/perms group <group> delete```
* ```/perms group <group> rename <newName>```
* ```/perms group <group> copy <newName>```
* ```/perms group <group> members [scope] [page]```
* ```/perms group <group> permission```
* ```/perms group <group> meta```
* ```/perms group <group> group ```
* ```/perms group <group> setPriority <priorit> ```

## Permission commands


* ```permission list [scope]```
* ```permission tree```
* ```permission show <permission> [scope]```
* ```permission set <permission> [action] [duration] [scope] [modifier]```
* ```permission unset <permission> [scope]```
* ```permission clear [scope]```
* ```permission check <permission> [scope]```

## Meta commands

* ```meta list [scope]```
* ```meta tree```
* ```meta show <key> [scope]```
* ```meta set <key> <value> [duration] [scope] ```
* ```meta unset <key> [scope]```
* ```meta clear [scope]```
* ```meta check <key> [scope]```

#### Group / Parent commands

* ```group list [scope]```
* ```group tree```
* ```group show <group> [scope]```
* ```group set <group> [action] [duration] [scope] [modifier]```
* ```group add <group> [action] [duration] [scope] [modifier]```
* ```group remove <group> [scope]```
* ```group clear [scope]```
* ```group check <key> [scope]```



