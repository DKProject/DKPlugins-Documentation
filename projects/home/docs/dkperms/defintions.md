---
title: Definitions
---

# Definitions

This page describes the key definitions and the structure of DKPerms. It is very important that you understand these things before you start using DKPerms.

## Permissions
Every plugin installed on your server usually brings its own permissions, these permissions are required to
restrict commands and features to different users and groups. These permissions allow you to control which user has access to a command or feature.

The permission node is a sequence of letters and is provided by the respective plugin author.
For example, to ban (`/ban dkrieger hacking`) a user with DKBans the permission `dkbans.ban` is required.

## Meta
The meta is a key value based information that can be set to groups and users.
Unlike permissions, the meta contains a value that can be read by another plugin.

For example, you might want to display a prefix before the player name in the tab list, so
you can set a meta entry with the key `prefix` and your value.


## Groups (Permission groups)
Usually different players have the same permission. In this case DKPerms has groups, which you can give permissions,
metas and other groups, later on you can assign this group to different players.

For example, you can create a ```moderator``` group, which contains permissions for banning, kicking and teleport.
When now a new moderator joins your team, you can easily assign the ```moderator``` group to him/her, and he/she will automatically get necessary permissions.

## Server Groups
A server group is a collection of different servers, every server is automatically in a server group the name of the group
is the first part of the group separator (```-```) defined in the configuration

For example, you have a different SkyWars servers called:
* ```SkyWars-1```
* ```SkyWars-2```
* ```SkyWars-3```

The server group for these servers is called ```SkyWars```, if you now need the same permissions on all skywars servers,
it is much easier to assign the permission to the server group instead to each server.

## Scope

DKPerms is based on a tree structure, everything in DKPerms (Objects, permissions, groups etc.) belongs to a scope and is only valid for this and all subordinate scopes.


This example shows how a tree can look like:

* ```Nemspace=Minecraft```
    * ```ServerGroup=Lobby```
        * ```Server=Lobby-1```
            * ```World=World-1```
        * ```Server=Lobby-2```

If the permission `dkbans.ban` is assigned to a player on the scope `Nemspace=Minecraft\\ServerGroup=Lobby` the permission is valid on `Lobby-1` and `Lobby-2`.

## Permission Object

A PermissionObject holds permission data and can be a group, user or a custom type. Objects are registered in DKPerms and assigned to a third-party resource.
