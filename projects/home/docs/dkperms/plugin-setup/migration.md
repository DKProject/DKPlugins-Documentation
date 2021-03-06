---
title: Migration
---

# Migrate to DKPerms

DKPerms supports different migration technologies to migrate another permission system to DKPerms.

***

## **DKPerms V1 Migration**
DKPerms V5 supports a simple migration mechanism to transfer DKPerms V1 data to the new generation.

!!! note ""
    Support for V1 ends on 01.05.2021, we recommend migrating as soon as possible


### **1. - Installation**

!!! warning ""
    Before you start the migration, create a backup of your entire network or server

Before you can start setting up the new DKPerms, you need to remove the old dkperms.jar in all your plugin folders 
(remove only the jar, do not delete any configuration files). After that you can start setting up the new DKPerms, 
use [this guide](installation.md).

### **1. - Migration**
After DKPerms is successfully installed, you can start with the migration of DKPerms V1.
To start the migration, run the following command in your console:

`./dkperms migrate DKPermsLegacy`

As soon as the migration is successfully completed, you can remove all old configuration and message files 
from your plugins folder and restart your entire network.

***

## **Migrate from another plugin**

DKPerms supports different plugins to migrate from. Create a [Suggestion](../support.md#suggestions) if your plugin is missing.


**Supported Migrations:**
 * PermissionEx
 * LuckPerms
 * CloudNet V2 perms
 * CloudNet V3 perms

### **1. - Installation**

!!! warning ""
    Before you start the migration, create a backup of your entire network or server

If you have decided to switch to DKPerms, you must first install DKPerms on your network, use [this guide](installation.md) to set up DKPerms.

We recommend disabling the old permission system by renaming `.jar` to `.disabled`.

### **1. - Migration**
After DKPerms is successfully installed, you can start migrating your old permissions plugin.
Make sure you re-enable the old system (rename `.disabled` to `.jar`) to start the migration, 
run the following command in your console:

!!! note ""
    During the migration both permission systems (DKPerms and the old one) will be installed, this can 
    cause problems. During the migration you should not connect to your server.

`./dkperms migrate <plugin-name>`

As soon as the migration is successfully completed, you can remove the old plugin and all configuration and message files
from your plugins folder and restart your entire network.
