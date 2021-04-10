---
title: Templates
---

# Templates

This page describes all possibility to operate with the dkbans template system. By default, there are three template types,
PUNISHMENT, REPORT and UNPUNISHMENT. All of them have some similarities. These are explained [below](#template-definition).
All templates are stored in the folder ````plugins/DKBans/templates````.

## General template definition

These template settings have to configured for all template types.

* ``type`` The type, which the template should have. Available type: PUNISHMENT, REPORT, UNPUNISHMENT
* ``calculation`` The type, how a template should operate with command interactions. Available calculation types: [AMOUNT](), [POINTS]()
* ``name`` The name for the group of templates
* ``templates`` All templates for this template group. The configuration depends on the [template type](#template-types). The number of the template should be incremented each time.

**Example:**
```
type: PUNISHMENT
calculation: AMOUNT
name: ban
templates:
    1:
        [...]
    2:
        [...]
    3:
        [...]
```

## Template types

These are the available template types.

* [```PUNISHMENT```](template-punishment.md)
* [```UNPUNISHMENT```](template-unpunishment.md)
* [```REPORT```](template-report.md)