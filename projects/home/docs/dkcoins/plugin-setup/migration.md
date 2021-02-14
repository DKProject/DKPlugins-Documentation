---
title: Migration
---

# Migrate to DKCoins

DKCoins supports different migration technologies to migrate another permission system to DKCoins.

***

## **DKCoins V3 Migration**
DKCoins V5 supports a simple migration mechanism to transfer DKCoins V3 data to the new generation.

!!! note ""
    Support for V4 ends on 01.05.2021, we recommend migrating as soon as possible


### **1. - Installation**

!!! warning ""
    Before you start the migration, create a backup of your entire network or server

Before you can start setting up the new DKCoins, you need to remove the old dkcoins.jar in all your plugin folders 
(remove only the jar, do not delete any configuration files). After that you can start setting up the new DKCoins, 
use [this guide](installation.md).

### **1. - Migration**
After DKCoins is successfully installed, you can start with the migration of DKCoins V4.
To start the migration, run the following command in your console:

`./dkcoins migrate DKCoinsLegacy`

As soon as the migration is successfully completed, you can remove all old configuration and message files 
from your plugins folder and restart your entire network.

***

## **Migrate from another plugin**

DKCoins supports different plugins to migrate from. Create a [Suggestion](../support.md#suggestions) if your plugin is missing.


**Supported Migrations:**
 * EssentialsX

### **1. - Installation**

!!! warning ""
    Before you start the migration, create a backup of your entire network or server

If you have decided to switch to DKCoins, you must first install DKCoins on your network, use [this guide](installation.md) to set up DKCoins.

We recommend disabling the old permission system by renaming `.jar` to `.disabled`.

### **1. - Migration**
After DKCoins is successfully installed, you can start migrating your old permissions plugin.
Make sure you re-enable the old system (rename `.disabled` to `.jar`) to start the migration, 
run the following command in your console:

!!! note ""
    During the migration both coin systems (DKCoins and the old one) will be installed, this can 
    cause problems. During the migration you should not connect to your server.

`./dkcoins migrate <plugin-name>`

As soon as the migration is successfully completed, you can remove the old plugin and all configuration and message files
from your plugins folder and restart your entire network.
