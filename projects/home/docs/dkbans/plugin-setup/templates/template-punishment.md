---
title: Punishment template
---

# Punishment template

This page describes, how to configure a punishment template. A punishment template is used for ban or warn commands.

## General template settings

* ``name`` The intern name for this template, which is also used in the command
* ``display`` The display name for this template. It is used for example in the chat
* ``permission`` The permission to be permitted for this template
* ``aliases`` All aliases to use this template in the command
* ``hidden`` If ``true``, the template is shown in the command, or else ``false``, the template is not shown in the command
* ``historyType`` The history type describes for which type the punishment should be executed. Available types: ``NETWORK``, `CHAT`
* ``category`` The category in this template to be grouped

**Example:**

````
name: Hacking
display: Hacking
permission: dkbans.ban.reason.hacking
aliases:
  - hacks
  - hacker
hidden: false
historyType: NETWORK
category: Bans
````

