---
title: Installation
---

# DKConnect Installation

The DKConnect installation is very easy and can be done in a few minutes. Follow these instructions 
exactly and contact our support if you have any questions or problems.

***

## **Compatibility**
DKConnect supports Minecraft 1.8 - 1.18.1 and runs on all McNative supported platforms:

 * Bukkit, Spigot, PaperSpigot, Yatopia, Tunity, Purpur, Airplane
 * BungeeCord, Waterfall, Travertine, FlameCord
 * McNative

DKConnect is designed for running on multiple servers and supports all McNative messaging technologies:

 * BungeeCord Proxy Network (Plugin Message Channels)
 * CloudNet V2 (Multi proxy)
 * CloudNet V3 (Multi proxy)

DKConnect only support official Minecraft versions published by Mojang. Cracked (offline mode) is not supported.

***

## **Requirements**

DKConnect supports java 8 - 1.18.1 and requires a stable internet connection (DKConnect downloads all necessary libraries dynamically). 
If you are using DKConnect on multiple servers, you also need a supported remote database (MySQL, PostgreSQL, MS-SQL, MongoDB et.c).

***

## **Installation**

### **1. - Get A License**
DKConnect is a paid plugin and before you can start with the setup you have to purchase a license in the [McNative Store](https://mcnative.org/plugins/pretronic/dkconnect). 
See also the DKConnect [license agreement](../license.md).

### **2. - Download**
To install DKConnect, download the latest loader [here](https://downloads.mcnative.org/id/1e6d4f31-e2e0-11eb-8ba0-0242ac180002) and
move it to your plugins folder. Start your server.

In this setup, we use the simple loader. If you are interested in the template loader to install multiple resources dynamically, 
checkout the [McNative Docs](https://docs.mcnative.org/).

!!! note ""
    If you are using a network with multiple servers, you must usually only install DKConnect on your proxy server.

### **3. - Licensing**
After DKConnect has started you will see an error in your console (`Missing or wrong authentication credentials`). 
To license DKConnect to your server you have to enter your network credentials in the McNative config (You will find the credentials in the McNative console) 
or use your personal license key.

**Key Licensing** <br />
If you want to continue with your personal `license.key` you just have to put it in the folder `plugins/DKConnect`.

**McNative Licensing** <br />
If you want to work with McNative and is capabilities, enter your console credentials (you will find them in the McNative console on the left side) in the McNative configuration (`plugins/McNative/config.yml`).


Restart your server, if everything worked correctly a folder named `DKConnect` should be created in `./plugins`.

### **(4. - Storage setup)**
After the installation you can optionally set up a storage solution like MySQL. Read more about storages [here](storage.md)

!!! note ""
    If you are using a network with multiple servers, you must connect to the same remote database.

### **5. - Setup the Discord guild**

@Todo

