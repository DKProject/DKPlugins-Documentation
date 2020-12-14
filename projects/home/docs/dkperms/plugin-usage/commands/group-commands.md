---
title: Group Commands
---

# Group Commands

This page describes the usage of DKPerms group commands. The group command always starts with `/perms group <group>`, while `<group>` is the name of the group.

Important things to remember:
* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```


#### Index

* [```/perms group <group> info```](#perms-group-group-create)
* [```/perms group <group> create```](#perms-group-group-create)
* [```/perms group <group> delete```](#perms-group-group-delete)
* [```/perms group <group> rename <newname>```](#perms-group-group-rename-newname)
* [```/perms group <group> copy <newname>```](#perms-group-group-copy-newname)
* [```/perms group <group> members [scope]```](#perms-group-group-rename-newname)
* [```/perms group <group> permission```](#perms-group-group-permission)
* [```/perms group <group> meta```](#perms-group-group-meta)
* [```/perms group <group> group```](#perms-group-group-group)
* [```/perms group <group> setPriority <priorit>```](#perms-group-group-setpriority-priorit)

***

## **```/perms group <group> info```**

**Permission:** dkperms.admin<br/>
**Alias:** i<br/>

Shows information about the group and its primary parent groups.

***

## **```/perms group <group> create```**

**Permission:** dkperms.admin<br/>
**Alias:** c <br/>

This command creates a new permission group that can be assigned to users or other groups.

***

## **```/perms group <group> delete```**

**Permission:** dkperms.admin<br/>
**Alias:** d <br/>

This command deletes an existing permission group, all players will be removed.

***
## **```/perms group <group> rename <newname>```**

**Permission:** dkperms.admin<br/>
**Alias:** d <br/>
**Arguments:**

* `<newname>` The new name of the group

This command renames an existing permission group.

***

## **```/perms group <group> copy <newname>```**

**Permission:** dkperms.admin<br/>
**Alias:** clone, c <br/>
**Arguments:**

* `<newname>` The name for the new group

This command copies an existing group and all its permissions, parent groups and metas.

***

## **```/perms group <group> members [scope]```**

**Permission:** dkperms.admin<br/>
**Alias:** n, list, players<br/>
**Arguments:**

* `[scope]` The scope to which the group should be assigned (by default, the namespace minecraft is used).

Lists all members of this group

***

## **```/perms group <group> setPriority <priorit>```**

**Permission:** dkperms.admin<br />
**Alias:** priority, p<br/>
**Arguments:**

* `<priorit>` The priority to set (1 = Highest priority)

Set the main priority of your hierarchy structure to this group.

***

## **```/perms group <group> permission```**

**Permission:** dkperms.admin<br/>
**Alias:** permissions, perm, perms, p<br/>
**Arguments:**

* `...` Sub commands, see [Permission Commands](Permission-Commands)

With this command you can add, delete, change or list permissions of a group.
You can find a more detailed explanation [here](Permission-Commands).
***

## **```/perms group <group> meta```**

**Permission:** dkperms.admin<br />
**Alias:** m, properties<br/>
**Arguments:**

* `...` Sub commands, see [Meta Commands](Meta-Commands)

With this command you can add, delete, change or list metadata of a group.
You can find a more detailed explanation [here](Meta-Commands).
***

## **```/perms group <group> group```**

**Permission:** dkperms.admin<br />
**Alias:** group, g<br/>
**Arguments:**

* `...` Sub commands, see [Parent Commands](Parent-Commands)

With this command you can set, add, delete or list inherited groups (parents) of a group.
You can find a more detailed explanation [here](Parent-Commands).

