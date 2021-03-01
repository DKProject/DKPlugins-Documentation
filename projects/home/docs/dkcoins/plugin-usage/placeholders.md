---
title: Placeholders
---

# Placeholders

DKCoins offers many placeholders which can be used in other plugins to display data provided by DKCoins.
DKCoins placeholders are available in all McNative supported placeholder sources (PlaceholderAPI).

Important things to remember:
* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

***

## %dkcoins_balance_[currency]%

This placeholder shows the balance of the player bank account for the specified currency. If the `currency` is not 
given, the default currency will be used.

***

## %dkcoins_player_&lt;player&gt;_balance_[currency]%

This placeholder shows the balance of the specified player bank account for the specified currency. 
If the `currency` is not given, the default currency will be used.

***

## %dkcoins_top_&lt;rank&gt;_name_[currency]%

This placeholder shows the name of the bank account at the specified ``rank`` position.
If the `currency` is not given, the default currency will be used.

***

## %dkcoins_top_&lt;rank&gt;_balance_[currency]%

This placeholder shows the balance of the bank account at the specified ``rank`` position.
If the `currency` is not given, the default currency will be used.

***

## %dkcoins_toppos_[currency]%

This placeholder shows the rank position of the player bank account in the specified ``currency``.
If the `currency` is not given, the default currency will be used.

***

## %dkcoins_bank_&lt;bank&gt;_balance_[currency]%

This placeholder shows the balance of the specified ``bank`` account for the specified currency.
If the `currency` is not given, the default currency will be used.

***
