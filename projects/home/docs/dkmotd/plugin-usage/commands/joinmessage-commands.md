---
title: Join message Commands
---

# Join message Commands

This page describes the usage and permissions of the Join message commands. The join message command always
starts with `/joinmessage <name>`, while `<name>` is the name of the join message template.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/joinmessage list```](#joinmessage-list)
* [```/joinmessage <name> [info]```](#joinmessage-name-info)
* [```/joinmessage <name> active```](#joinmessage-name-active)
* [```/joinmessage <name> create```](#joinmessage-name-create)
* [```/joinmessage <name> delete```](#joinmessage-name-delete)
* [```/joinmessage <name> name <newName>```](#joinmessage-name-name-newname)
* [```/joinmessage <name> baseMessage <text>```](#joinmessage-name-basemessage-text)
* [```/joinmessage <name> secondMessages```](#joinmessage-name-secondmessages)
***

## **```/joinmessage list```**

**Permission:** dkmotd.command.joinmessage<br />

This is the joinmessage list command. It lists all joinmessage templates.

***

## **```/joinmessage <name> [info]```**

**Permission:** dkmotd.command.joinmessage<br />
**Arguments:**

* `<name>` the name of joinmessage template

This is the base command for a joinmessage template. It shows you all information of the joinmessage template, like name, baseMessage and more.
If the joinmessage template does not exist, it will be shown in the chat.

***

## **```/joinmessage <name> active```**

**Permission:** dkmotd.command.joinmessage<br />
**Arguments:**

* `<name>` the name of joinmessage template

This command toggle the active of a joinmessage template. If you toggle on a joinmessage template, all other joinmessage templates will be inactive.

***

## **```/joinmessage <name> create```**

**Permission:** dkmotd.command.joinmessage<br />
**Arguments:**

* `<name>` the name of joinmessage template

This command creates a new joinmessage template with the name ``<name>``.

***

## **```/joinmessage <name> delete```**

**Permission:** dkmotd.command.joinmessage<br />
**Arguments:**

* `<name>` the name of joinmessage template

This command deletes the joinmessage template ``<name>``, if it exists.

***

## **```/joinmessage <name> name <newName>```**

**Permission:** dkmotd.command.joinmessage<br />
**Arguments:**

* `<name>` the name of joinmessage template
* `<newName>` the new name of joinmessage template

This command renames the joinmessage template to ``<newName>``, if no other joinmessage template is named `<newName>`.

***

## **```/joinmessage <name> baseMessage <text>```**

**Permission:** dkmotd.command.joinmessage<br />
**Arguments:**

* `<name>` the name of joinmessage template
* `<text>` the new text of joinmessage template

This command changes the joinmessage baseMessage to ``<text>``.

***

## **```/joinmessage <name> secondMessages```**

**Permission:** dkmotd.command.joinmessage<br />
**Arguments:**

* `<name>` the name of joinmessage template

This command manages the second messages of a joinmessage template. For more information, look on this [page](joinmessage-secondMessages-commands.md).

***