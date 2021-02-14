---
title: Storage
---

# Storage setup

DKBans uses the McNative storage technology and supports all storage types supported by McNative. McNative storage technology 
is centralized storage integration for all supported plugins, it brings various performance and time benefits. Read more about it [here]()

**Location:** ``./plugins/McNative/storage.yml``

The configuration consists of two parts, the drivers that connect to the database server which are
shared between the plugins, and the database part, where you can configure the database for each plugin.

### **Driver settings**

You can use the same driver for multiple plugins, see all supported types and configuration options in the McNative documentation. Only one sql setup is covered on this page.

[McNative driver docs](https://github.com/McNative/McNative/wiki/Storage-Configuration)

* ``mysql`` The internal name of the driver (Used below in the database `driverName` setting)
  * ``address`` The address of your database server
  * ``username`` The username to authenticate 
  * ``password`` The password to authenticate
  * ``driver`` The used driver (See all available drivers in the McNative docs)
  * ``name`` The internal driver name (Used for logging and separation)
  * ``dialectName`` The sql dialect (Supported: MySQL, MariaDB, MS-SQL, PostgreSQL)
  * ``useSSL`` The above configured driver to use
    
**Example:**
```
drivers: 
  mysql: 
    address: '127.0.0.1:3306'
    username: 'mcnative'
    password: '1234'
    driver: 'net.pretronic.databasequery.sql.driver.SQLDatabaseDriver'
    name: 'MySQL'
    dialectName: 'MySQL'
    useSSL: false
```

### **Database settings**

After the driver configuration, you have to set up a database for DKBans in the `databases` section.

* ``pluginName`` The plugin name, use `DKBans`
* ``name`` The internal database name, use `default`
* ``database`` The name of your database (e.g. `DKBans`)
* ``driverName`` The above configured driver to use

**Example:**
```
databases: 
  - pluginName: 'DKBans'
    name: 'default'
    database: 'DKBans'
    driverName: 'default'
```

### **Database settings**
A complete configuration may look something like this (Only DKBans):

```
drivers: 
  mysql: 
    address: '127.0.0.1:3306'
    username: 'mcnative'
    password: '1234'
    driver: 'net.pretronic.databasequery.sql.driver.SQLDatabaseDriver'
    name: 'MySQL'
    dialectName: 'MySQL'
    useSSL: false
databases: 
  - pluginName: 'DKBans'
    name: 'default'
    database: 'DKBans'
    driverName: 'mysql'
```
