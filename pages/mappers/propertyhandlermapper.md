---
layout: default
sidebar: mappers
title: "PropertyHandlerMapper"
description: "A class that is being used to map a property handler into a .NET CLR type or a class property. This class is used as an alternative to PropertyHandler attribute."
permalink: /mapper/propertyhandlermapper
tags: [repodb, class, propertyhandlermapper, orm, hybrid-orm, sqlserver, sqlite, mysql, postgresql]
parent: MAPPERS
---

# PropertyHandlerMapper

---

A class that is being used to map a property handler into a .NET CLR type or a class property. This class is used as an alternative to the [PropertyHandler](/attribute/propertyhandler) attribute.

Please see the [IPropertyHandler](/interface/ipropertyhandler) for more details about the property handling implementation.

### Methods

Below are the methods available from this class.

- `Add` - adds a property handler mapping on a class or property.
- `Clear` - clears all the existing mappings of the property handlers.
- `Get` - gets the existing mapped property handler of the class or property.
- `Remove` - removes the existing mapped property handler of the class or property.

### Usability

Let us say you had implemented a `DateTime` handler like below.

```csharp
public class DateTimeKindToUtcPropertyHandler : IPropertyHandler<DateTime?, DateTime?>
{
    public DateTime? Get(DateTime? input, ClassProperty property)
    {
        return DateTime.SpecifyKind(input, DateTimeKind.Utc);
    }

    public DateTime? Set(DateTime? input, ClassProperty property)
    {
        return DateTime.SpecifyKind(input.GetValueOrDefault(), DateTimeKind.Unspecified);
    }
}
```

#### Property Level Mapping

To add a property level mapping, simply call the `Add()` method and pass the target property and the instance of the property handler.

```csharp
PropertyHandlerMapper.Add<Customer, DateTimeKindToUtcPropertyHandler>(e => e.DateOfBirth, new DateTimeKindToUtcPropertyHandler(), true);
```

> An exception will be thrown if the mapping is already exists and you passed a `false` value in the `force` argument.

To get the mapping, use the `Get()` method.

```csharp
var propertyHandler = PropertyHandlerMapper.Get<Customer, DateTimeKindToUtcPropertyHandler>(e => e.DateOfBirth);
```

To remove the mapping, use the `Remove()` method.

```csharp
PropertyHandlerMapper.Remove<Customer, DateTimeKindToUtcPropertyHandler>(e => e.DateOfBirth);
```

#### Type Level Mapping

To add a class level mapping, simply call the type-level `Add()` method and pass the target .NET CLR type and the instance of property handler.

```csharp
PropertyHandlerMapper.Add<DateTime, DateTimeKindToUtcPropertyHandler>(new DateTimeKindToUtcPropertyHandler(), true);
```

> An exception will be thrown if the mapping is already exists and you passed a `false` value in the `force` argument.

To get the mapping, use the type-level `Get()` method.

```csharp
var propertyHandler = PropertyHandlerMapper.Get<DateTime, DateTimeKindToUtcPropertyHandler>();
```

To remove the mapping, use the type-level `Remove()` method.

```csharp
PropertyHandlerMapper.Remove<DateTime>();
```