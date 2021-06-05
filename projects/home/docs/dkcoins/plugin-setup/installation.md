---
title: Installation
---

# DKCoins Installation

The DKCoins installation is very easy and can be done in a few minutes. Follow these instructions 
exactly and contact our support if you have any questions or problems.

***

## **Compatibility**
DKCoins supports minecraft 1.8 - 1.16.4 and later and runs on all McNative supported platforms:

* Bukkit, Spigot, PaperSpigot, Yatopia, Tunity, Purpur
* BungeeCord, Waterfall, Travertine, FlameCord
* McNative

DKCoins is designed for running on multiple servers and supports all McNative messaging technologies:

 * BungeeCord Proxy Network (Plugin Message Channels)
 * CloudNet V2 (Multi proxy)
 * CloudNet V3 (Multi proxy)

***

## **Requirements**

DKCoins supports java 8 - 15 and requires a stabl internet connection (DKCoins downloads all necessary libraries dynamically). 
If you are using DKCoins on multiple servers, you also need a supported remote database (MySQL, PostgreSQL, MS-SQL, MongoDB et.c).

***

## **Installation**

### **1. - Download**
To install DKCoins, download the latest loader [here](https://downloads.mcnative.org/id/0249f842-de95-42df-b611-7ad390d90086) and
move it to your plugins folder. Start your server.

In this setup, we use the simple loader. If you are interested in the template loader to install multiple resources dynamically, 
checkout the [McNative Docs](https://docs.mcnative.org/).

!!! note ""
    If you are using a network with multiple servers, you must connect DKCoins to the same remote database.


### **(2  - Storage setup)**
After the installation you can optionally set up a storage solution like MySQL. Read more about storages [here](storage.md)

!!! note ""
    If you are using a network with multiple servers, you must connect to the same remote database.

### **3. - Set coins to your account**

After DKCoins is successfully installed on your network, join with your minecraft account on the server and run the 
following command to set your coin amount (Replace `<player>` with your username).

 * `./dkperms admin <player> set 100000`

