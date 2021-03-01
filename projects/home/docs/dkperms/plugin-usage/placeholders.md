---
title: Placeholders
---

# Placeholders

DKPerms offers many placeholders which can be used in other plugins to display data provided by DKPerms. 
DKPerms placeholders are available in all McNative supported placeholder sources (PlaceholderAPI).

***

## %dkperms_name%F

This placeholder shows the name of the player. 

***

## %dkperms_uniqueId%

This placeholder shows the unique id of the player 

***

## %dkperms_id%

This placeholder returns the unique internal object ID of DKPerms.

***

## %dkperms_scope%

Returns the actual scope where a player is currently located. Note that this can cause problems with proxy networks.

***

## %dkperms_rank%

Returns the highest rank of the player, ordered by priority.

***

## %dkperms_ranks%

Returns all assigned ranks of a player, separated by a comma. Group colors are not contained in this placeholder.

***

## %dkperms_color%

Returns the color of the player. The color is provided by the McNative player design and set directly 
to a player or an assigned group as a meta value in DKPerms.

***

## %dkperms_prefix%

Returns the prefix of the player. The prefix is provided by the McNative player design and set directly
to a player or an assigned group as a meta value in DKPerms.

***

## %dkperms_suffix%

Returns the color of the suffix. The suffix is provided by the McNative player design and set directly
to a player or an assigned group as a meta value in DKPerms.

***

## %dkperms_display%

Returns the dispaly (chat prefix) of the suffix. The dispaly (chat prefix) is provided by the McNative player design and set directly
to a player or an assigned group as a meta value in DKPerms.

***

## %dkperms_priority%

Returns the player priority (used in the tab). The priority is provided by the McNative player design and set directly 
to a player or assigned group as a meta value in DKPerms. If no meta is set, the highest group priority is taken.

***

## %dkperms_team%

Returns `true` if the player is in a group marked as `team` (set via the group meta).

***

## %dkperms_property_\<KeyName>%

This placeholder returns a custom meta value set on a DKPerms object or an assigned group.
Replace `<KeyName>` with the name of your meta key.

***

## %dkperms_boolProperty_\<KeyName>%

This placeholder returns a custom meta value set on a DKPerms object or an assigned group.
Replace `<KeyName>` with the name of your meta key.
In addition to the normal property, it returns `true` if the value matches `true`, otherwise it returns false.

***

## %dkperms_numberProperty_\<KeyName>%

This placeholder returns a custom meta value set on a DKPerms object or an assigned group. 
Replace `<KeyName>` with the name of your meta key. 
In addition to the normal property, 0 is returned if the value is not set.
