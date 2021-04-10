---
title: Developer Getting Started
---

# Getting Started

DKPerms contains a large and powerful API that is easy to use. The api is very flexible and gives you the 
possibility to fully interact with DKPerms. You don't need to worry about anything else, the DKPerms api 
interface will handle everything for you.


**Thread safety**

All operations in DKPerms are totally thread safety and designed for asynchronously usage.

**Storage & Synchronisation operations**

DKPerms offers you a simple api to create, modify, update and delete objects scopes and other stuff. You have not to deal 
with saving or synchronizing data, DKPerms is automatically handling those things in the background.


## Javadocs

The full Api documentation is available as Javadocs [here](https://javadocs.pretronic.net/dkperms). 
This wiki covers only basic examples, the api is much bigger and offers many more possibilities.

## Dependency

DKPerms is built with the Maven build tool and has its own repository (Public available).

**Repository**

=== "Maven"

    ``` xml
    <repository>
        <id>pretronic</id>
        <url>https://repository.pretronic.net/repository/pretronic/</url>
    </repository>

    ```

=== "Gradle"

    ```
    repositories {
        maven {
            url "https://repository.pretronic.net/repository/pretronic/"
        }
    }
    ```

**Dependency**


=== "Maven"

    ``` xml
    <dependency>
        <groupId>net.pretronic.dkperms</groupId>
        <artifactId>dkperms-api</artifactId>
        <version>VERSION</version>
        <scope>compile</scope>
    </dependency>
    ```

=== "Gradle"

    ```
    dependencies {
        compile 'net.pretronic.dkperms:dkperms-api:VERSION'
    }




    ```


**Get the DKPerms instance**

You can obtain the DKPerms instance through the McNative service registry or use the direct instance.

**Direct access:**
```
DKPerms dkperms = DKPerms.getInstance();
```

**Over McNative service registry:**
```
DKPerms dkperms = McNative.getInstance().getRegistry().getService(DKPerms.class);
```

If you are in a McNative plugin class, you can also use the `getRuntime` method.
```
DKPerms dkperms = getRuntime().getService(DKPerms.class);
```
