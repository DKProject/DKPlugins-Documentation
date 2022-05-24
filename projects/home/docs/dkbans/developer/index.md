---
title: Developer Getting Started
---

# Getting Started

DKBans contains a large and powerful API that is easy to use. The api is very flexible and gives you the 
possibility to fully interact with DKBans. You don't need to worry about anything else, the DKBans api 
interface will handle everything for you.

!!! note ""
    **As soon as McNative is available for developers, we will document exactly how to use and integrate with DKBans.
    If you already want to use the DKBans api, use the development channel on our Discord to get help from us and our community.**

**Thread safety**

All operations in DKBans are totally thread safety and designed for asynchronously usage.

**Storage & Synchronisation operations**

DKBans offers you a simple api to create, modify, update and delete currency and bank account and other things. 
You have not to deal with saving or synchronizing data, DKBans is automatically handling those things in the background.


## Javadocs

The full Api documentation is available as Javadocs [here](https://javadocs.pretronic.net/dkbans). 
This wiki covers only basic examples, the api is much bigger and offers many more possibilities.

## Dependency

DKBans is built with the Maven build tool and has its own repository (Public available).

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
        <groupId>net.pretronic.dkbans</groupId>
        <artifactId>dkbans-api</artifactId>
        <version>VERSION</version>
        <scope>compile</scope>
    </dependency>
    ```

=== "Gradle"

    ```
    dependencies {
        compile 'net.pretronic.dkbans:dkbans-api:VERSION'
    }




    ```
