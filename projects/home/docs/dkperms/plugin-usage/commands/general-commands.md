---
title: General Commands
---

# General Commands

This page describes the usage and permissions of the DKPerms general commands.

Important things to remember:
* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/perms```](#perms)
* [```/perms info```](#perms-info)
* [```/perms sync```](#perms-sync)
* [```/perms migrate```](#perms-migrate-system)
* [```/perms groups```](#perms-groups)
* [```/perms group <group>```](#perms-group-group-)
* [```/perms user <user>```](#perms-user-player-)
* [```/perms track <track>```](#perms-track-track-)
* [```/perms analyse```](#perms-analyse-action)

***

## **```/perms```**

**Permission:** dkperms.admin<br />

This is the base command of DKPerms. It is use for administrating the whole DKPerms permission system on your network.
If you don't have access to this command, the plugin version and author is displayed.

***

## **```/perms info```**

**Permission:** dkperms.admin<br/>
**Alias:** information, i, version, v<br/>
Shows information about the current installed plugin, like the version and author.

***

## **```/perms sync```**

**Permission:** dkperms.admin<br/>
**Alias:** synchronize, s<br/>
Synchronizes permissions, groups, users and metadata a cross multiple server in a network.

***

## **```/perms migrate <system>```**

**Permission:** dkperms.admin<br/>
**Alias:** migration, m<br/>
**Arguments:**
* `<system>` The system to migrate (DKPermsLegacy, PermissionEx etc.)

Imports permissions and groups from other permission systems or older DKPerms versions.
You can find a more detailed explanation [here]().

***

## **```/perms groups```**

**Permission:** dkperms.admin<br/>
Lists all available groups sorted by priority.

***

## **```/perms group <group> ...```**

**Permission:** dkperms.admin<br/>
**Alias:** g<br/>
**Arguments:**
* `<group>` The name of the group
* `...` Optional sub commands, see [Permission Group Commands](Permission-Group-Commands)

Shows information about the targeted group and is used for managing groups.
You can find a more detailed explanation [here](Permission-Group-Commands).

***

## **```/perms user <player> ...```**

**Permission:** dkperms.admin<br/>
**Alias:** u, player, p<br/>
**Arguments:**
* `<player>` The name of the player
* `...` Optional sub commands, see [User Commands](User-Commands)

Shows information about the targeted group and is used for managing players.
You can find a more detailed explanation [here](User-Commands).

***

## **```/perms track <track> ...```**

**Permission:** dkperms.admin<br/>
**Alias:** t<br/>
**Arguments:**
* `<track>` The name of the track
* `...` Optional sub commands, see [Track Commands](Track-Commands)

Shows information about the targeted track and is used for managing tracks.
You can find a more detailed explanation [here](Track-Commands).

***

## **```/perms analyse <action>```**

**Permission:** dkperms.admin<br/>
**Arguments:**
* `<action>` The action to perform

Helps debugging permissions problems on your server

**Available actions:**
* `on` Enables permission analysing and printing
* `off` Disables permission analysing and printing
* `join` Joins the player into the printing listener to receive permission debug prints
* `leave` Removed the player from the printing listener


