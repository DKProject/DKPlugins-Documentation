---
title: Motd supported versions Commands
---

# Motd supported versions Commands

This page describes the usage and permissions of the Motd commands. The motd command always
starts with `/motd <name> supportedVersions`, while `<name>` is the name of the motd template.

Important things to remember:

* Required arguments are declared with ```<example>```
* Optional arguments are declared with ```[example]```

#### Index

* [```/motd <name> supportedVersions add <version>```](#motd-name-supportedversions-add-version)
* [```/motd <name> supportedVersions remove <version>```](#motd-name-supportedversions-remove-version)
* [```/motd <name> supportedVersions set <version>```](#motd-name-supportedversions-set-version)
* [```/motd <name> supportedVersions modify <index> <version>```](#motd-name-supportedversions-modify-index-version)
* [```/motd <name> supportedVersions clear```](#motd-name-supportedversions-clear)
***

## **```/motd <name> supportedVersions add <version>```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `<name>` the name of motd template
* `<version>` the new version to be added

This command adds a new supported version.

***

## **```/motd <name> supportedVersions remove <version>```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `<name>` the name of motd template
* `<version>` the version to remove

This command removes the supported ``<version>``.

***

## **```/motd <name> supportedVersions set <version>```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `<name>` the name of motd template
* `<version>` the supported version to set

This command sets the supported version of the supported versions and removes all other supported versions.

***

## **```/motd <name> supportedVersions modify <index> <version>```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `<name>` the name of motd template
* ``<index>`` the index to modify
* `<version>` the supported version

This command modifies the supported versions of the ``<index>`` to `<version>`.

***

## **```/motd <name> supportedVersions clear```**

**Permission:** dkmotd.command.motd<br />
**Arguments:**

* `<name>` the name of motd template

This command clears the supported versions of the motd template.

***