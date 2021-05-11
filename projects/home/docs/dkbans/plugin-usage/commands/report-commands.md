---
title: Report Commands
---

# Report Commands

This page describes the usage and permissions of the DKBans report commands.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/report <player> <template>```](#report-player-template)
* [```/report <player> <reason>```](#report-player-reason)
* [```/report accept <player>```](#report-accept-player)
* [```/report decline <player>```](#report-decline-player)
* [```/report take <player>```](#report-take-player)
* [```/report list```](#report-list)
* [```/report login/logout/toggle```](#report-loginlogouttoggle)

***


!!! note 
    You need for all report commands the permission ``dkbans.command.report``. This permission is customizable
    in the command config (plugins/dkbans/commands.yml)


## **```/report <player> <template>```**

**Permission:** Configured permission of the template. Default: dkbans.report<br />
**Arguments:**
* `<player>` The target player to report
* `<template>` The template in the template group

This command reports the target ``<player>`` for the given `<template>`. The template must be configured in
the template group, otherwise it will not be able to report the player.

[Template configuration](../../plugin-setup/punishment-templates.md)

***

## **```/report <player> <reason>```**

**Permission:** dkbans.command.report<br />
**Arguments:**
* `<player>` The target player to report
* `<reason>` The reason to report

This command reports the target ``<player>`` for the given `<reason>`.

***

## **```/report accept <player>```**

**Permission:** dkbans.report.staff<br />
**Arguments:**
* `<player>` The target player to accept

This command accepts a report of the ``<player>``. The player will be banned for the configured punishment template,
if the report mode is template and punishment template is configured.

***

## **```/report decline <player>```**

**Permission:** dkbans.report.staff<br />
**Arguments:**
* `<player>` The target player to accept

This command decline a report of the ``<player>``. This means, that the report reason of the player is not applicable.

***

## **```/report take <player>```**

**Permission:** dkbans.report.staff<br />
**Arguments:**
* `<player>` The target player to accept

This command takes a report of the ``<player>``. The stuff (executor of the command) will watch the report and after
he watched he will use the ``accept`` or `decline` report command.

***

## **```/report list```**

**Permission:** dkbans.report.staff<br />

This command lists all open reports.

***

## **```/report login/logout/toggle```**

**Permission:** dkbans.report.staff<br />

This command controls, if the stuff is login or logout in the report system. This means, if the stuff is login, he
will receive notifications for open reports and if the stuff is logout he will not be able to interact with the
report system. Toggle will login or logout the stuff in the report system, depended on his previous login/logout state.

***