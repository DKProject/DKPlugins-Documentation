---
title: General Commands
---

# General Commands

This page describes the usage and permissions of the DKCoins general commands.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/dkcoins```](#dkcoins)
* [```/dkcoins info```](#dkcoins-info)
* [```/dkcoins migrate <system>```](#dkcoins-migrate-system)
* [```/dkcoins admin <player/bank> <action> <amount> [currency]```](#dkcoins-admin-playerbank-action-amount-currency)

***

## **```/dkcoins```**

**Permission:** dkcoins.admin<br />

This is the base command of DKCoins. It is use for administrating the whole DKCoins economy system on your network.
If you don't have access to this command, the plugin version and author is displayed.

***

## **```/dkcoins info```**

**Alias:** information, i, version, v<br/>
Shows information about the current installed plugin, like the version and author.

***

## **```/dkcoins migrate <system>```**

**Permission:** dkcoins.admin<br/>
**Alias:** migration, m<br/>
**Arguments:**

* `<system>` The name of the system to migrate (DKCoinsLegacy, EssentialsX, etc.)

Import coins from another coin system to DKCoins

***

## **```/dkcoins admin <player/bank> <action> <amount> [currency]```**

**Permission:** dkcoins.admin<br/>
**Alias:** bankAdmin<br/>
**Arguments:**

  * `<player/bank>` The player or name of the bank
  * `<action>` The action to perform
  * `<amount>` The amount
  * `[currency]` The name of the currency

Administration commands to manipulate bank and player account balances.

**Available actions:**

* `set` Set the amount to the account
* `add` Add the amount to the account
* `remove` Remove the amount to the account


