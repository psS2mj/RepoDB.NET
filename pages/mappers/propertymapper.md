---
layout: default
sidebar: mappers
title: "PropertyMapper"
description: "A mapper class that is being used to map the class property into its equivalent column in the database. This class is used as an alternative to Map attribute."
permalink: /mapper/propertymapper
tags: [repodb, class, propertymapper, orm, hybrid-orm, sqlserver, sqlite, mysql, postgresql]
parent: MAPPERS
---

# PropertyMapper

---

A mapper class that is being used to map the class property into its equivalent column in the database. This class is used as an alternative to the [Map](/attribute/map) attribute.

### Methods

Below are the methods available from this class.

- `Add` - adds a database column name mapping into a property.
- `Clear` - clears all the existing database columns mappings.
- `Get` - gets the existing mapped database column name of the property.
- `Remove` - removes the exising mapped database column name of the property.

### Usability

To add a mapping, simply call the `Add()` method.

```csharp
PropertyMapper.Add<Customer>(c => c.FirstName, "[FName]", true);
PropertyMapper.Add<Customer>(c => c.LastName, "[LName]", true);
PropertyMapper.Add<Customer>(c => c.DateOfBirth, "[DOB]", true);
```

> An exception will be thrown if the mapping is already exists and you passed a `false` value in the `force` argument.

To get the mapping, use the `Get()` method.

```csharp
var mappedName = PropertyMapper.Get<Customer>(c => c.FirstName);
```

> Please consider to always use the [PropertyMappedNameCache](/cacher/classmappednamecache) class when extracting the mapped property name.

To remove the mapping, use the `Remove()` method.

```csharp
PropertyMapper.Remove<Customer>(c => c.FirstName);
```