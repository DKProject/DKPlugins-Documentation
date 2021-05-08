---
title: Filter
---

# Filter

DKBans filters bring a simple and easy solution to protect your server or network from offensive content. Filters can 
be created for different areas with different matching operations. Filters are managed with an ingame command.

How to use the command can be found [here]()

***

## Areas

To separate filters and define there scope, DKBans uses areas. DKBans has five built-in areas, more can be added with extensions:

**CHAT_ADVERTISING** => Used to block chat messages for advertising <br />
**CHAT_INSULT** => Used to block chat messages for insult <br />
**COMMANDS** => Used to block commands for all players <br />
**COMMANDS_MUTE** => Used to block commands for muted players <br />
**PLAYER_NAME** => Used to block player names (the player will not be able to join the server) <br />

***

## Operations

For comparing messages DKBans has five built-in operations, more can be added with extensions:

**EQUALS** => The input message must exactly match the filter value <br />
**CONTAINS** => The input message must contain the filter value <br />
**STARTS_WITH** => The input message must start with the filter value <br />
**ENDS_WITH** => The input message must end with the filter value <br />
**REGEX** => The input message must contain a regex pattern (Use [https://regexr.com/](https://regexr.com/) to build your pattern).
