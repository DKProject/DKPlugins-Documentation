---
title: User Commands
---

# User Commands

This page describes the usage of DKPerms user commands. The user command always starts with `/perms user <player>`, while `<player>` is the name of the player.

Important things to remember:
* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/perms user <player> info```](#perms-user-player-info)
* [```/perms user <player> permission```](#perms-user-player-permission-)
* [```/perms user <player> meta```](#perms-user-player-meta-)
* [```/perms user <player> parent```](#perms-user-player-parent-)

***

## **```/perms user <player> info```**

**Permission:** dkperms.admin<br/>
**Alias:** i<br/>

Shows information about the player and his primary groups.

***

## **```/perms user <player> permission ...```**

**Permission:** dkperms.admin<br/>
**Alias:** permissions, perm, perms, p<br/>
**Arguments:**
* `...` Sub commands, see [Permission Commands](Permission-Commands)

With this command you can add, delete, change or list permissions of a player.
You can find a more detailed explanation [here](Permission-Commands).

***

## **```/perms user <player> meta ...```**

**Permission:** dkperms.admin<br />
**Alias:** m<br/>
**Arguments:**
* `...` Sub commands, see [Meta Commands](Meta-Commands)

With this command you can add, delete, change or list metadata of a player.
You can find a more detailed explanation [here](Meta-Commands).

***

## **```/perms user <player> parent ...```**

**Permission:** dkperms.admin<br />
**Alias:** p, group, g<br/>
**Arguments:**
* `...` Sub commands, see [Parent Commands](Parent-Commands)

With this command you can set, add, delete or list inherited groups (parents) of a player.
You can find a more detailed explanation [here](Parent-Commands).
