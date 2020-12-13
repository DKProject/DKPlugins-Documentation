---
title: Frequently Asked Questions
---

# Frequently Asked Questions

These page contains some questions which are frequently asked about DKPerms.
Before you ask a question in our support, please check this page and make sure that the question is not already answered.

***
## How can I create a default group?
DKPerms handles default groups in its meta. You can set a group as default on the whole network or on a specified server.

If you set the meta ```default``` to ```true``` of a group, all players will automatically gets all permissions
of the group, but the group is not directly assigned to the player. If you want set a group to each player when he
joined the server, you can set the meta ``defaultAssign``` to ```true```, so every new player automatically receives this group.

**Examples**

```/perms group <group> meta set default true```

```/perms group <group> meta set defaultAsign true```

```/perms group <group> meta set default true world=world-1```
In this case the group is only default on world-1
