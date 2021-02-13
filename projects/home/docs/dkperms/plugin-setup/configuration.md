---
title: Configuration
---

# Configuration

This page describes all configuration possibilities in the DKPerms config.yml.
**Location:** ``./plugins/DKPerms/config.yml``

#### Index

* [Scope settings](#scope-settings)
* [McNative settings](#mcnative-settings)
* [Object settings](#object-settings)
* [Security settings](#security-settings)
* [Delete timeout settings](#delete-timeout-settings)
* [Format timeout settings](#format-timeout-settings)
* [Commands settings](#commands-settings)

***

## **Scope settings**

DKPerms uses different scopes to separate permission levels. The scopes are arranged hierarchically in a
tree structure and can be configured individually for each server.

* ``namespace`` The namespace where the plugin operates (Usually Minecraft)
* ``current`` Settings for the scope on the current server.
    * ``dynamic`` If this value is `True` the scope will automatically detected on supported networks (e.g. BungeeCord, CloudNet).
    * ``instance`` A custom configured server scope (e.g. CityBuild-1).
    * ``group`` A custom configured server group area (all servers with the same role should have the same group).
* ``serverGroupSplit`` How the server group should be detected by the server name.
* ``worldKey`` Which scope key should be used to separate worlds (`\\World=Plots`).

**Example:**
```
scope: 
  namespace: 'Minecraft'
  current: 
    dynamic: true
    instance: '\ServerGroup=Server\Server=Server-1'
    group: '\ServerGroup=Server'
  serverGroupSplit: '-'
  worldKey: 'World'
```

***

## **McNative settings**

These settings define how the McNative permission api should integrate with DKPerms.

* ``managementScope`` The scopes to be taken by the McNative api
  * ``group`` To which scope the McNative api should check and assign groups
  * ``permission`` To which scope the McNative api should check and assign permission
  * ``operator`` To which scope the McNative api should check and assign operator privileges (When /op is used)

**Example:**
```
mcnative: 
  managementScope: 
    group: '{global}'
    permission: '{currentGroup}'
    operator: '{currentGroup}'
```

***

## **Object settings**

DKPerms uses different objects to store permissions (e.g. group and player). 
With this setting you can change the location of the storage scope.

* ``player`` The player object type
  * ``scope`` The default scope to create and load players
* ``group`` The group object type
  * ``scope`` The default scope to create and load groups
* ``track`` Permission group tracks
  * ``scope`` The default scope to create and load tracks

**Example:**
```
object: 
  player: 
    scope: '\\namespace=minecraft'
  group: 
    scope: '\\namespace=minecraft'
  track: 
    scope: '\\namespace=minecraft'
```

***

## **Security settings**

To keep DKPerms secure

* ``logging`` Change logging
  * ``enabled`` If `True` changes are logged into the database
* ``commands`` DKPerms commands
  * ``enabled`` If `True` commands are enabled (console and chat)
* ``operator`` Default Minecraft operation privileges (When /op is used)
  * ``enabled`` If `True` operators are allowed and /op can be used
* ``restricted`` Command restricted to certain users
  * ``enabled`` If `True` only the configured users can execute DKPerms commands (except /rank)
  * ``users`` The uuid or name of the players in an array that are allowed to execute DKPerms commands.

**Example:**
```
security: 
  logging: 
    enabled: true
  commands: 
    enabled: true
  operator: 
    enabled: false
  restricted: 
    enabled: false
    users: ['Dkrieger','cb7f0812-1fbb-4715-976e-a81e52be4b67']
```

***

## **Delete timeout settings**

To clean your database from expired permissions, groups or properties, DKPerms uses a simple task. 
(Note, if the permission has expired before the task is executed, the permission is already not valid and visible).

* ``deleteTimedOutEntries`` Database cleanup 
  * ``enabled`` If `True` the task will be executed
  * ``interval`` How often to run the task to delete unused entries (Use McNative duration format).

**Example:**
```
deleteTimedOutEntries: 
  enabled: true
  interval: '30m'
```

***

## **Format timeout settings**

Display format options

* ``format`` General formatting settings
  * ``date`` Date formatting settings
    * ``pattern`` Java date time patterns (https://docs.oracle.com/javase/7/docs/api/java/text/SimpleDateFormat.html)
    * ``endlessly`` The symbol used for permanent things

**Example:**
```
format: 
  date: 
    pattern: 'dd-MM-yyyy HH:mm'
    endlessly: '-'
```

***

## **Commands settings**

DKPerms commands settings

* ``command`` General formatting settings
  * ``permission`` The DKPerms admin permission command
    * ``enabled`` If `True` the command is enabled and can be used
    * ``name`` The name of the command
    * ``permission`` The required permission to use this command
    * ``aliases`` Aliases to execute this command
  * ``rank`` The DKPerms simplified rank command
    * ``...``
  * ``team`` The DKPerms team info command
    * ``...``

**Example:**
```
command: 
  permission: 
    enabled: true
    name: 'permissions'
    permission: 'dkperms.admin'
    aliases: ['perms','permission','perm','dkperms']
  rank: 
    enabled: true
    name: 'rank'
    permission: 'dkperms.rank'
    aliases: ['ranks']
  team: 
    enabled: true
    name: 'team'
    permission: 'dkperms.team'
    aliases: []
```
