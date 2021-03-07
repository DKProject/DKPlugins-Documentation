---
title: Commands
---

# Commands

This page describes all available commands to operate DKCoins from the player chat and console.

Important things to remember about commands:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```
* Sub commands documented on another page are declared with ```...```

## General commands
These commands are used to operate DKCoins on your network or server.

* [```/dkcoins```](general-commands.md##dkcoins)
* [```/dkcoins info```](general-commands.md#dkcoins-info)
* [```/dkcoins migrate <system>```](general-commands.md#dkcoins-migrate-system)
* [```/dkcoins admin <player/bank> <action> <amount> [currency]```](general-commands.md#dkcoins-admin-playerbank-action-amount-currency)



## Currency commands
These commands are used to manage different currencies in DKCoins and set exchange rates.

* [```/currency [list]```](currency-commands.md#currency-list)
* [```/currency <name>```](currency-commands.md#currency-name)
* [```/currency <name> create <symbol>```](currency-commands.md#currency-name-create-symbol)
* [```/currency <name> delete```](currency-commands.md#currency-name-delete)
* [```/currency <name> edit name <name>```](currency-commands.md#currency-name-edit-name-name)
* [```/currency <name> edit symbol <symbol>```](currency-commands.md#currency-name-edit-symbol-symbol)
* [```/currency <name> edit exchangeRate <target> <amount>```](currency-commands.md#currency-name-edit-exchangerate-target-amount)
* [```/currency <name> edit exchangeRate <target> disable```](currency-commands.md#currency-name-edit-exchangerate-target-disable)

## Bank commands
These commands are used to manage all bank accounts in DKCoins

* [```/bank [list]```](bank-commands.md#bank-list)
* [```/bank <name>```](bank-commands.md#bank-name)
* [```/bank <name> create <accountType>```](bank-commands.md#bank-name-create-accounttype)
* [```/bank <name> delete```](bank-commands.md#bank-name-delete)
* [```/bank <name> settings <setting> <value>```](bank-commands.md#bank-name-settings-setting-value)
* [```/bank <name> transfer <receiver> <amount> [currency]```](bank-commands.md#bank-name-transfer-receiver-amount-currency)
* [```/bank <name> exchange <source> <target> <amount>```](bank-commands.md#bank-name-exchange-source-target-amount)
* [```/bank <name> member```](bank-commands.md#bank-name-member)
* [```/bank <name> role```](bank-commands.md#bank-name-role-role)
* [```/bank <name> limit```](bank-commands.md#bank-name-limit)
* [```/bank <name> statement```](bank-commands.md#bank-name-statement)

## Bank limit commands
These commands are used for managing the limitation for roles, bank and users for a specified bank.

* [```[list]```](bank-limit-commands.md#list)
* [```set <interval> <amount> <calculationType> <currency>```](bank-limit-commands.md#set-interval-amount-calculationtype-currency)
* [```remove <interval> <amount> <calculationType> <currency>```](bank-limit-commands.md#remove-interval-amount-calculationtype-currency)

## Bank member commands
These commands are used for managing the members for a specified bank. It can not be used on user accounts.

* [```[list]```](bank-member-commands.md#list)
* [```<member> [info]```](bank-member-commands.md#member-info)
* [```<member> add```](bank-member-commands.md#member-add)
* [```<member> remove```](bank-member-commands.md#member-remove)
* [```<member> role <role>```](bank-member-commands.md#member-role-role)
* [```<member> limit```](bank-member-commands.md#member-limit)

## Bank role commands
These commands are used for controlling a specified role in a specified bank.

* [```limit```](bank-role-commands.md#limit)

## User bank commands
These commands are used for simplifier controlling the user bank account with the specified currency.

* [```/<command>```](user-bank-commands.md#command)
* [```/<command> <target>```](user-bank-commands.md#command-target)
* [```/<command> transfer <receiver> <amount>```](user-bank-commands.md#command-transfer-receiver-amount)
* [```/<command> top [page]```](user-bank-commands.md#command-top-page)