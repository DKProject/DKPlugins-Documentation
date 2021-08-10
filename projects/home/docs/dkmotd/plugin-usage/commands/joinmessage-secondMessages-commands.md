---
title: Join message Secondmessages Commands
---

# Join message second messages Commands

This page describes the usage and permissions of the Join message commands. The joinmessage command always
starts with `/joinmessage <name> secondMessages`, while `<name>` is the name of the joinmessage template.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/joinmessage <name> secondMessages add <line>```](#joinmessage-name-secondmessages-add-line)
* [```/joinmessage <name> secondMessages remove <index>```](#joinmessage-name-secondmessages-remove-index)
* [```/joinmessage <name> secondMessages set <line>```](#joinmessage-name-secondmessages-set-line)
* [```/joinmessage <name> secondMessages modify <index> <line>```](#joinmessage-name-secondmessages-modify-index-line)
* [```/joinmessage <name> secondMessages clear```](#joinmessage-name-secondmessages-clear)
***

## **```/joinmessage <name> secondMessages add <line>```**

**Permission:** dkmotd.command.joinmessage<br />
**Arguments:**

* `<name>` the name of joinmessage template
* `<line>` the new line to be added

This command adds a new line to the second messages.

***

## **```/joinmessage <name> secondMessages remove <index>```**

**Permission:** dkmotd.command.joinmessage<br />
**Arguments:**

* `<name>` the name of joinmessage template
* `<index>` the index to remove

This command removes line of the second messages by the index of the line.

***

## **```/joinmessage <name> secondMessages set <line>```**

**Permission:** dkmotd.command.joinmessage<br />
**Arguments:**

* `<name>` the name of joinmessage template
* `<line>` the line to set

This command sets the line of the second messages and removes all other lines.

***

## **```/joinmessage <name> secondMessages modify <index> <line>```**

**Permission:** dkmotd.command.joinmessage<br />
**Arguments:**

* `<name>` the name of joinmessage template
* ``<index>`` the index to modify
* `<line>` the modified line

This command modifies the second message of the ``<index>`` to `<line>`.

***

## **```/joinmessage <name> secondMessages clear```**

**Permission:** dkmotd.command.joinmessage<br />
**Arguments:**

* `<name>` the name of joinmessage template

This command clears the second messages of the joinmessage template.

***