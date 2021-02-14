---
title: Bank Commands
---

# Bank Commands

This page describes the usage and permissions of the Bank commands. The bank command always 
starts with `/bank <name>`, while `<name>` is the name of the bank.

Important things to remember:
* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/bank [list]```](#bank-list)
* [```/bank <name>```](#bank-name)
* [```/bank <name> create <accountType>```](#bank-name-create-accounttype)
* [```/bank <name> delete```](#bank-name-delete)
* [```/bank <name> settings <setting> <value>```](#bank)
* [```/bank <name> transfer <receiver> <amount> [currency]```](#bank)
* [```/bank <name> exchange <source> <target> <amount>```](#bank)
* [```/bank <name> member [list]```](#bank)
* [```/bank <name> member <member> [info]```](#bank)
* [```/bank <name> member <member> add```](#bank)
* [```/bank <name> member <member> remove```](#bank)
* [```/bank <name> member <member> role```](#bank)
* [```/bank <name> member <member> limit```](#bank)
* [```/bank <name> role limit```](#bank)
* [```/bank <name> limit```](#bank)
* [```/bank <name> statement```](#bank)
***

## **```/bank [list]```**

**Permission:** dkcoins.command.bank<br />

This is the base bank command. It lists all your bank accounts.

***

## **```/bank <name>```**

**Permission:** dkcoins.command.bank<br />

This is the base command for a specific bank. It shows you all your account credits with the certain amount.
If the bank does not exist, it will be shown in the chat. 

***

## **```/bank <name> create <accountType>```**

**Permission:** dkcoins.command.bank<br />
**Arguments:**

* `<accountType>` The account type

This command creates a bank with the specific name and account type.
Default there are two account types, `bank` and `user`, but a user account can't be created manually.

***

## **```/bank <name> delete```**

**Permission:** dkcoins.command.bank<br />

This command deletes a bank of you. You need to be the owner of the specified bank.

***

## **```/bank <name> settings <setting> <value>```**

**Permission:** dkcoins.command.bank<br />
**Arguments:**

* `<setting>` The setting type
* `<value>` The value to be changed

This command changes settings of a bank.

Settings:
* receivenotifications, boolean value

***

## **```/bank <name> transfer <receiver> <amount> [currency]```**

**Permission:** dkcoins.command.bank<br />
**Arguments:**

* `<receiver>` The receiver bank
* `<amount>` The amount to be transferred
* `[currency]` currency to be transferred, if not given the default currency will be chosen

This command transfer money from a bank to another bank in a specified currency. If the sender bank does not have enough
money of the currency, it will not be work.

***

## **```/bank <name> exchange <source> <target> <amount>```**

**Permission:** dkcoins.command.bank<br />
**Arguments:**

* `<source>` The source currency
* `<target>` The target currency
* `<amount>` The amount to be transferred

This command exchanges a specified amount of money from a currency to another specified currency.

***

## **```/bank <name> member```**

**Permission:** dkcoins.command.bank<br />

This command controls the member management of the bank.

***

## **```/bank <name> limit```**

**Permission:** dkcoins.command.bank<br />

This command controls all global bank limits of the bank.

***

## **```/bank <name> statement```**

**Permission:** dkcoins.command.bank<br />

This command shows you all your bank transfers and exchanges.

***
