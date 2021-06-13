---
title: Installation
---

# DKPerms Installation

The DKPerms installation is very easy and can be done in a few minutes. Follow these instructions 
exactly and contact our support if you have any questions or problems.

***

## **Compatibility**
DKPerms supports minecraft 1.8 - 1.17 and runs on all McNative supported platforms:

 * Bukkit, Spigot, PaperSpigot, Yatopia, Tunity, Purpur
 * BungeeCord, Waterfall, Travertine, FlameCord
 * McNative

DKPerms is designed for running on multiple servers and supports all McNative messaging technologies:

 * BungeeCord Proxy Network (Plugin Message Channels)
 * CloudNet V2 (Multi proxy)
 * CloudNet V3 (Multi proxy)

***

## **Requirements**

DKPerms supports java 8 - 16 and requires a stabl internet connection (DKPerms downloads all necessary libraries dynamically). 
If you are using DKPerms on multiple servers, you also need a supported remote database (MySQL, PostgreSQL, MS-SQL, MongoDB et.c).

***

## **Installation**

### **1. - Get A License**
DKPerms is a paid plugin and before you can start with the setup you have to purchase a license in the [McNative Store](https://mcnative.org/plugins/pretronic/dkperms). 
See also the DKPerms [license agreement](../license.md).

!!! note ""
    If you are a buyer of DKPermsV1 on SpigotMc, you can get a free 6-month license until If you are a buyer of DKPermsV1 
    on SpigotMc, you can get a free 6-month license until **2021-05-01**. To get your license, contact DKPerms via SpigotMc conversation.

### **2. - Download**
To install DKPerms, download the latest loader [here](https://downloads.mcnative.org/id/19303be6-0b2d-11eb-9f43-0242ac180002) and
move it to your plugins folder. Start your server.

In this setup, we use the simple loader. If you are interested in the template loader to install multiple resources dynamically, 
checkout the [McNative Docs](https://docs.mcnative.org/).

!!! note ""
    If you are using a network with multiple servers, you must install DKPerms on all servers and connect to the same remote database.

### **3. - Licensing**
After DKPerms has started you will see an error in your console (`Missing or wrong authentication credentials`). 
To license DKPerms to your server you have to enter your network credentials in the McNative config (You will find the credentials in the McNative console) 
or use your personal license key.

**Key Licensing (SpigotMc)** <br />
If you want to continue with your personal `license.key` you just have to put it in the folder `plugins/DKPerms`.

**McNative Licensing** <br />
If you want to work with McNative and is capabilities, enter your console credentials in the Mcnative configuration (`plugins/McNative/config.yml`).


Restart your server, if everything worked correctly a folder named `DKPerms` should be created in `./plugins`.

### **(4. - Storage setup)**
After the installation you can optionally set up a storage solution like MySQL. Read more about storages [here](storage.md)

!!! note ""
    If you are using a network with multiple servers, you must connect to the same remote database.

### **5. - Grant administrator rights to your account**

After DKPerms is successfully installed on your network, join with your minecraft account on the server and open the console 
window then run the following command (Replace `<player>` with your username).

 * `./perms user <player> permission add *`

