---
title: Bank member Commands
---

# Bank Member Commands

This page describes the usage and permissions of the Bank member commands. The bank command always
starts with `/bank <name> member`, while `<name>` is the name of the bank.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```[list]```](#list)
* [```<member> [info]```](#member-info)
* [```<member> add```](#member-add)
* [```<member> remove```](#member-remove)
* [```<member> role <role>```](#member-role-role)
* [```<member> limit```](#member-limit)


***

## **```[list]```**

**Permission:** dkcoins.command.bank<br/>

This command lists all members of this bank.

***

## **```<member> [info]```**

**Permission:** dkcoins.command.bank<br/>
**Arguments:**
* `member` the target member name

This command shows a detailed overview about the specific member.

***

## **```<member> add```**

**Permission:** dkcoins.command.bank<br/>
**Arguments:**
* `member` the target member name

This command adds a member to your bank, if the member is not already add to this bank.

***

## **```<member> remove```**
**Arguments:**
* `member` the target member name

**Permission:** dkcoins.command.bank<br/>

This command removes the member from the bank, if the member is a member of the bank.

***

## **```<member> role <role>```**
**Arguments:**
* `member` the target member name
* `role` the role to set

**Permission:** dkcoins.command.bank<br/>

This command change the role of the member. The specific role must be lower in the hierarchies as the own role.

Available roles (The Highest role on top):
* OWNER
* ADMIN
* MANAGER
* USER
* GUEST

***

## **```<member> limit```**

**Permission:** dkcoins.command.bank<br/>
**Arguments:**
* `member` the target member name

This command manage the limit of the specific member.
For more information about the limit commands, [click here](bank-limit-commands.md).