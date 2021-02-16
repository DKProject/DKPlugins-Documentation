---
title: Currency Commands
---

# Currency Commands

This page describes the usage and permissions of the currency commands. 
The currency command always starts with `/currency <name>`, while `<name>` is the name of the currency.

Important things to remember:
  
* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/currency [list]```](#currency-list)
* [```/currency <name>```](#currency-name)
* [```/currency <name> create <symbol>```](#currency-name-create-symbol)
* [```/currency <name> delete```](#currency-name-delete)
* [```/currency <name> edit name <name>```](#currency-name-edit-name-name)
* [```/currency <name> edit symbol <symbol>```](#currency-name-edit-symbol-symbol)
* [```/currency <name> edit exchangeRate <target> <amount>```](#currency-name-edit-exchangerate-target-amount)
* [```/currency <name> edit exchangeRate <target> disable```](#currency-name-edit-exchangerate-target-disable)

***

## **```/currency [list]```**

**Permission:** dkcoins.command.currency<br />

This is the base currency command. It lists all currencies.

***

## **```/currency <name>```**

**Permission:** dkcoins.command.currency<br />

This is the base command for a specific currency. It shows all information about the currency.
If the currency does not exist, it will be shown in the chat.

***

## **```/currency <name> create <symbol>```**

**Permission:** dkcoins.command.currency<br />
**Arguments:**

* `<symbol>` The symbol of the currency (e.g. $)

This command creates a currency with the specific symbol.

***

## **```/currency <name> delete```**

**Permission:** dkcoins.command.currency<br />

This command deletes a currency.

***

## **```/currency <name> edit name <name>```**

**Permission:** dkcoins.command.currency<br />
**Arguments:**

* `<name>` The new name of the currency

This command renames the currency to the specified name.

***

## **```/currency <name> edit symbol <symbol>```**

**Permission:** dkcoins.command.currency<br />
**Arguments:**

* `<symbol>` The new symbol of the currency

This command changes the symbol of the currency.

***

## **```/currency <name> edit exchangeRate <target> <amount>```**

**Permission:** dkcoins.command.currency<br />
**Arguments:**

* `<target>` The target currency (to exchange)
* `<amount>` The change amount as double, for example 1.2 or 2

This command changes the exchange rate to the specified currency. 
The amount means how much an amount of the currency is in the target currency.

***

## **```/currency <name> edit exchangeRate <target> disable```**

**Permission:** dkcoins.command.currency<br />
**Arguments:**

* `<target>` The target currency (to exchange)

This command disables the exchange into the target currency.
