---
layout: default
sidebar: mappers
title: "DbSettingMapper"
description: "A mapper class for all the database setting classes. The mapping can be made based on the type of the target RDBMS data provider."
permalink: /mapper/dbsettingmapper
tags: [repodb, class, dbsettingmapper, orm, hybrid-orm, sqlserver, sqlite, mysql, postgresql]
parent: MAPPERS
---

# DbSettingMapper

---

A mapper class for the [IDbSetting](/interface/idbsetting)-based class. The mapping can be made based on the type of the target RDBMS data provider. Please visit the [Database Setting](/extensibility/databasesetting) for more information.

### Methods

Below are the methods available from this class.

- `Add` - adds a mapping between the [IDbSetting](/interface/idbsetting) and the type of the `DbConnection`.
- `Clear` - clears all the existing mappings of the database settings.
- `Get` - gets the existing mapped [IDbSetting](/interface/idbsetting) object based on the type of the `DbConnection`.
- `Remove` - removes the existing mapped [IDbSetting](/interface/idbsetting) object based on the type of the `DbConnection`.

### Usability

To add a mapping, simply call the `Add()` method.

```csharp
DbSettingMapper.Add<SqlConnection>(new MyCustomSqlServerDbSetting(), true);
```

> An exception will be thrown if the mapping is already exists and you passed a `false` value in the `force` argument.

To get the mapping, use the `Get()` method.

```csharp
var dbSetting = DbSettingMapper.Get<SqlConnection>();
```

To remove the mapping, use the `Remove()` method.

```csharp
DbSettingMapper.Remove<SqlConnection>();
```

