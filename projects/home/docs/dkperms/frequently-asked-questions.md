---
title: Frequently Asked Questions
---

# Frequently Asked Questions

this page contains some questions which are frequently asked about DKPerms.
Before you ask a question in our support, please check this page and make sure that the question is not already answered.

#### Index

* [How can I create a default group?](#how-can-i-create-a-default-group)
* [How can I use the Tablist and Chat?](#how-can-i-use-the-tablist-and-chat)
* [Why do I not have permission on BungeeCord?](#why-do-i-not-have-permission-on-bungeecord)
* [Why do I not have permission on Spigot?](#why-do-i-not-have-permission-on-spigot)

***
## How can I create a default group?
DKPerms handles default groups in its meta. You can set a group as default on the whole network or on a specified server.

If you set the meta ```default``` to ```true``` of a group, all players will automatically gets all permissions
of the group, but the group is not directly assigned to the player. If you want set a group to each player when he
joined the server, you can set the meta ``defaultAssign``` to ```true```, so every new player automatically receives this group.

**Examples**

```/perms group <group> meta set default true```

```/perms group <group> meta set defaultAsign true```

```/perms group <group> meta set default true world=world-1```
In this case the group is only default on world-1

***
## How can I use the Tablist and Chat?
The Tablist/Chat is provided by McNative and must be enabled in the McNative configuration `plugins/McNative/config.yml`. DKPerms will then
provide all colors and information to McNative.

***
## Why do I not have permissions on BungeeCord?
DKPerms must be installed on all servers and your proxy (BungeeCord). In order that DKPerms can correctly synchronize the permission, make sure that DKPerms
is connected to the same database on all servers and `bungeecord` is set to `true` in the `spigot.yml`.

***
## Why do I not have permissions on Spigot?
DKPerms must be installed on all servers and your proxy (BungeeCord). In order that DKPerms can correctly synchronize the permission, make sure that DKPerms
is connected to the same database on all servers and `bungeecord` is set to `true` in the `spigot.yml`.


