---
title: Configuration
---

# Configuration

This page describes all configuration possibilities in the DKBans config.yml.

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
