---
title: Bank member Commands
---

# Bank Limit Commands

This page describes the usage of DKCoins **limit-commands**. Those commands are sub commands of [user](bank-commands.md),
[group](bank-member-commands.md) and [role](bank-role-commands.md) commands.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```[list]```](#list)
* [```set <interval> <amount> <calculationType> <currency>```](#set-interval-amount-calculationtype-currency)
* [```remove <interval> <amount> <calculationType> <currency>```](#bank)

***

## **```[list]```**

**Permission:** dkcoins.command.bank<br/>

This command lists all limitations for the specific target.

***

## **```set <interval> <amount> <calculationType> <currency>```**

**Permission:** dkcoins.command.bank<br/>
**Arguments:**
* `interval` the specific interval (DAILY, WEEKLY, MONTHLY)
* `amount` the amount to limit as decimal number
* `calculationType` the calculation type(GLOBAL, USER_BASED)
* `currency` the currency to limit

This command set a limit for specified target for the specified parameters.

***

## **```remove <interval> <amount> <calculationType> <currency>```**

**Permission:** dkcoins.command.bank<br/>
**Arguments:**
* `interval` the specific interval (DAILY, WEEKLY, MONTHLY)
* `amount` the amount to limit as decimal number
* `calculationType` the calculation type(GLOBAL, USER_BASED)
* `currency` the currency to limit

This command removes a limit for specified target for the specified parameters.

***