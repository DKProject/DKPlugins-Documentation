---
title: Filter Commands
---

# Filter Commands

This page describes the usage and permissions of the DKBans filter commands.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/filter list```](#filter-list)
* [```/filter add <area> <value> [operation]```](#filter-add-area-value-operation)
* [```/filter remove <id>```](#filter-remove-id)

***

## **```/filter list```**

**Permission:** dkbans.command.filter<br />

List all available filters on this network.

***

## **```/filter add <area> <value> [operation]```**

**Permission:** dkbans.command.filter<br />
**Arguments:**
* `<area>` The area to add this filter
* `<value>` The value of the filter
* `[operation]` The compare operation/algorithm

Add a new filter and block messages.

**Available areas:**

* `CHAT_ADVERTISING` Block messages from the chat for advertising
* `CHAT_INSULT` Block messages from the chat for insulting
* `COMMAND` Block entire commands for the network
* `COMMAND_MUTE` Block commands for muted players (e.g. ./msg)
* `PLAYER_NAME` Block player names from the network

**Available operations:**

* `EQUALS` The filter value and the chat input must exactly match
* `CONTAINS` The chat input must contain the value
* `STARTS_WITH` The chat input must start with the value
* `ENDS_WITH` The chat input must end the value
* `REGEX` The chat input matches with the configured regex

***

## **```/filter remove <id>```**

**Permission:** dkbans.command.filter<br />
**Arguments:**
* `<id>` The id of the filter (available in filter list)

Remove an existing filter by id.
