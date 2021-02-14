---
title: Configuration
---

# Configuration

This page describes all configuration possibilities in the DKCoins config.yml.

**Location:** ``./plugins/DKCoins/config.yml``

#### Index

* [Currency settings](#currency-settings)
* [Date format settings](#date-format-settings)
* [Bank account settings](#bank-account-settings)
* [Economy provider settings](#economy-provider-settings)
* [Payment settings](#payment-settings)
* [Commands settings](#commands-settings)

***

## **Currency settings**

DKCoins currency settings.

* ``default`` The name of the default currency (Make sure that the configured currency exist, otherwise this can cause issues). 
* ``format`` Coin formatting options.
    * ``pattern`` The java number format patterns (https://docs.oracle.com/javase/7/docs/api/java/text/DecimalFormat.html).
    * ``separator`` 
       * ``grouping`` The 1000 delimiter.
       * ``decimal`` The decimal delimiter.

**Example:**
```
currency: 
  default: 'Coins'
  format: 
    pattern: '###,###.##'
    separator: 
      grouping: ''''
      decimal: '.'
```

***

## **Date format settings**

How DKCoins should display date times.

* ``format`` Date formatting options.
  * ``pattern`` Java date time patterns (https://docs.oracle.com/javase/7/docs/api/java/text/SimpleDateFormat.html).

**Example:**
```
date: 
  format: 
    pattern: 'dd-MM-yyyy HH:mm'
```

***

## **Bank account settings**

DKCoins uses different bank accounts to

* ``type`` Account type settings (DKCoins supports the creation of different account types)
    * ``startAmount`` How much money a newly created account should contain (configured per account type)
        * ``<bankType>`` The amount for this type 

* ``user`` Simplified commands to transfer money from users to bank accounts
    * ``creditAliases`` The configured command aliases (Multiple entries in an array can be created)
        * ``<currency>`` The name of the currency to use (Make sure that the configured currency exist, otherwise this can cause issues).
        * ``<permission>`` The required permission to execute the command
        * ``<otherPermission>`` The permission to view coins of other players
        * ``<commands>`` The command aliases
        * ``<disabledWorlds>`` Optionally you can disable this command in certain worlds
* ``payment`` Money transfer settings between bank accounts and users
    * ``minimum`` 
        * ``user`` The minimum required amount to pay to another user or bank account
        * ``all`` The minimum required amount to pay to all other users or bank accounts
    
    **Example:**
```
account: 
  type: 
    startAmount: 
      User: 1000
      Bank: 0
  user: 
    creditAliases: 
      - currency: 'Coins'
        permission: 'dkcoins.command.coins'
        otherPermission: 'dkcoins.command.coins.other'
        commands: ['coins','money']
        disabledWorlds: []
  payment: 
    minimum: 
      user: 0.01
      all: 1.0
```

***

## **Economy provider settings**

With this setting you can configure how DKCoins should hook into third party economy providers (e.g. Vault).

* ``enabled`` If `True` DKCoins will hook into available providers.
* ``priority`` DKCoins will use this priority to hook into the provider.
* ``currency`` The currency used for the operations performed by the provider (Make sure that the configured currency exist, otherwise this can cause issues).

**Example:**
```
economyProvider: 
  enabled: true
  priority: 127
  currency: 'Coins'
```

***

## **Payment settings**

With this setting you can configure how DKCoins should hook into third party economy providers (e.g. Vault).

* ``all`` 
  * ``aliases`` DKCoins will use this priority to hook into the provider.
* ``currency`` The currency used for the operations performed by the provider (Make sure that the configured currency exist, otherwise this can cause issues).

**Example:**
```
payment: 
  all: 
    aliases: ['*']
```
**

## **Commands settings**

DKCoins commands settings

!!! note ""
    You can optionally configure a coin command per currency. See more [here](#bank-account-settings)

* ``top`` Coins top command.
    * ``entriesPerPage`` How many entries should be displayed per page
* ``bank`` The DKCoins bank command
    * ``enabled`` If `True` the command is enabled and can be used.
    * ``name`` The name of the command.
    * ``permission`` The required permission to use this command.
    * ``aliases`` Aliases to execute this command.
* ``currency`` The DKCoins currency command
    * ``...``
* ``pay`` The DKCoins simplified pay command
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
