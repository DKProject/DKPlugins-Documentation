---
title: Motd Commands
---

# Motd Commands

This page describes the usage and permissions of the Motd commands. The motd command always
starts with `/motd <name>`, while `<name>` is the name of the motd template.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/motd list```](#motd-list)
* [```/motd <name> [info]```](#motd-name-info)
* [```/motd <name> active```](#motd-name-active)
* [```/motd <name> create```](#motd-name-create)
* [```/motd <name> delete```](#motd-name-delete)
* [```/motd <name> name <newName>```](#motd-name-name-newname)
* [```/motd <name> baseLine <text>```](#motd-name-baseline-text)
* [```/motd <name> secondLines```](#motd-name-secondlines)
* [```/motd <name> versionText <text>```](#motd-name-versiontext-text)
* [```/motd <name> wrongVersionText <text>```](#motd-name-wrongversiontext-text)
* [```/motd <name> supportedVersions```](#motd-name-supportedversions)
* [```/motd <name> favicon <favicon>```](#motd-name-favicon-favicon)
* [```/motd <name> playerInfo```](#motd-name-playerinfo)
***

## **```/motd list```**

**Permission:** dkmotd.command.motd<br />

This is the motd list command. It lists all motd templates.

***

## **```/motd <name> [info]```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `name` the name of motd template

This is the base command for a motd template. It shows you all information of the motd template, like name, baseLine and more.
If the motd template does not exist, it will be shown in the chat.

***

## **```/motd <name> active```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `name` the name of motd template

This command toggle the active of a motd template. If you toggle on a motd template, all other motd templates will be inactive.

***

## **```/motd <name> create```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `name` the name of motd template

This command creates a new motd template with the name ``<name>``.

***

## **```/motd <name> delete```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `name` the name of motd template

This command deletes the motd template ``<name>``, if it exists.

***

## **```/motd <name> name <newName>```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `name` the name of motd template
* `newName` the new name of motd template

This command renames the motd template to ``<newName>``, if no other motd template is named `<newName>`.

***

## **```/motd <name> baseLine <text>```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `name` the name of motd template
* `text` the new text of motd template

This command changes the motd baseLine to ``<text>``.

***

## **```/motd <name> secondLines```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `name` the name of motd template

This command manages the second lines of a motd template. For more information, look on this [page](motd-secondLines-commands.md).

***

## **```/motd <name> versionText <text>```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `name` the name of motd template
* `text` the new version text of the motd template

This command changes the motd version text to ``<text>``.

***

## **```/motd <name> wrongVersionText <text>```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `name` the name of motd template
* `text` the new wrong version text of the motd template

This command changes the motd wrong version text to ``<text>``.

***

## **```/motd <name> supportedVersions```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `name` the name of motd template

This command manages the supported versions of a motd template. For more information, look on this [page](motd-supportedVersions-commands.md).

***

## **```/motd <name> favicon <favicon>```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `name` the name of motd template
* `favicon` the new favicon of the motd template

This command changes the motd favicon to ``<favicon>``.

The ``<favicon>`` must be a valid image url (starting with http) or a valid file path.
Also the image must be in a 64x64 format.
***

## **```/motd <name> playerInfo```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `name` the name of motd template

This command manages the player info of a motd template. For more information, look on this [page](motd-playerInfo-commands.md).

***