---
title: DKPerms Events
---

# DKPerms Events

DKPerms provides several events for better interaction with the plugin. You can use events in a 
normal Bukkit/BungeeCord listener with `@EventHandler` or subscribe to the McNative event bus.
If you need other events, create a [suggestion](../support.md#suggestions).

## Usage

The usage for all


### Bukkit / BungeeCord

On Bukkit and BungeeCord, you can use the normal `@EventHandler` in a listener to subscribe to a DKPerms event

```
@EventHandler
public void onPermissionCalculate(DKPermsPermissionCalculationEvent event){
    if(event.getObject().getName().equals("Dkrieger")){
        event.setAction(PermissionAction.ALLOW);
    }
}
```


### McNative

In a McNative plugin, you can use the `@Listener` annotation or subscribe directly to the local event bus.

```
@Listener
public void onPermissionCalculate(DKPermsPermissionCalculationEvent event){
    if(event.getObject().getName().equals("Dkrieger")){
        event.setAction(PermissionAction.ALLOW);
    }
}
```

****


## Available events

You can use all events listed here.

### DKPermsPermissionObjectCreateEvent

This event is fired, when a new permission object (e.g. player, group) is created. 


### DKPermsPermissionObjectDeleteEvent

This event is fired, when a new permission object (e.g. player, group) is deleted.


### DKPermsPermissionCalculationEvent

This event is fired when a permission of an object is checked. You can change the permission result with this event.


### DKPermsScopeChangeEvent

This event is fired when a player switches to a new scope (e.g. from World-1 to World-2).
