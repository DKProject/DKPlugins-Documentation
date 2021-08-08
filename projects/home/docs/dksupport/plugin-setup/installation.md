---
title: Installation
---

# DKSupport Installation

The DKSupport installation is very easy and can be done in a few minutes. Follow these instructions 
exactly and contact our support if you have any questions or problems.

***

## **Compatibility**
DKSupport supports Minecraft 1.8 - 1.17.1 and runs on all McNative supported platforms:

 * Bukkit, Spigot, PaperSpigot, Yatopia, Tunity, Purpur, Airplane
 * BungeeCord, Waterfall, Travertine, FlameCord
 * McNative

DKSupport is designed for running on multiple servers and supports all McNative messaging technologies:

 * BungeeCord Proxy Network (Plugin Message Channels)
 * CloudNet V2 (Multi proxy)
 * CloudNet V3 (Multi proxy)

***

## **Requirements**

DKSupport supports java 8 - 1.17.1 and requires a stable internet connection (DKPerms downloads all necessary libraries dynamically). 
If you are using DKSupport on multiple servers, you also need a supported remote database (MySQL, PostgreSQL, MS-SQL, MongoDB et.c).

***

## **Installation**

### **1. - Get A License**
DKSupport is a paid plugin and before you can start with the setup you have to purchase a license in the [McNative Store](https://mcnative.org/plugins/pretronic/dkmotd). 
See also the DKSupport [license agreement](../license.md).

### **2. - Download**
To install DKSupport, download the latest loader [here](https://downloads.mcnative.org/id/9304d68a-bbdf-11eb-8ba0-0242ac180002) and
move it to your plugins folder. Start your server.

In this setup, we use the simple loader. If you are interested in the template loader to install multiple resources dynamically, 
checkout the [McNative Docs](https://docs.mcnative.org/).

!!! note ""
    If you are using a network with multiple servers, you must usually only install DKSupport on your proxy server.

### **3. - Licensing**
After DKSupport has started you will see an error in your console (`Missing or wrong authentication credentials`). 
To license DKSupport to your server you have to enter your network credentials in the McNative config (You will find the credentials in the McNative console) 
or use your personal license key.

**Key Licensing** <br />
If you want to continue with your personal `license.key` you just have to put it in the folder `plugins/DKSupport`.

**McNative Licensing** <br />
If you want to work with McNative and is capabilities, enter your console credentials (you will find them in the McNative console on the left side) in the McNative configuration (`plugins/McNative/config.yml`).


Restart your server, if everything worked correctly a folder named `DKSupport` should be created in `./plugins`.

### **(4. - Storage setup)**
After the installation you can optionally set up a storage solution like MySQL. Read more about storages [here](storage.md)

!!! note ""
    If you are using a network with multiple servers, you must connect to the same remote database.
