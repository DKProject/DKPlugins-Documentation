---
title: Migration
---

# Migrate to DKBans

DKBans supports different migration technologies to migrate another punishment system to DKBans.

***

## **DKBans V2 Migration**
DKBans V5 supports a simple migration mechanism to transfer DKBans V2 data to the new generation.

!!! note ""
    Support for V2 ends on 01.05.2021, we recommend migrating as soon as possible


### **1. - Installation**

!!! warning ""
    Before you start the migration, create a backup of your entire network or server

Before you can start setting up the new DKBans, you need to remove the old dkbans.jar in all your plugin folders 
(remove only the jar, do not delete any configuration files). After that you can start setting up the new DKBans, 
use [this guide](installation.md).

### **1. - Migration**
After DKBans is successfully installed, you can start with the migration of DKBans V2.
To start the migration, run the following command in your console:

`./dkbans migrate DKBansLegacy`

As soon as the migration is successfully completed, you can remove all old configuration and message files 
from your plugins folder and restart your entire network.

***

## **Migrate from another plugin**

DKBans supports different plugins to migrate from. Create a [Suggestion](../support.md#suggestions) if your plugin is missing.


**Supported Migrations:**
 * Implementation in progress

### **1. - Installation**

!!! warning ""
    Before you start the migration, create a backup of your entire network or server

If you have decided to switch to DKBans, you must first install DKBans on your network, use [this guide](installation.md) to set up DKBans.

We recommend disabling the old punishment system by renaming `.jar` to `.disabled`.

### **1. - Migration**
After DKBans is successfully installed, you can start migrating your old punishment plugin.
Make sure you re-enable the old system (rename `.disabled` to `.jar`) to start the migration, 
run the following command in your console:

!!! note ""
    During the migration both punishment systems (DKBans and the old one) will be installed, this can 
    cause problems. During the migration you should not connect to your server.

`./dkbans migrate <plugin-name>`

As soon as the migration is successfully completed, you can remove the old plugin and all configuration and message files
from your plugins folder and restart your entire network.
