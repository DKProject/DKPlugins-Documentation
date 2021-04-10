---
title: DKPerms scopes
---

# DKPerms scopes

DKPerms uses an innovative scope architecture to segregate permissions between different
scopes (e.g. servers, worlds, etc.) and to prioritize the weight of each permission. Scopes are 
created automatically and managed internally in DKPerms. There are many ways to obtain scopes.

****

## Root scope

The root area is the base scope of the tree structure.

```java
PermissionScope scope = dkperms.getScopeManager().getRoot();
```

****

## Namespace scope

DKPerms separates permission areas between parent namespaces to have more possibilities to extend DKPerms to other 
areas (e.g. Discord, TeamSpeak). In most cases, you will only need the `Minecraft` namespace.

```java
PermissionScope scope = dkperms.getScopeManager().getNamespace("Minecraft");
```

****

## Current instance scope

Each runtime instance has its own base scope, which defines the current location of the instance.
However, also note that not every player has the same scope on the same instance.


```java
PermissionScope scope = dkperms.getScopeManager().getCurrentInstanceScope();
```

****

## Obtain scope tree

As mentioned before, DKPerms scopes are structured in a tree, you can easily find the required 
scope using the `getChild` method.

```java
PermissionScope scope = dkperms.getScopeManager().getRoot()
        .getChild("namespace","Minecraft")
        .getChild("server","Lobby-1")
        .getChild("world","World-1");
```

****

## Compile scope tree

You are also able to easily compile a scope definition string to a DKPerms scope tree.

```java
PermissionScope scope = dkperms.getScopeManager().get("namespace=Minecraft\\server=Lobby-1\\world=World-1");
```



