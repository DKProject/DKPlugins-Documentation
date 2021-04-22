---
title: Broadcast Group Commands
---

# Broadcast Commands

This page describes the usage and permissions of the DKBans broadcast group commands.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/broadcastgroup <name> create <interval>```](#broadcastgroup-name-create-interval)
* [```/broadcastgroup <name> assignment <broadcast> add```](#broadcastgroup-name-assignment-broadcast-add)
* [```/broadcastgroup <name> assignment <broadcast> remove```](#broadcastgroup-name-assignment-broadcast-remove)
* [```/broadcastgroup <name> assignment list```](#broadcastgroup-name-assignment-list)
* [```/broadcastgroup <name> assignment <broadcast> [info]```](#broadcastgroup-name-assignment-broadcast-info)
* [```/broadcastgroup <name> edit <action> <value>```](#broadcastgroup-name-edit-action-value)
* [```/broadcastgroup <name> list```](#broadcastgroup-name-list)

***

## **```/broadcastgroup <name> create <interval>```**

**Permission:** dkbans.command.broadcast.group<br />
**Arguments:**
* `<name>` The name of the broadcast group
* `<interval>` The interval for the group

This command creates a new broadcast group, which will broadcast all assigned broadcasts in the specified interval.

***

## **```/broadcastgroup <name> assignment <broadcast> add```**

**Permission:** dkbans.command.broadcast.group<br />
**Arguments:**
* `<name>` The name of the broadcast group
* `<broadcast>` The broadcast to asign

This command assigns the broadcast with the name ``<broadcast>`` to this broadcast group.

***

## **```/broadcastgroup <name> assignment <broadcast> remove```**

**Permission:** dkbans.command.broadcast.group<br />
**Arguments:**
* `<name>` The name of the broadcast group
* `<broadcast>` The broadcast to asign

This command remove the assignment of the broadcast with the name ``<broadcast>`` of this broadcast group.

***

## **```/broadcastgroup <name> assignment list```**

**Permission:** dkbans.command.broadcast.group<br />
**Arguments:**
* `<name>` The name of the broadcast group

This command lists all assigned broadcasts of this broadcast group.

***

## **```/broadcastgroup <name> assignment <broadcast> [info]```**

**Permission:** dkbans.command.broadcast.group<br />
**Arguments:**
* `<name>` The name of the broadcast group
* `<broadcast>` The broadcast to asign

This command displays information about the broadcast assignment

***

## **```/broadcastgroup <name> edit <action> <value>```**

**Permission:** dkbans.command.broadcast.group<br />
**Arguments:**
* `<name>` The name of the broadcast group
* `<action>` The edit action to perform
* `<value>` The new value

This command edits the group settings.

Action with value:
- name <name>
- enabled <true, false>
- permission <permission>
- order <order>
- interval <interval>
- scope <type:name:[id]>

***

## **```/broadcastgroup <name> list```**

**Permission:** dkbans.command.broadcast.group<br />
**Arguments:**
* `<name>` The name of the broadcast group

This command lists all broadcast groups.

***