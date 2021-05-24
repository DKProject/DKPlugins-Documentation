---
title: IP-Address Commands
---

# IP-Address Commands

This page describes the usage and permissions of the DKBans ip commands.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/ipInfo <player>```](#ipinfo-player)
* [```/ipInfo <address>```](#ipinfo-address)
* [```/ipInfo <address> details```](#ipinfo-address-details)

* [```/ipblock <address> <reason> template <template>```](#ipblock-address-reason-template-template)
* [```/ipblock <address> <reason> temporary ```](#ipblock-address-reason-temporary-duration-ban-reason)
* [```/ipblock <address> <reason> permanently```](#ipblock-address-reason-permanently-ban-reason)

* [```/ipunblock <address> ```](#ipunblock-address)

***

## **```/ipInfo <player>```**

**Permission:** dkbans.command.ipInfo<br />
**Arguments:**
* `<player>` The player

Get information about all ip addresses of a player.

***

## **```/ipInfo <address>```**

**Permission:** dkbans.command.ipInfo<br />
**Arguments:**
* `<address>` The ip address to check

Get ip information about this addresses and all player which connect from this address.

***

## **```/ipInfo <address> details```**

**Permission:** dkbans.command.ipInfo<br />
**Arguments:**
* `<address>` The ip address to check

Get detailed information if this ip is blocked and more

***

## **```/ipblock <address> <reason> template <template>```**

**Permission:** dkbans.command.ipBlock<br />
**Arguments:**
* `<address>` The ip address to check
* `<reason>` The reason for this ip block
* `template` Indicated a template ban assignment
* `<template>` The template id (<group>@<id>)

Block an ip address, if a player joins with this ip, he will automatically be banned for the configured template.

***

## **```/ipblock <address> <reason> temporary <duration> <ban-reason>```**

**Permission:** dkbans.command.ipBlock<br />
**Arguments:**
* `<address>` The ip address to check
* `<reason>` The reason for this ip block
* `temporary` Indicated a temporary ban assignment with a reason
* `<duration>` The duration of the ban
* `<ban-reason>` The reason for which the player gets banned

Block an ip address, if a player joins with this ip, he will automatically be banned for the configured duration and reason.

***

## **```/ipblock <address> <reason> permanently <ban-reason>```**

**Permission:** dkbans.command.ipBlock<br />
**Arguments:**
* `<address>` The ip address to check
* `<reason>` The reason for this ip block
* `temporary` Indicated a temporary ban assignment with a reason
* `<ban-reason>` The reason for which the player gets banned

Block an ip address, if a player joins with this ip, he will automatically be banned for the configured reason.


***

## **```/ipunblock <address>```**

**Permission:** dkbans.command.ipUnblock<br />
**Arguments:**
* `<address>` The ip address to check

Unblock an ip address (players which are not banned can again join, players which are automatically banned based on the block will still not be able to join)
