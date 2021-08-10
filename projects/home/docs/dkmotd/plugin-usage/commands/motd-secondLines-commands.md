---
title: Motd Secondlines Commands
---

# Motd second lines Commands

This page describes the usage and permissions of the Motd commands. The motd command always
starts with `/motd <name> secondLines`, while `<name>` is the name of the motd template.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/motd <name> secondlines add <line>```](#motd-name-secondlines-add-line)
* [```/motd <name> secondlines remove <index>```](#motd-name-secondlines-remove-index)
* [```/motd <name> secondlines set <line>```](#motd-name-secondlines-set-line)
* [```/motd <name> secondlines modify <index> <line>```](#motd-name-secondlines-modify-index-line)
* [```/motd <name> secondlines clear```](#motd-name-secondlines-clear)
***

## **```/motd <name> secondlines add <line>```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `<name>` the name of motd template
* `<line>` the new line to be added

This command adds a new line to the second lines.

***

## **```/motd <name> secondlines remove <index>```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `<name>` the name of motd template
* `<index>` the index to remove

This command removes line of the second lines by the index of the line.

***

## **```/motd <name> secondlines set <line>```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `<name>` the name of motd template
* `<line>` the line to set

This command sets the line of the second lines and removes all other lines.

***

## **```/motd <name> secondlines modify <index> <line>```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `<name>` the name of motd template
* ``<index>`` the index to modify
* `<line>` the modified line

This command modifies the second line of the ``<index>`` to `<line>`.

***

## **```/motd <name> secondlines clear```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `<name>` the name of motd template

This command clears the second lines of the motd template.

***