---
title: Punishment templates
---

# Punishment templates

DKBans V5 brings a completely redesigned punishment template system with more possibilities and flexibility to your server 
or network. With the new template architecture you can create innovative punishment procedures with calculation algorithms, 
different types of punishments and more.


***

## **Introduction**

The template system consists of two parts, the `template group` and the `template`. A `template group` is a list of 
related templates. And a `template` contains the exact punishment information and belongs to a `template group`.

**Template Group** <br />
A template group is usually bound to a command (.e.g. `./ban`, `./cityBuildBan` or `./warn`), and contains related templates. 
You are very flexible and can create as many template groups as you need.

**Template** <br />
A template (e.g. hacking, advertising, provocation) contains exact information about the punishment, how he will be 
punished (ban, mute, warning etc.), how long the player will be punished and all other information.

### Punishment type
DKBans offers four known punishment types, more can be added with extensions.

**BAN** => The player is no longer able to join your server. <br />
**MUTE** => The player is no longer able to use the chat and LabyMod voice chat. <br />
**KICK** => The player will be kicked from the server. <br />
**WARN** => A simple warning message is sent to the player. <br />

### Punishment calculation 

DKBans contains two different algorithms for calculating the best punishments for your bad players.

**AMOUNT calculation** <br />
DKBans points system is an intelligent algorithm for calculating the best type and duration based on the 
unique player history. Each punishment adds a certain amount of points to the player's history, which is used to 
calculate the next punishment. You are also able to define divider and multiplier to get more accurate 
and better punishments for different reasons and templates.


### History types
Another powerful technology of DKBans is the unique history system that allows you to create separate 
calculation units for amounts and points. For example, you can separate network and chat penalties into 
different histories, or even create a separate history for a server (e.g. CityBuild).

***

## Configure a template group

A template group corresponds to a file in the `./plugins/DKBans/templates` folder. There are already 
three default groups (`ban`, `report` and `unban`). If you need another group, e.g. for warnings or to create 
server punishments, simply create a new file. The file must contain the following header information:

* ``type`` DKBans differentiates between three core template types: `PUNISHMENT`, `UNPUNISH` and `REPORT`.
* ``calculation`` The calculation type to use, `AMOUNT` or `POINTS` (see above fill explanation)
* ``name`` The name of this template group, should be similar to the file name
* ``templates`` All templates of this group, see below.


**Example:**
```
type: PUNISHMENT
calculation: AMOUNT
name: ban
templates:
```


If you want to use this template group in combination  with a command, you need to configure it in the 
punishment template section (line 190) in the `commands.yml`.

Add this section with the name of the command and template group to your `commands.yml`:
```
<template-group-name>: 
  enabled: true
  name: 'ban'
  permission: 'dkbans.ban'
  aliases: ['mute']
```

***

## Configure a template

Each template group contains one to infinite number of templates. The template format looks different for the three template types.

### Punishment
Required template group type: `PUNISHMENT` (see above)

* ``<id>`` The internal id of your template (use only number values)
    * ``name`` The unique name of this template
    * ``display`` The display name in the ban screen
    * ``permission`` The required permission to use this template
    * ``aliases`` Alternative names to use in commands 
    * ``hidden`` If `True`, the template will not be displayed in commands
    * ``historyType`` The name of the history type to use for this template (See above for more information)
    * ``<amount/points>`` The amount of punishments or points (depending on the selected calculation)
        * ``type`` The punishment type (See above for more information)
        * ``duration`` The duration of the punishment (not all punishment types have a duration)
  * ``points`` Additional configuration for points (only in `POINTS` calculation)
      * ``addedPoints`` Points to add to the history for this punishment
      * ``pointsDivider`` The divider to use before the duration calculation

**Example:**
```
templates:
  1:
    name: Hacking
    display: Hacking
    permission: dkbans.ban.reason.hacking
    aliases:
      - hacks
      - hacker
    hidden: false
    historyType: NETWORK
    category: Bans
    messageKey: test
    durations:
      1:
        type: BAN
        duration: 30d
      2:
        type: BAN
        duration: 90d
      3:
        type: BAN
        duration: -1
    points:
      addedPoints: 7
      pointsDivider: 1.0
```


### Report
Required template group type: `REPORT` (see above)

* ``<id>`` The internal id of your template (use only number values)
    * ``name`` The unique name of this template
    * ``display`` The display name in the ban screen
    * ``permission`` The required permission to use this template
    * ``watchPermission`` The required permission to take and watch this report
    * ``aliases`` Alternative names to use in commands
    * ``hidden`` If `True`, the template will not be displayed in commands
    * ``targetPunishment`` The target punishment when a report gets accepted (Format: <template-group>@<template-name>)

**Example:**
```
templates:
  1:
    name: Hacking
    display: Hacking
    permission: dkbans.report
    watchPermission: dkbans.report.staff
    aliases:
      - hacking
    hidden: false
    targetPunishment: ban@Hacking
```

### Unpunishment
Required template group type: `UNPUNISHMENT` (see above)

**Work in progress**


## Import

After you have configured the templates, you need to import them into your database using the following command:

`./dkbans template import`
