---
title: Configuration
---

# Configuration

This page describes all configuration possibilities in the DKBans config.yml.

**Location:** ``./plugins/DKCoins/config.yml``

#### Index

* [Date format settings](#date-format-settings)
* [Player settings](#player-settings)
* [Chat settings](#chat-settings)
* [Joinme settings](#joinme-settings)
* [Ip address settings](#ip-address-settings)

***

## **Date format settings**

Display format settings.

* ``format`` General formatting settings.
    * ``date`` Date formatting settings.
        * ``pattern`` Java date time patterns (https://docs.oracle.com/javase/7/docs/api/java/text/SimpleDateFormat.html).
        * ``endlessly`` The symbol used for permanent things.

**Example:**
```
format: 
  date: 
    pattern: 'dd-MM-yyyy HH:mm'
    endlessly: '-'
```

***

## **Player settings**

DKBans player settings.

* ``onJoin`` Settings when a player joins the server.
    * ``clearChat`` If `True` the chat of the player will be cleared.
        * ``info`` Player login information messages
          * ``teamChat`` If `True` the team chat login status will be showed to the player (if he has permission).
          * ``punishNotify`` If `True` the notification login status will be showed to the player (if he has permission).
          * ``report`` If `True` the report login status will be showed to the player (if he has permission).
           * ``listReports`` If `True` the amount of open reports will be showed to the player.
  * ``session`` If `True` the chat of the player will be cleared.
    * ``logging`` If `True` player login sessions are recorded.
    * ``retention`` The duration. how long logging sessions are kept (be careful with this value, it can significantly increase the amount of data).

**Example:**
```
player: 
  onJoin: 
    clearChat: true
    info: 
      teamChat: true
      punishNotify: true
      report: true
    listReports: true
  session: 
    logging: true
    retention: '180d'
```

## **Chat settings**

Chat settings.

* ``filter`` Chat filter options.
    * ``enabled`` If `True` chat filters are enabled and will block certain messages (As configured with ./filter).
    * ``repeatDelay`` How fast players can send messages (In milliseconds).
    
**Example:**
```
chat: 
  filter: 
    enabled: true
    repeatDelay: 1000
```

## **Joinme settings**

Joinme settings (./joinme).

* ``headEnabled`` If `True` the player head is shown before the text message.
* ``multipleLines``If `True` multiple lines are used, otherwise only the first line is displayed.
* ``disabledScopes`` Specific servers or worlds where the joinme is disabled.
* ``cooldown`` How fast in succession a player can use the joinme.
  
  **Example:**
```
joinme: 
  headEnabled: true
  multipleLines: true
  disabledScopes: []
  cooldown: '15m'
```

## **Ip address settings**

Settings about ip address blocking

* ``blockAltMinPlaytime`` The maximum amount of game time a player needs to not be recognized as an alt account.
* ``historyType`` The used history to ban an alt account.
  
  **Example:**
```
ipAddress: 
  blockAltMinPlaytime: '3m'
  historyType: 'NETWORK'
```

