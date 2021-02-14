---
title: Track Commands
---

# Track Commands

This page describes the usage of DKPerms **track-commands**.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```


#### Index

* [```/perms track <name> create```](#perms-track-name-create)
* [```/perms track <name> delete```](#perms-track-name-delete)
* [```/perms track <name> rename <newName>```](#perms-track-name-rename-newname)
* [```/perms track <name> add <group>```](#perms-track-name-add-group)
* [```/perms track <name> insert <group> <position>```](#perms-track-name-insert-group-position)
* [```/perms track <name> remove <group>```](#perms-track-name-remove-group)
* [```/perms track <name> list```](#perms-track-name-list)

***

## **```/perms track <name> create```**

**Permission:** dkperms.admin<br/>
**Alias:** c <br/>
**Arguments:**

* `<name>` The name of the track to create

This command creates a new permission track to order groups.

***

## **```/perms track <name> delete```**

**Permission:** dkperms.admin<br/>
**Alias:** d <br/>
**Arguments:**

* `<name>` The name of the track

This command deletes an existing track.

***

## **```/perms track <name> rename <newName>```**

**Permission:** dkperms.admin<br/>
**Alias:** re <br/>
**Arguments:**

* `<name>` The name of the track
* `<newName>` The new name of the track

Rename an existing track.

***

## **```/perms track <name> add <group>```**

**Permission:** dkperms.admin<br/>
**Alias:** a <br/>
**Arguments:**

* `<name>` The name of the track
* `<group>` The permission group which should be added to this track

Add a permission group to this track.

## **```/perms track <name> insert <group> <position>```**

**Permission:** dkperms.admin<br/>
**Alias:** i <br/>
**Arguments:**

* `<name>` The name of the track
* `<group>` The permission group which should be inserted to this track
* `<position>` The position where to insert the group

Insert a permission group to this track.

***

## **```/perms track <name> remove <group>```**

**Permission:** dkperms.admin<br/>
**Alias:** r <br/>
**Arguments:**

* `<name>` The name of the track
* `<group>` The permission group to remove from this track
  
Remove a permission group from this track.

***

## **```/perms track <name> list```**

**Permission:** dkperms.admin<br/>
**Alias:** l <br/>
**Arguments:**

* `<name>` The name of the track

List all groups of this track (ordered)
