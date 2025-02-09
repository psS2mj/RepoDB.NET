---
layout: default
sidebar: releases
title: Core Package
description: "This page contains the latest information of the releases of RepoDB library."
nav_order: 1
permalink: /release/core
parent: RELEASES
---

# Releases for RepoDB (Core)

---

Please click [here](https://www.nuget.org/packages/RepoDb) to see the actual Nuget package. Otherwise, please click [here](https://www.nuget.org/api/v2/package/RepoDb) to download it.

### RepoDB (v1.12.9)

- Enhancement: Make the value argument of the functional [QueryField](/class/queryfield) objects to `System.Object`. [#926](https://github.com/mikependon/RepoDB/issues/926)


### RepoDB (v1.12.8)

- NETSTANDARD2.0: Added the `Microsoft.Bcl.AsyncInterfaces v5.0.0` package.
- NETSTANDARD2.0: Added the `Microsoft.Bcl.HashCode v1.1.1` package.
- Added the `System.Linq.Async v5.0.0` package.
- Added the `net5.0` as part of the target frameworks.
- Bug: Dynamic insertion via `Dictionary<string, object>` is failing [#791](https://github.com/mikependon/RepoDB/issues/791).
- Bug: `IsDictionaryStringObject()` does not work in F# [#789](https://github.com/mikependon/RepoDB/issues/789).
- Bug: An identify field parameter issue is being thrown when invoking the [MergeAll](/operation/mergeall) operation dynamically [#849](https://github.com/mikependon/RepoDB/issues/849).
- Bug: A SQL syntax issue is being thrown if the [BulkMerge](/operation/bulkmerge) is called with multiple qualifiers [#850](https://github.com/mikependon/RepoDB/issues/850).
- Bug: Output parameters of type varchar gives `Size` exception [#836](https://github.com/mikependon/RepoDB/issues/836).
- Bug: Calls to any operation throws an object `NullReferenceException` if not properly initialized. [#861](https://github.com/mikependon/RepoDB/issues/861).
- Bug: Different lambdas in [QueryAsync](/operation/query) generate the same SQL expression (cache problem) [#782](https://github.com/mikependon/RepoDB/issues/782).
- (Rebuilt Only) Bug: [OrderField](/class/orderfield) ignores MapAttribute [#769](https://github.com/mikependon/RepoDB/issues/769)
- Bug: [OrderField](/class/orderfield) ignores [MapAttribute](/attribute/map) [#769](https://github.com/mikependon/RepoDB/issues/769)
- Bug: Querying by string field fails in VB .Net [#767](https://github.com/mikependon/RepoDB/issues/767)
- Bug: [Insert](/operation/insert) exception since 1.1.3 with mysql... [#765](https://github.com/mikependon/RepoDB/issues/765)
- Enhancement: Added the `Size` property into the [DirectionalQueryField](/class/directionalqueryfield) object.
- Enhancement: Exposed the `Type` property of the [DirectionalQueryField](/class/directionalqueryfield) object.
- Enhancement: Added the `NULL` comparer as part of the qualifiers on the [MergeAll](/operation/mergeall), [UpdateAll](/operation/updateall), [BulkMerge](/operation/bulkmerge) and [BulkUpdate](/operation/bulkupdate) operations.
- Enhancement: Made the [QueryGroup.GetString()](/class/querygroup) method virtual.
- Enhancement: Added the [QueryField.GetString()](/class/queryfield) method (as virtual).
- Enhancement: Make the [DbRepository.CreateConnection()](/class/dbrepository) method virtual. [#856](https://github.com/mikependon/RepoDB/issues/856)
- Enhancement: Made the `CreateConnection()` method of the [BaseRepository](/class/baserepository) class virtual.
- Enhancement: Enhancement: Add an additional property on the [DbField](/class/dbfield) class that handles the DB Provider. [#890](https://github.com/mikependon/RepoDB/issues/890)
- Enhancement: Added the [PropertyValueAttribute](/attribute/propertyvalue) attribute class.
- Enhancement: Create a base class for the Type Map attributes ([NpgsqlTypeMapAttribute](/attribute/npgsqltypemap), [MySqlTypeMapAttribute](/attribute/npgsqltypemap), [MicrosoftSqlServerTypeMapAttribute](/attribute/microsoftsqlservertypemap) and [SystemSqlServerTypeMapAttribute](/attribute/systemsqlservertypemap)) [#873](https://github.com/mikependon/RepoDB/issues/873).
- Enhancement: Add the attribute-based parameter setters for the `DbParameter` object. [#886](https://github.com/mikependon/RepoDB/issues/886)
- Enhancement: Add a mapper for [PropertyValueAttribute](/attribute/propertyvalue) [#887](https://github.com/mikependon/RepoDB/issues/887)
- Enhancement: Added the [DbTypeAttribute](/attribute/dbtype) attribute.
- Enhancement: Added the [DirectionAttribute](/attribute/direction) attribute.
- Enhancement: Added the [IsNullableAttribute](/attribute/isnullable) attribute.
- Enhancement: Added the [NameAttribute](/attribute/name) attribute.
- Enhancement: Added the [PrecisionAttribute](/attribute/precision) attribute.
- Enhancement: Added the [ScaleAttribute](/attribute/scale) attribute.
- Enhancement: Added the [SizeAttribute](/attribute/size) attribute.
- Enhancement: Added the [PropertyValueAttributeMapper](/mappper/propertyvalueattributemapper) class.
- Enhancement: Added the [PropertyValueAttributeCache](/cachers/propertyvalueattributecache) class.
- Enhancement: Added the [PropertyValueAttributeResolver](/resolvers/propertyvalueattributeresolver) class.
- Enhancement: Added the `PropertyValueAttributes()` method on the [FluentMapper](/mapper/fluentmapper) class.
- Enhancement: Introduce the formatters for the [QueryField](/class/queryfield) class [899](https://github.com/mikependon/RepoDB/issues/899))


### RepoDB (v1.12.8-beta5)

- NETSTANDARD2.0: Added the `Microsoft.Bcl.AsyncInterfaces v5.0.0` package.
- NETSTANDARD2.0: Added the `Microsoft.Bcl.HashCode v1.1.1` package.
- Added the `System.Linq.Async v5.0.0` package.
- Added the `net5.0` as part of the target frameworks.
- Bug: Dynamic insertion via `Dictionary<string, object>` is failing [#791](https://github.com/mikependon/RepoDB/issues/791).
- Bug: `IsDictionaryStringObject()` does not work in F# [#789](https://github.com/mikependon/RepoDB/issues/789).
- Bug: An identify field parameter issue is being thrown when invoking the [MergeAll](/operation/mergeall) operation dynamically [#849](https://github.com/mikependon/RepoDB/issues/849).
- Bug: A SQL syntax issue is being thrown if the [BulkMerge](/operation/bulkmerge) is called with multiple qualifiers [#850](https://github.com/mikependon/RepoDB/issues/850).
- Bug: Output parameters of type varchar gives `Size` exception [#836](https://github.com/mikependon/RepoDB/issues/836).
- Bug: Calls to any operation throws an object `NullReferenceException` if not properly initialized. [#861](https://github.com/mikependon/RepoDB/issues/861).
- Enhancement: Added the `Size` property into the [DirectionalQueryField](/class/directionalqueryfield) object.
- Enhancement: Exposed the `Type` property of the [DirectionalQueryField](/class/directionalqueryfield) object.
- Enhancement: Added the `NULL` comparer as part of the qualifiers on the [MergeAll](/operation/mergeall), [UpdateAll](/operation/updateall), [BulkMerge](/operation/bulkmerge) and [BulkUpdate](/operation/bulkupdate) operations.
- Enhancement: Made the [QueryGroup.GetString()](/class/querygroup) method virtual.
- Enhancement: Added the [QueryField.GetString()](/class/queryfield) method (as virtual).
- Enhancement: Make the [DbRepository.CreateConnection()](/class/dbrepository) method virtual. [#856](https://github.com/mikependon/RepoDB/issues/856)
- Enhancement: Made the `CreateConnection()` method of the [BaseRepository](/class/baserepository) class virtual.
- Enhancement: Enhancement: Add an additional property on the [DbField](/class/dbfield) class that handles the DB Provider. [#890](https://github.com/mikependon/RepoDB/issues/890)
- Enhancement: Added the [PropertyValueAttribute](/attribute/propertyvalue) attribute class.
- Enhancement: Create a base class for the Type Map attributes ([NpgsqlTypeMapAttribute](/attribute/npgsqltypemap), [MySqlTypeMapAttribute](/attribute/npgsqltypemap), [MicrosoftSqlServerTypeMapAttribute](/attribute/microsoftsqlservertypemap) and [SystemSqlServerTypeMapAttribute](/attribute/systemsqlservertypemap)) [#873](https://github.com/mikependon/RepoDB/issues/873).
- Enhancement: Add the attribute-based parameter setters for the `DbParameter` object. [#886](https://github.com/mikependon/RepoDB/issues/886)
- Enhancement: Added the [DbTypeAttribute](/attribute/dbtype) attribute.
- Enhancement: Added the [DirectionAttribute](/attribute/direction) attribute.
- Enhancement: Added the [IsNullableAttribute](/attribute/isnullable) attribute.
- Enhancement: Added the [NameAttribute](/attribute/name) attribute.
- Enhancement: Added the [PrecisionAttribute](/attribute/precision) attribute.
- Enhancement: Added the [ScaleAttribute](/attribute/scale) attribute.
- Enhancement: Added the [SizeAttribute](/attribute/size) attribute.
- Enhancement: Added the [PropertyValueAttributeMapper](/mappper/propertyvalueattributemapper) class.
- Enhancement: Added the [PropertyValueAttributeCache](/cachers/propertyvalueattributecache) class.
- Enhancement: Added the [PropertyValueAttributeResolver](/resolvers/propertyvalueattributeresolver) class.
- Enhancement: Added the `PropertyValueAttributes()` method on the [FluentMapper](/mapper/fluentmapper) class.
- Enhancement: Introduce the formatters for the [QueryField](/class/queryfield) class [899](https://github.com/mikependon/RepoDB/issues/899))

### RepoDB (v1.12.8-beta4)

- Bug: Different lambdas in [QueryAsync](/operation/query) generate the same SQL expression (cache problem) [#782](https://github.com/mikependon/RepoDB/issues/782).


### RepoDB (v1.12.8-beta3)

- (Rebuilt Only) Bug: [OrderField](/class/orderfield) ignores MapAttribute [#769](https://github.com/mikependon/RepoDB/issues/769)


### RepoDB (v1.12.8-beta2)

- Bug: [OrderField](/class/orderfield) ignores [MapAttribute](/attribute/map) [#769](https://github.com/mikependon/RepoDB/issues/769)
- Bug: Querying by string field fails in VB .Net [#767](https://github.com/mikependon/RepoDB/issues/767)


### RepoDB (v1.12.8-beta1)

- Bug: [Insert](/operation/insert) exception since 1.1.3 with mysql... [#765](https://github.com/mikependon/RepoDB/issues/765)


### RepoDB (v1.12.7)

- Enhancement: Add a `Reset()` method into the [Parameter](/class/parameter) object. [#709](https://github.com/mikependon/RepoDB/issues/709)
- Enhancement: Add a method `DbParameter` into the [QueryField](/class/queryfield) object. [#711](https://github.com/mikependon/RepoDB/issues/711)
- Enhancement: Revisits the Immutable Classes Instantiation [#753](https://github.com/mikependon/RepoDB/issues/753)
- Bug: Extract function throws exception when using [ExecuteQueryMultiple](/operation/executequerymultiple) [#761](https://github.com/mikependon/RepoDB/issues/761)
- Bug: RepoDb.SqlServer Enum picking up 2 types when upgraded from 1.1.1 -> 1.1.2 [#736](https://github.com/mikependon/RepoDB/issues/736)
- Bug: null reference during fetch [#748](https://github.com/mikependon/RepoDB/issues/748)


### RepoDB (v1.12.6)

- Feature: Support the Output Parameters [#686](https://github.com/mikependon/RepoDB/issues/686) - **NEW**
- Enhancement: Add the `__RepoDb_OrderColumn` at the Batch Operations ([InsertAll](/operation/insertall), [MergeAll](/operation/mergeall)) [#703](https://github.com/mikependon/RepoDB/issues/703)
- Enhancement: Add a `Reset()` method into the [Parameter](/class/parameter) object. [#709](https://github.com/mikependon/RepoDB/issues/709)
- Enhancement: Add the methods named `GetName()` and `GetValue()` in the [QueryField](/class/queryfield) object. [#707](https://github.com/mikependon/RepoDB/issues/707)
- Enhancement: Add a method `DbParameter` into the [QueryField](/class/queryfield) object. [#711](https://github.com/mikependon/RepoDB/issues/711)


### RepoDB (v1.12.5)

- Enhancement: Add the dynamic [ExecuteQueryMultiple](/operation/executequerymultiple) method in the [DbRepository](/class/dbrepository) [#630](https://github.com/mikependon/RepoDB/issues/630)
- Possible bug - Enum with Flag attribute is not correctly handled [#624](https://github.com/mikependon/RepoDB/issues/624)
- [Core] Support `ExpandoObject` in [Insert](/operation/insert) via `TableName`. [#234](https://github.com/mikependon/RepoDB/issues/234)
- [Core] Support `ExpandoObject` in [Merge](/operation/merge) via `TableName`. [#238](https://github.com/mikependon/RepoDB/issues/238)
- [Core] Support `ExpandoObject` in [Update](/operation/update) via `TableName`. [#236](https://github.com/mikependon/RepoDB/issues/236)
- [Core] Support `ExpandoObject` in [InsertAll](/operation/insertall) via `TableName`. [#235](https://github.com/mikependon/RepoDB/issues/235)
- [Core] Support `ExpandoObject` in [MergeAll](/operation/mergeall) via `TableName`. [#239](https://github.com/mikependon/RepoDB/issues/239)
- [Core] Support `ExpandoObject` in [UpdateAll](/operation/updateall) via `TableName`. [#237](https://github.com/mikependon/RepoDB/issues/237)
- Introduce the support of Dynamic and ExpandoObject in [BulkInsert](/operation/bulkinsert). [#243](https://github.com/mikependon/RepoDB/issues/243)
- Enhancement: Support `ExpandoObject` in [BulkInsert](/operation/bulkinsert) [#610](https://github.com/mikependon/RepoDB/issues/610)
- Enhancement: Support `ExpandoObject` in [BulkMerge](/operation/bulkmerge) [#611](https://github.com/mikependon/RepoDB/issues/611)
- Enhancement: Support `ExpandoObject` in [BulkUpdate](/operation/bulkupdate) [#612](https://github.com/mikependon/RepoDB/issues/612)
- Enhancement: Support `ExpandoObject` in [BulkDelete](/operation/bulkdelete) [#613](https://github.com/mikependon/RepoDB/issues/613)
- Bug: Exception is being thrown for the Type level [PropertyHandler](/features/propertyhandlers) for Dynamic Insertion [#628](https://github.com/mikependon/RepoDB/issues/628).
- Added a validation to ensure the type of the `TPropertyHandler` has implemented the [IPropertyHandler](/interface/ipropertyhandler) interface when calling the `Add()` method of the [PropertyHandlerCache](/cacher/propertyhandlercache) object.
- Request: Do not crash if on empty enumerable on bulk operation [#635](https://github.com/mikependon/RepoDB/issues/635).
- Request: Introduce optional caching to [ExecuteScalar](/operation/executescalar) methods. [#648](https://github.com/mikependon/RepoDB/issues/648)
- Enhancement: Add the non-parameterized Truncate operation. [#652](https://github.com/mikependon/RepoDB/issues/652)
- Adhoc: Remove the Initialize method from the [DataEntityDataReader](https://repodb.net/class/dataentitydatareader). [#673](https://github.com/mikependon/RepoDB/issues/673) - this is a breaking changes
- Bug: Query failed when field mapping used on FSharp records. [#662](https://github.com/mikependon/RepoDB/issues/662)
- Bug: [FluentMapper](/mapper/fluentmapper) is not working with Abstract Properties [#666](https://github.com/mikependon/RepoDB/issues/666)
- Question: [IPropertyHandler](/interface/ipropertyhandler) for `Dictionary<string, string>` [#647](https://github.com/mikependon/RepoDB/issues/647)
- Upgraded the `Microsoft.Data.SqlClient` to `v2.1.0`.
- Upgraded the `System.ComponentModel.Annotations` to `v5.0.0`.
- Fixed the related issues found at model-based operation [ExecuteQuery](/operation/executequery) (almost related to [#666](https://github.com/mikependon/RepoDB/issues/666))


### RepoDB (v1.12.5-beta6)

- Fixed the related issues found at model-based operation [ExecuteQuery](/operation/executequery) (almost related to [#666](https://github.com/mikependon/RepoDB/issues/666))


### RepoDB (v1.12.5-beta5)

- Adhoc: Remove the Initialize method from the [DataEntityDataReader](https://repodb.net/class/dataentitydatareader). [#673](https://github.com/mikependon/RepoDB/issues/673) - this is a breaking changes
- Bug: Query failed when field mapping used on FSharp records. [#662](https://github.com/mikependon/RepoDB/issues/662)
- Bug: [FluentMapper](/mapper/fluentmapper) is not working with Abstract Properties [#666](https://github.com/mikependon/RepoDB/issues/666)
- Question: [IPropertyHandler](/interface/ipropertyhandler) for `Dictionary<string, string>` [#647](https://github.com/mikependon/RepoDB/issues/647)
- Upgraded the `Microsoft.Data.SqlClient` to `v2.1.0`.
- Upgraded the `System.ComponentModel.Annotations` to `v5.0.0`.


### RepoDB (v1.12.5-beta4)

- Request: Introduce optional caching to [ExecuteScalar](/operation/executescalar) methods. [#648](https://github.com/mikependon/RepoDB/issues/648)
- Enhancement: Add the non-parameterized Truncate operation. [#652](https://github.com/mikependon/RepoDB/issues/652)

###  RepoDB (v1.12.5-beta3)

- Request: Do not crash if on empty enumerable on bulk operation [#635](https://github.com/mikependon/RepoDB/issues/635).

### RepoDB (v1.12.5-beta2)

- Bug: Exception is being thrown for the Type level [PropertyHandler](/features/propertyhandlers) for Dynamic Insertion [#628](https://github.com/mikependon/RepoDB/issues/628).
- Added a validation to ensure the type of the `TPropertyHandler` has implemented the [IPropertyHandler](/interface/ipropertyhandler) interface when calling the `Add()` method of the [PropertyHandlerCache](/cacher/propertyhandlercache) object.


### RepoDB (v1.12.5-beta1)

- Enhancement: Add the dynamic [ExecuteQueryMultiple](/operation/executequerymultiple) method in the [DbRepository](/class/dbrepository) [#630](https://github.com/mikependon/RepoDB/issues/630)
- Possible bug - Enum with Flag attribute is not correctly handled [#624](https://github.com/mikependon/RepoDB/issues/624)
- [Core] Support `ExpandoObject` in [Insert](/operation/insert) via `TableName`. [#234](https://github.com/mikependon/RepoDB/issues/234)
- [Core] Support `ExpandoObject` in [Merge](/operation/merge) via `TableName`. [#238](https://github.com/mikependon/RepoDB/issues/238)
- [Core] Support `ExpandoObject` in [Update](/operation/update) via `TableName`. [#236](https://github.com/mikependon/RepoDB/issues/236)
- [Core] Support `ExpandoObject` in [InsertAll](/operation/insertall) via `TableName`. [#235](https://github.com/mikependon/RepoDB/issues/235)
- [Core] Support `ExpandoObject` in [MergeAll](/operation/mergeall) via `TableName`. [#239](https://github.com/mikependon/RepoDB/issues/239)
- [Core] Support `ExpandoObject` in [UpdateAll](/operation/updateall) via `TableName`. [#237](https://github.com/mikependon/RepoDB/issues/237)
- Introduce the support of Dynamic and ExpandoObject in [BulkInsert](/operation/bulkinsert). [#243](https://github.com/mikependon/RepoDB/issues/243)
- Enhancement: Support `ExpandoObject` in [BulkInsert](/operation/bulkinsert) [#610](https://github.com/mikependon/RepoDB/issues/610)
- Enhancement: Support `ExpandoObject` in [BulkMerge](/operation/bulkmerge) [#611](https://github.com/mikependon/RepoDB/issues/611)
- Enhancement: Support `ExpandoObject` in [BulkUpdate](/operation/bulkupdate) [#612](https://github.com/mikependon/RepoDB/issues/612)
- Enhancement: Support `ExpandoObject` in [BulkDelete](/operation/bulkdelete) [#613](https://github.com/mikependon/RepoDB/issues/613)


### RepoDB (v1.12.4)

- CancellationToken support? [#343](https://github.com/mikependon/RepoDB/issues/343)


### RepoDB (v1.12.3)

- Bug: Behavior change from previous versions prior v1.12.0 [#602](https://github.com/mikependon/RepoDB/issues/602)
- Bug: Async fetch operations are not using the `DbDataReader.ReadAsync` method (in v1.12.0 to v1.12.2) [#601](https://github.com/mikependon/RepoDB/issues/601)


### RepoDB (v1.12.2)

- Bug: A `NullReferenceException` Is Thrown for NULL Query Expression [#600](https://github.com/mikependon/RepoDB/issues/600)


### RepoDB (v1.12.1)

- Enhancement: New Compiler Possible Collision Problem - Refactor the DbDataReader GetHashCode() Generator [#597](https://github.com/mikependon/RepoDb/issues/597)
- Bug: Unable to share POCOs between different database providers (Sqlite and Postgres) [#595](https://github.com/mikependon/RepoDb/issues/595]


### RepoDB (v1.12.0)

- Complete support to F# programming language as requested by the F# Community. Thank you to [Isaac Abraham](https://twitter.com/isaac_abraham) and [Angel Munoz](https://twitter.com/Daniel_Tuna) for being so collaborative.
- Request: F# - Consider the Anonymous Types in the Query and QueryAll operation [#536](https://github.com/mikependon/RepoDb/issues/536).
- Bug: [QueryAsync](/operation/query) with empty [QueryField](/class/queryfield) list throws SQL exception [#498](https://github.com/mikependon/RepoDb/issues/498).
- Bug: [IPropertyHandler](/interface/ipropertyhandler) not being called [#514](https://github.com/mikependon/RepoDb/issues/514)
- Bug: Property mapping fails with Turkish locale [#502](https://github.com/mikependon/RepoDb/issues/502)
- Bug: Non-query statements are not taking into account SQL Server table hints [#533](https://github.com/mikependon/RepoDb/issues/533).
- Bug: Async methods use synchronous calls [#589](https://github.com/mikependon/RepoDB/issues/589)
- Feature: Introduce the ClassHandler Support [#524](https://github.com/mikependon/RepoDb/issues/524)
- Feature: Support to Enumerable Scalar Values [#538](https://github.com/mikependon/RepoDb/issues/538) - **NEW**
- Request: Completely expose the `fields` argument in the [BatchQuery](/operation/batchquery), [Query](/operation/query), [Insert](/operation/insert), [Merge](/operation/merge) and [Update](/operation/update) operations (and all its Batch operations). [#523](https://github.com/mikependon/RepoDb/issues/523)
- Request: Add caching for [ExecuteQuery](/operation/executequery) and [ExecuteQuery&lt;TEntity&gt;](/operation/executequery) [#522](https://github.com/mikependon/RepoDb/issues/522)
- Request: Adds an overloaded method for [QueryAll&lt;TEntity&gt;](/operation/queryall) operation that takes the `tableName` parameter. [#521](https://github.com/mikependon/RepoDb/issues/521) - **BREAKING**
- Request: Add caching for [ExecuteQuery](/operation/executequery) and [ExecuteQuery&lt;TEntity&gt;](/operation/executequery) [#522](https://github.com/mikependon/RepoDb/issues/522)
- Request: Add the 'isMoveToNextResult' argument to the [QueryMultipleExtractor](/class/querymultipleextractor) (Extract and Scalar) methods [#591](https://github.com/mikependon/RepoDB/issues/591)
- Request: Support the Immutable Entities [#465](https://github.com/mikependon/RepoDb/issues/465)
- Question: Question on how to properly configure type mapping for FSharp Option types [#483](https://github.com/mikependon/RepoDb/issues/483)
- Question: Specific Columns in `Query<TEntity>` [#545](https://github.com/mikependon/RepoDb/issues/545)
- Enhancement: Use the `Identity` field if the `Primary` field is not available during the [Query](/operation/query), [Delete](/operation/delete) and [Update](/operation/update) operations.
- Refactoring: Enhance the coding in the Core Compiler [#479](https://github.com/mikependon/RepoDb/issues/479). **BREAKING**
- Enhancement: Complete support to the Fluent named-based operation [#499](https://github.com/mikependon/RepoDb/issues/499).
- Enhancement: Replaces the usage of `IsNullOrEmpty` to `IsNullOrWhiteSpace`.
- Enhancement: Replaces the usage of `ToLower()` to `ToLowerInvariant()`.
- Enhancement: Replaces the usage of string equality to `string.Equals(value1, value2, StringComparer.OrdinalIgnoreCase)`.
- Enhancement: Added the `Async` methods in the compiler. [#482](https://github.com/mikependon/RepoDb/issues/482) [#477](https://github.com/mikependon/RepoDb/issues/477)
- Enhancement: Add the dynamic [ExecuteQuery](/operation/executequery) method in the [DbRepository](/class/dbrepository). [#517](https://github.com/mikependon/RepoDb/issues/517)
- Enhancement: Renamed the `whereOrPrimaryKey` argument to `what` to extend the support to both (data entity object, dynamic/object expression, primary key and identity key), to further support the `F#` community. **BREAKING**
- Enhancement: Updated the [QueryGroup.Parse()](/class/querygroup) method to be an argument-typed-based method.
- Enhancement: Refactored and optimized the `Parse` method of the [QueryField](/class/queryfield) and [QueryGroup](/class/querygroup) objects.
- Enhancement: Refactor the Table-Based Calls to return `IEnumerable<ExpandoObject>` instead of `IEnumerable<dynamics>`. [#540](https://github.com/mikependon/RepoDb/issues/540)
- Enhancement: Consider supporting the execution of the TVP in SQL Server. [#566](https://github.com/mikependon/RepoDb/issues/566)
- Enhancement: Support for returning `IDictionary<string, object>` instead of ExpandoObject. [#537](https://github.com/mikependon/RepoDb/issues/537)
- Enhancement: Re-assess if the `IsAssignableFrom` can be used over the customized `IsInterfacedTo`. [#469](https://github.com/mikependon/RepoDb/issues/469)
- Enhancement: Handle the Exception Handling of the Serialization/Deserialization process of the [ClassHandler](/feature/classhanders) that is connected to a different Data Entity [#539](https://github.com/mikependon/RepoDb/issues/539)
- Refactoring: Make all the `cacheItemExpiration` arguments nullable. **BREAKING**
- Refactoring: Make the [BaseRepository](/class/dbrepository) and [DbRepository](/class/dbrepository) objects `CacheItemExpiration` property nullable.
- Refactoring: Make the [CacheItem](/class/cacheitem) object `CacheItemExpiration` property nullable.
- Test: Added the Integration Tests for the `NonKeyedTable`.
- Integration Tests: Added more Integration Tests for the `DbType` Map Attribute (includes SQL Server, PostgreSQL and MySQL).
- Added the `KeyFieldNotFoundException`, `MissingQualifierFieldsException` and the `IdentityFieldNotFoundException`.
- Added the `<TEntity>(TableName)` methods to the [BatchQuery](/operation/batchquery) operation.
- Added the `<TEntity>(TableName)` methods to the [Query](/operation/query) and [QueryAll](/operation/queryall) operations.
- Added the `<TEntity>(TableName)` methods to the [Delete](/operation/delete) and [DeleteAll](/operation/deleteall operations).
- Added the `<TEntity>(TableName)` methods to the [Insert](/operation/insert) and [InsertAll](/operation/insertall) operations.
- Added the `<TEntity>(TableName)` methods to the [Merge](/operation/merge) and [MergeAll](/operation/mergeall) operations.
- Added the `<TEntity>(TableName)` methods to the [Update](/operation/update) and [UpdateAll](/operation/updateall) operations.
- Added the `<TEntity, TResult>` methods to the [Average](/operation/average) and [AverageAll](/operation/averageall operations).
- Added the `<TEntity, TResult>` methods to the [Max](/operation/max) and [MaxAll](/operation/maxall operations).
- Added the `<TEntity, TResult>` methods to the [Min](/operation/min) and [MinAll](/operation/minall operations).
- Added the `<TEntity, TResult>` methods to the [Sum](/operation/sum) and [SumAll](/operation/sumall operations).
- Added the execution context provider internal classes for the [Insert](/operation/insert), [Merge](/operation/merge), [Update](/operation/update), internal class for the [InsertAll](/operation/insertall), [MergeAll](/operation/mergeall) and [UpdateAll](/operation/updateall)operations.


### RepoDB (v1.12.0-beta4)

- Enhancement: Consider supporting the execution of the TVP in SQL Server. [#566](https://github.com/mikependon/RepoDb/issues/566)
- Integration Tests: Added more Integration Tests for the `DbType` Map Attribute (includes SQL Server, PostgreSQL and MySQL).


### RepoDB (v1.12.0-beta3)

- Enhancement: Refactor the Table-Based Calls to return `IEnumerable<ExpandoObject>` instead of `IEnumerable<dynamics>`. [#540](https://github.com/mikependon/RepoDb/issues/540)
- Enhancement: Support for returning `IDictionary<string, object>` instead of ExpandoObject. [#537](https://github.com/mikependon/RepoDb/issues/537)
- Enhancement: Re-assess if the `IsAssignableFrom` can be used over the customized `IsInterfacedTo`. [#469](https://github.com/mikependon/RepoDb/issues/469)
- Enhancement: Handle the Exception Handling of the Serialization/Deserialization process of the [ClassHandler](/feature/classhanders) that is connected to a different Data Entity [#539](https://github.com/mikependon/RepoDb/issues/539)
- Feature: Support to Enumerable Scalar Values [#538](https://github.com/mikependon/RepoDb/issues/538) - **NEW**


### RepoDB (v1.12.0-beta2)

- Enhancement: Updated the [QueryGroup.Parse()](/class/querygroup) method to be an argument-typed-based method.
- Enhancement: Refactored and optimized the `Parse` method of the [QueryField](/class/queryfield) and [QueryGroup](/class/querygroup) objects.
- Bug: Non-query statements are not taking into account SQL Server table hints [#533](https://github.com/mikependon/RepoDb/issues/533).
- Request: F# - Consider the Anonymous Types in the Query and QueryAll operation [#536](https://github.com/mikependon/RepoDb/issues/536).
- Question: Specific Columns in `Query<TEntity>` [#545](https://github.com/mikependon/RepoDb/issues/545)


### RepoDB (v1.12.0-beta1)

- Complete support to F# programming language as requested by the F# Community. Thank you to [Isaac Abraham](https://twitter.com/isaac_abraham) and [Angel Munoz](https://twitter.com/Daniel_Tuna) for being so collaborative.
- Bug: [QueryAsync](/operation/query) with empty [QueryField](/class/queryfield) list throws SQL exception [#498](https://github.com/mikependon/RepoDb/issues/498).
- Bug: [IPropertyHandler](/interface/ipropertyhandler) not being called [#514](https://github.com/mikependon/RepoDb/issues/514)
- Bug: Property mapping fails with Turkish locale [#502](https://github.com/mikependon/RepoDb/issues/502)
- Feature: Introduce the ClassHandler Support [#524](https://github.com/mikependon/RepoDb/issues/524)
- Request: Completely expose the `fields` argument in the [BatchQuery](/operation/batchquery), [Query](/operation/query), [Insert](/operation/insert), [Merge](/operation/merge) and [Update](/operation/update) operations (and all its Batch operations). [#523](https://github.com/mikependon/RepoDb/issues/523)
- Request: Add caching for [ExecuteQuery](/operation/executequery) and [ExecuteQuery&lt;TEntity&gt;](/operation/executequery) [#522](https://github.com/mikependon/RepoDb/issues/522)
- Request: Adds an overloaded method for [QueryAll&lt;TEntity&gt;](/operation/queryall) operation that takes the `tableName` parameter. [#521](https://github.com/mikependon/RepoDb/issues/521) - **BREAKING**
- Request: Add caching for [ExecuteQuery](/operation/executequery) and [ExecuteQuery&lt;TEntity&gt;](/operation/executequery) [#522](https://github.com/mikependon/RepoDb/issues/522)
- Request: Support the Immutable Entities [#465](https://github.com/mikependon/RepoDb/issues/465)
- Question: Question on how to properly configure type mapping for FSharp Option types [#483](https://github.com/mikependon/RepoDb/issues/483)
- Enhancement: Use the `Identity` field if the `Primary` field is not available during the [Query](/operation/query), [Delete](/operation/delete) and [Update](/operation/update) operations.
- Refactoring: Enhance the coding in the Core Compiler [#479](https://github.com/mikependon/RepoDb/issues/479). **BREAKING**
- Enhancement: Complete support to the Fluent named-based operation [#499](https://github.com/mikependon/RepoDb/issues/499).
- Enhancement: Replaces the usage of `IsNullOrEmpty` to `IsNullOrWhiteSpace`.
- Enhancement: Replaces the usage of `ToLower()` to `ToLowerInvariant()`.
- Enhancement: Replaces the usage of string equality to `string.Equals(value1, value2, StringComparer.OrdinalIgnoreCase)`.
- Enhancement: Added the `Async` methods in the compiler. [#482](https://github.com/mikependon/RepoDb/issues/482) [#477](https://github.com/mikependon/RepoDb/issues/477)
- Enhancement: Add the dynamic [ExecuteQuery](/operation/executequery) method in the [DbRepository](/class/dbrepository). [#517](https://github.com/mikependon/RepoDb/issues/517)
- Enhancement: Renamed the `whereOrPrimaryKey` argument to `what` to extend the support to both (data entity object, dynamic/object expression, primary key and identity key), to further support the `F#` community. **BREAKING**
- Refactoring: Make all the `cacheItemExpiration` arguments nullable. **BREAKING**
- Refactoring: Make the [BaseRepository](/class/dbrepository) and [DbRepository](/class/dbrepository) objects `CacheItemExpiration` property nullable.
- Refactoring: Make the [CacheItem](/class/cacheitem) object `CacheItemExpiration` property nullable.
- Test: Added the Integration Tests for the `NonKeyedTable`.
- Added the `KeyFieldNotFoundException`, `MissingQualifierFieldsException` and the `IdentityFieldNotFoundException`.
- Added the `<TEntity>(TableName)` methods to the [BatchQuery](/operation/batchquery) operation.
- Added the `<TEntity>(TableName)` methods to the [Query](/operation/query) and [QueryAll](/operation/queryall) operations.
- Added the `<TEntity>(TableName)` methods to the [Delete](/operation/delete) and [DeleteAll](/operation/deleteall operations).
- Added the `<TEntity>(TableName)` methods to the [Insert](/operation/insert) and [InsertAll](/operation/insertall) operations.
- Added the `<TEntity>(TableName)` methods to the [Merge](/operation/merge) and [MergeAll](/operation/mergeall) operations.
- Added the `<TEntity>(TableName)` methods to the [Update](/operation/update) and [UpdateAll](/operation/updateall) operations.
- Added the `<TEntity, TResult>` methods to the [Average](/operation/average) and [AverageAll](/operation/averageall operations).
- Added the `<TEntity, TResult>` methods to the [Max](/operation/max) and [MaxAll](/operation/maxall operations).
- Added the `<TEntity, TResult>` methods to the [Min](/operation/min) and [MinAll](/operation/minall operations).
- Added the `<TEntity, TResult>` methods to the [Sum](/operation/sum) and [SumAll](/operation/sumall operations).
- Added the execution context provider internal classes for the [Insert](/operation/insert), [Merge](/operation/merge), [Update](/operation/update), internal class for the [InsertAll](/operation/insertall), [MergeAll](/operation/mergeall) and [UpdateAll](/operation/updateall)operations.


### RepoDB (v1.11.6)

- Code optimizations and XML comments refactoring.
- Bug: `NullReferenceException` occurs when [InsertAllAsync](/operation/insertall) is executed on Connection that belongs to `TransactionScope`. [#490](https://github.com/mikependon/RepoDb/issues/490)
- Bug: Typed `UpdateAsync` fails for composite key table [#493](https://github.com/mikependon/RepoDb/issues/493)
- Bug: RepoDB does not seem to work for SQL Server tables with dot in the name [#492](https://github.com/mikependon/RepoDb/issues/492)
- Enhancement: Remove the `SchemaSeparator` property from the `IDbSetting` interface [#475](https://github.com/mikependon/RepoDb/issues/475)
- Enhancement: Using async `DbFieldCache` [#481](https://github.com/mikependon/RepoDb/issues/481)
- Enhancement: Add a `SessionId` property in the [TraceLog](/class/tracelog) class. [#484](https://github.com/mikependon/RepoDb/issues/484)
- Enhancement: Refactor the usage of `Count()` and `ElementAt()`.
- Request: Enable the Enumerable when calling the operations with `IN` operation. [#495](https://github.com/mikependon/RepoDb/issues/495)
- Obsolete: Completely removed the `PropertyTypeHandlerMapper` class.
- Obsolete: Completely removed the `TypeMapper.Map()` method.
- Obsolete: Completely removed the `TypeMapper.Unmap()` method.
- Obsolete: Completely removed the `TypeMapper.ConversionType` property.
- Added some micro optimizations #476
- Added a `DataEntityReader.Connection` property.
- Added a `DataEntityReader.Transaction` property.
- Added a `DataEntityReader.Initialize` method
- Added a `DataEntityReader.InitializeAsync()` method.


### RepoDB (v1.11.5)

- Fixed the problem when installing the library in .NET Framework `4.7.x`.
- Restored the referenced `System.ComponentModel.Annotations` package to `v4.7.0`.


### RepoDB (v1.11.4)

- Bug: Table schema is ignored for the identical table names [#456](https://github.com/mikependon/RepoDb/issues/456)
- Bug: Regression Issue [#457](https://github.com/mikependon/RepoDb/issues/457)
- Bug: Table Attribute Potential Bug [#464](https://github.com/mikependon/RepoDb/issues/464)
- Bug?: SqlException: Incorrect syntax near ')' [#463](https://github.com/mikependon/RepoDb/issues/463)
- Updated the XML documentations of the `cache` argument for both [Query](/operation/query) and [QueryAll](/operation/queryall) operations.


### RepoDB (v1.11.4-beta3)

- Bug: Table schema is ignored for the identical table names [#456](https://github.com/mikependon/RepoDb/issues/456)
- Bug: Regression Issue [#457](https://github.com/mikependon/RepoDb/issues/457)
- Bug: Table Attribute Potential Bug [#464](https://github.com/mikependon/RepoDb/issues/464)
- Bug?: SqlException: Incorrect syntax near ')' [#463](https://github.com/mikependon/RepoDb/issues/463)
- Updated the XML documentations of the `cache` argument for both [Query](/operation/query) and [QueryAll](/operation/queryall) operations.


### RepoDB (v1.11.4-beta2)

- Community Request: Additional fix for [#457](https://github.com/mikependon/RepoDb/issues/457)


### RepoDB (v1.11.4-beta1)

- Bug: Regression Issue [#457](https://github.com/mikependon/RepoDb/issues/457)


### RepoDB (v1.11.3)

- Community Request: Enhancement: Enable Field class to Parse the Expression for Multiple Properties [#453](https://github.com/mikependon/RepoDb/issues/453)
- Enhancement: Set the return type `Field.Parse<T>()` to `IEnumerable<Field>` (instead of [Field](/class/field)).
- Added more Unit Tests on [Field](/class/field) class parsing method.
- Removed the `BeforeBulkInsert` and `AfterBulkInsert` from the [ITrace](/interface/itrace) interface.
- Made the [CancellableTraceLog](/class/cancellabletracelog) class non-sealed, and also, exposed the constructor.
- Added an overload method for the [Merge](/operation/merge), [MergeAll](/operation/mergeall) and [UpdateAll](/operation/updateall) operations that accepts the `expression` for the `qualifiers` argument.


### RepoDB (v1.11.2)

- Bug: [SQL Server 2019] RepoDB truncates strings of "Text" types [#444](https://github.com/mikependon/RepoDb/issues/444)
- Request: [SQL Server] Provide better exception message when table mapping is wrong [#443](https://github.com/mikependon/RepoDb/issues/443)


### RepoDB (v1.11.1)

- Bug: The property handler mapping via [FluentMapper](/mapper/fluentmapper) or [PropertyHandlerMapper](/mapper/propertyhandlermapper) is not being triggered. [#438](https://github.com/mikependon/RepoDb/issues/438)
- Requests: Support for Table attribute [#360](https://github.com/mikependon/RepoDb/issues/360)
- Optimization: Transfer the logic of [ClassProperty](/class/classproperty) into various mappers.
- Optimization: Added an `IResolver` interface that does not require an `input` argument.
- Bug: The property handler mapping via [FluentMapper](/mapper/fluentmapper) or [PropertyHandlerMapper](/mapper/propertyhandlermapper) is not being triggered. [#438](https://github.com/mikependon/RepoDb/issues/438)
- Bug: No coercion operator is defined between types `System.String` and `System.Guid`. [#437](https://github.com/mikependon/RepoDb/issues/437)
- Added an extensive Integration Tests for Property Handler Implicit Mapping.
- Added an extensive Unit and Integration Tests for `Key`, `Column` and `Table` attributes support. [#435](https://github.com/mikependon/RepoDb/issues/435)
- Added more Unit Tests for `Key/Primary` and `Table/Column/Map` collisions. [#435](https://github.com/mikependon/RepoDb/issues/435)
- Added the `GetTypeMapAttribute()`, `GetPropertyHandler()`, `GetPropertyHandlerAttribute()` methods in the [ClassProperty](/class/classproperty) class.
- Added the `PrimaryResolver` to resolve the primary [ClassProperty](/class/classproperty) of the data entity type.
- Added the `IdentityResolver` to resolve the identity [ClassProperty](/class/classproperty) of the data entity type.
- Added the `ClassMappedNameResolver` to resolve the database object name mapping of the data entity type.
- Added the `PropertyMappedNameResolver` to resolve the cached column name mappings of the property.
- Added both the `TypeMapPropertyLevelResolver` and `TypeMapTypeLevelResolver` classes to resolve the equivalent `DbType` object of both the property and .NET CLR type.
- Added both the `PropertyHandlerPropertyLevelResolver` and `PropertyHandlerTypeLevelResolver` classes to resolve the equivalent property handler of both the property and .NET CLR type.
- Added the `entityType` argument in the `DbCommandExtensions.CreateParameters()` method.


### RepoDB (v1.11.1-beta3)

- Added the `entityType` argument in the `DbCommandExtensions.CreateParameters()` method.


### RepoDB (v1.11.1-beta2)

- Requests: Support for Table attribute [#360](https://github.com/mikependon/RepoDb/issues/360)
- Bug: The property handler mapping via [FluentMapper](/mapper/fluentmapper) or [PropertyHandlerMapper](/mapper/propertyhandlermapper) is not being triggered. [#438](https://github.com/mikependon/RepoDb/issues/438)
- Bug: No coercion operator is defined between types `System.String` and `System.Guid`. [#437](https://github.com/mikependon/RepoDb/issues/437)
- Added an extensive Unit and Integration Tests for `Key`, `Column` and `Table` attributes support. [#435](https://github.com/mikependon/RepoDb/issues/435)
- Added more Unit Tests for `Key/Primary` and `Table/Column/Map` collisions. [#435](https://github.com/mikependon/RepoDb/issues/435)
- Added the `GetTypeMapAttribute()`, `GetPropertyHandler()`, `GetPropertyHandlerAttribute()` methods in the [ClassProperty](/class/classproperty) class.
- Optimization: Transfer the logic of [ClassProperty](/class/classproperty) into various mappers.
- Optimization: Added an `IResolver` interface that does not require an `input` argument.
- Added the `PrimaryResolver` to resolve the primary [ClassProperty](/class/classproperty) of the data entity type.
- Added the `IdentityResolver` to resolve the identity [ClassProperty](/class/classproperty) of the data entity type.
- Added the `ClassMappedNameResolver` to resolve the database object name mapping of the data entity type.
- Added the `PropertyMappedNameResolver` to resolve the cached column name mappings of the property.
- Added both the `TypeMapPropertyLevelResolver` and `TypeMapTypeLevelResolver` classes to resolve the equivalent `DbType` object of both the property and .NET CLR type.
- Added both the `PropertyHandlerPropertyLevelResolver` and `PropertyHandlerTypeLevelResolver` classes to resolve the equivalent property handler of both the property and .NET CLR type.


### RepoDB (v1.11.1-beta1)

- Bug: The property handler mapping via [FluentMapper](/mapper/fluentmapper) or [PropertyHandlerMapper](/mapper/propertyhandlermapper) is not being triggered. [#438](https://github.com/mikependon/RepoDb/issues/438)
- Added an extensive Integration Tests for Property Handler Implicit Mapping.


### RepoDB (v1.11.0)

- Enhancement: Use lambda to define property handlers within DTO constructor. [#421](https://github.com/mikependon/RepoDb/issues/421)
- Enhancement: Consider Mapping class [#415](https://github.com/mikependon/RepoDb/issues/415)
- Request: Allow custom implementation without attribute [#399](https://github.com/mikependon/RepoDb/issues/399)
- Question: ColumnName Resolver [#387](https://github.com/mikependon/RepoDb/issues/387)
- Added the [FluentMapper](/mapper/fluentmapper), [EntityMapFluentDefinition](/class/entitymapfluentdefinition) and [TypeMapFluentDefinition](/class/typemapfluentdefinition).
- Added the expression-based invocation in the `Add()`, `Get()` and `Remove()` methods of the [DbHelperMapper](/mapper/dbhelpermapper), [DbSettingMapper](/mapper/dbsettingmapper) and [StatementBuilderMapper](/mapper/statementbuildermapper) classes.
- Refactor the `Parse()` method of the `OrderField` and [Field](/class/field) classes.
- Refactor the `GetProperty()` method of the `ExpressionExtension` class to solve the problem in the mappers.
- Added the [PropertyHandlerCache](/cacher/propertyhandlercache) class.
- Added the methods `Add()`, `Remove()` and `Get()` at the `PropertyHandlerMapper` class to cater the property level mapping.
- Added a class named [PropertyHandlerMapper](/mapper/propertyhandlermapper) as a replacement of `PropertyTypeHandlerMapper` class.
- Added more Integration Tests on the implicit mappings feature.
- Added Unit and Integration Tests for the fluent mappings.
- Added the `ObseleteAttribute` attribute at the `PropertyTypeHandlerMapper` class.
- Removed the `throwException` arguments in the `Remove()` method of the [DbHelperMapper](/mapper/dbhelpermapper), [DbSettingMapper](/mapper/dbsettingmapper) and [StatementBuilderMapper](/mapper/statementbuildermapper) classes.
- Removed the return value of the `Remove()` method of the [DbHelperMapper](/mapper/dbhelpermapper), [DbSettingMapper](/mapper/dbsettingmapper) and [StatementBuilderMapper](/mapper/statementbuildermapper).
- Rename all the mappers `Flush()` method into `Clear()`.


### RepoDB (v1.11.0-beta4)

- Refactor: Renamed the argument `objectName` to `databaseObjectName` of [ClassMapper](/mapper/classmapper) class.
- Added: Added the method `Get()` via `propertyName`, [Field](/class/field) and Linq expression at [PropertyCache](/cache/propertycache) class.
- Refactor: Hide the method `Get()` via [ClassProperty](/class/classproperty) at [ClassExpression](/class/classexpression) class.
- Removed: Removed the method `Get()` via [DbField](/class/dbfield) at [ClassExpression](/class/classexpression) class.


#### All packages are affected:
- Bug: (Direct Reports) Fixed the issue at `DeleteAll()` via primary keys if the items is beyond `2100`.
- Performance: Reverted the value of `Constant.DefaultBatchOperationSize` into `10`.


### RepoDB (v1.11.0-beta3)

- Issue in the [PrimaryMapper](/mapper/primarymapper) and [IdentityMapper](/mapper/identitymapper) for the interface property collision reported by the user in RepoDB v1.11.0-beta2.
- Removed the exposure of the `PropertyInfo` and [ClassProperty](/class/classproperty) in [PropertyHandlerCache](/cacher/propertyhandlercache), [TypeMapCache](/cacher/typemapcache), [PropertyHandlerMapper](/mapper/propertyhandlermapper) and [TypeMapper](/class/typemapper) classes.
- Removed the `Add()`, `Get`, `Remove()` methods of the [PropertyMapper](/mapper/propertymapper) with both `PropertyInfo` and [ClassProperty](/class/classproperty) arguments.


### RepoDB (v1.11.0-beta2)

- Removed the return value of the `Remove()` method of the [DbHelperMapper](/mapper/dbhelpermapper), [DbSettingMapper](/mapper/dbsettingmapper) and [StatementBuilderMapper](/mapper/statementbuildermapper).
- Added the expression-based invocation in the `Add()`, `Get()` and `Remove()` methods of the [DbHelperMapper](/mapper/dbhelpermapper), [DbSettingMapper](/mapper/dbsettingmapper) and [StatementBuilderMapper](/mapper/statementbuildermapper) classes.
- Removed the `throwException` arguments in the `Remove()` method of the [DbHelperMapper](/mapper/dbhelpermapper), [DbSettingMapper](/mapper/dbsettingmapper) and [StatementBuilderMapper](/mapper/statementbuildermapper) classes.
- Refactor the `Parse()` method of the `OrderField` and [Field](/class/field) classes.
- Refactor the `GetProperty()` method of the `ExpressionExtension` class to solve the problem in the mappers.
- Added more Integration Tests on the implicit mappings feature.


### RepoDB (v1.11.0-beta1)

- Added the [PropertyHandlerCache](/cacher/propertyhandlercache) class.
- Added the methods `Add()`, `Remove()` and `Get()` at the `PropertyHandlerMapper` class to cater the property level mapping.
- Added a class named [PropertyHandlerMapper](/mapper/propertyhandlermapper) as a replacement of [PropertyHandlerMapper](/mapper/propertyhandlermapper) class.
- Added the `ObseleteAttribute` attribute at the [PropertyHandlerMapper](/mapper/propertyhandlermapper) class.
- Rename all the mappers `Flush()` method into `Clear()`.

### RepoDB (v1.11.0-alpha1):

- Added the [ClassMapper](/mapper/classmapper), [PropertyMapper](/mapper/propertymapper), [PrimaryMapper](/mapper/primarymapper), [IdentityMapper](/mapper/identitymapper) and [TypeMapCache](/cacher/typemapcache) classes.
- Added the `Add<T>`, `Get<T>` and `Remove<T>` methods in the [TypeMapper](/mapper/typemapper) class.
- Made the `Map` method of the [TypeMapper](/mapper/typemapper) class obsolete.
- Made the `Unmap` method of the [TypeMapper](/mapper/typemapper) class obsolete.
- Added the `PropertyNotFoundException` exception class.
- Added a method named `GenerateCustomizedHashCode` in the `PropertyExtension` class.
- Added the [Converter](/class/converter) class to handle the [TypeMapper.Conversion](/class/typemapper) property.
- Removed the internal class named `ObjectConverter`. All methods has been placed to a newly created class named [Converter](/class/converter).
- Made the `Get(Type)` method of [ClassMappedNameCache](/cache/classmappednamecache] class exposed as `public`.
- Added more thorough Unit Tests for `Class`, `Property`, `Primary`, `Identity` and `Type` mappings (both [Cachers](https://github.com/mikependon/RepoDb/tree/master/RepoDb.Core/RepoDb.Tests/RepoDb.UnitTests/Caches) and [Mappers](https://github.com/mikependon/RepoDb/tree/master/RepoDb.Core/RepoDb.Tests/RepoDb.UnitTests/Mappers)).


### RepoDB (v1.10.11):

- Implemented the [IExpirable](/interface/iexpirable) into [CacheItem](/class/cacheitem).
- Added a `TEntity` generic type in the [CacheItem](/class/cacheitem) properties.
- Added the [IExpirable](/interface/iexpirable) interface.
- Added the [CacheItem.CacheItemExpiration](/class/cacheitem) property.
- Added the `ConverterNotFoundException` class.
- At the [CancellableTraceLog.Cancel()](/class/cancellabletracelog) method, the `throwException` argument has been defaulted the `true`.
- Enhancement: Ensure that [PropertyHandler](/interface/ipropertyhandler)(s) must ignore the [TypeMapper](/mapper/typemapper) automatic conversion and also `Enum` handlers. [#412](https://github.com/mikependon/RepoDb/issues/412)
- Enhancement: Make the [Constant.DefaultBatchOperationSize](/class/constant) property value to `10`. Targeting the bulk operations (i.e.: [BulkInsert](/operation/bulkinsert), [BulkDelete](/operation/bulkdelete), [BulkMerge](/operation/bulkinsert) and [BulkUpdate](/operation/bulkupdate)) default batch-size.
- Bug: UnaryExpression: Add support for `&&` and `||` operators in the expressions [398](https://github.com/mikependon/RepoDb/issues/#398)
- Bug: Enum Bug [#400](https://github.com/mikependon/RepoDb/issues/400)
- Bug: Enum Bug on Null value on [Insert](/operation/insert). [#401](https://github.com/mikependon/RepoDb/issues/401)
- Bug: [PropertyHandler](/interface/ipropertyhandler) for Nullable Enum [#402](https://github.com/mikependon/RepoDb/issues/402)
- Bug: Calling to [DeleteAll](/operation/deleteall) operation with the list of `PrimaryKeys` and `Transaction` object is failing. Reported by Christian Franck. [#404](https://github.com/mikependon/RepoDb/issues/404).


### RepoDB (v1.10.11-beta3):

- Implemented the [IExpirable](/interface/iexpirable) into [CacheItem](/class/cacheitem).
- Added a `TEntity` generic type in the [CacheItem](/class/cacheitem) properties.
- Added the [IExpirable](/interface/iexpirable) interface.
- Added the [CacheItem.CacheItemExpiration](/class/cacheitem) property.
- Bug: Enum Bug on Null value on [Insert](/operation/insert). [#401](https://github.com/mikependon/RepoDb/issues/401)
- Added the `ConverterNotFoundException` class.
- Enhancement: Ensure that [PropertyHandler](/interface/ipropertyhandler)(s) must ignore the [TypeMapper](/mapper/typemapper) automatic conversion and also `Enum` handlers. [#412](https://github.com/mikependon/RepoDb/issues/412)
- Enhancement: Make the [Constant.DefaultBatchOperationSize](/class/constant) property value to `10`. Targeting the bulk operations (i.e.: [BulkInsert](/operation/bulkinsert), [BulkDelete](/operation/bulkdelete), [BulkMerge](/operation/bulkinsert) and [BulkUpdate](/operation/bulkupdate)) default batch-size.


### RepoDB (v1.10.11-beta2):

- Bug: Enum Bug [#400](https://github.com/mikependon/RepoDb/issues/400)
- Bug; [PropertyHandler](/interface/ipropertyhandler) for Nullable Enum [#402](https://github.com/mikependon/RepoDb/issues/402)


### RepoDB (v1.10.11-beta1):

- At the [CancellableTraceLog.Cancel()](/class/cancellabletracelog) method, the `throwException` argument has been defaulted the `true`.
- Bug: Calling to [DeleteAll](/operation/deleteall) operation with the list of `PrimaryKeys` and `Transaction` object is failing. Reported by Christian Franck. [#404](https://github.com/mikependon/RepoDb/issues/404).


### RepoDB (v1.10.10)

- Features: Full support to Bulk Operations ([BulkDelete](/operation/bulkdelete), [BulkInsert](/operation/bulkinsert), [BulkMerge](/operation/bulkmerge) and [BulkUpdate](/operation/bulkupdate)).
- Enhancement: `AsFieldsAsAliasFields` - added left and right aliases.
- Enhancement: XML Documentation updates for the SQL statement Builders.
- Enhancement: Add a `Type` extended method named `IsNullable`.
- Bug: Solve the intermittent `NullReferenceException` when calling the Batch Operations (i.e.: [InsertAll](/operation/insertall), [MergeAll](/operation/mergeall), [UpdateAll](/operation/updateall)). [#392](https://github.com/mikependon/RepoDb/issues/392)
- Bug: The property handlers mapped via `PropertyHandlerMapper` is failing if both `NULLABLE` and `NON-NULLABLE` property types are present in the class. [#394](https://github.com/mikependon/RepoDb/issues/394)


### RepoDB (v1.10.10-beta1)

- Full support to Bulk Operations ([BulkDelete](/operation/bulkdelete), [BulkInsert](/operation/bulkinsert), [BulkMerge](/operation/bulkmerge) and [BulkUpdate](/operation/bulkupdate)).
- `AsFieldsAsAliasFields` - added left and right aliases.
- XML Documentation updates for the SQL statement Builders.


### RepoDB (v1.10.9)

- Enhancement: Compiler changes for `ClassProperty.GetDbType()` calls.
- Feature: Support for `SqlServer.SqlDbType` (Microsoft and System), `PostgreSql.NpgsqlDbType` [#390](https://github.com/mikependon/RepoDb/issues/390) and `MySql.MySqlDbType`.


### RepoDB (v1.10.8)

- Bug: `InvalidCastException` Converting `Enums` to `Strings` in Postgres [#388](https://github.com/mikependon/RepoDb/issues/388)


### RepoDB (v1.10.7)

- Enhancement: Separate the `Bulk` operations into a separate Solution and Nuget Package. [#385](https://github.com/mikependon/RepoDb/issues/385)
- Enhancement: Separete all `SqlServer` related stuffs to a different library named `RepoDb.SqlServer`. [#282](https://github.com/mikependon/RepoDb/issues/282)
- Enhancement: Remove the support to `System.Data.SqlClient` in the `RepoDb.Core`. [#386](https://github.com/mikependon/RepoDb/issues/386)


### RepoDB (v1.10.6)

- Added the class property as an argument context in the `Get()` and `Set()`  method.
- Exposed the underlying `DbRepository` property at the ``BaseRepository`` object.


### RepoDB (v1.10.5)

#### Highlights

- Support: Initiate the support to `Microsoft.Data.SqlClient` namespace. [#374](https://github.com/mikependon/RepoDb/issues/374)
- Feature: Support `PropertyHandlerAttribute` as requested. [#367](https://github.com/mikependon/RepoDb/issues/367)
- Feature: Re-enabled the [BulkInsert](/operation/bulkinsert) for `DataTable`.
- Feature: Support deleting an array of entity objects or primary keys via [DeleteAll](/operation/deleteall). [#353](https://github.com/mikependon/RepoDb/issues/353)

#### Others

- Support: Change the target type to .NetStandard 2.0.
- Support: Initiate the support to `Microsoft.Data.SqlClient` namespace. [#374](https://github.com/mikependon/RepoDb/issues/374)
- Enhancement: Support to Microsoft.Data.SqlClient [#359](https://github.com/mikependon/RepoDb/issues/359)
- NTH: Add a table hints in [Merge](/operation/merge) and [MergeAll](/operation/mergeall). [#370](https://github.com/mikependon/RepoDb/issues/370)
- NTH: Add a table hints in [Update](/operation/update) and [UpdateAll](/operation/updateall). [#371](https://github.com/mikependon/RepoDb/issues/371)
- NTH: Add a table hints in [Delete](/operation/delete) and [DeleteAll](/operation/deleteall). [#376](https://github.com/mikependon/RepoDb/issues/376)
- NTH: Add a table hints in [Insert](/operation/insert) and [InsertAll](/operation/insertall). [#379](https://github.com/mikependon/RepoDb/issues/379)


### RepoDB (v1.10.4)

- Initial support of RepoDb.PostgreSql.
- Added `IsPreparable` Property for `IDbSetting`.
- Removed the `basedOnFields` logic when extracting the `DbDataReader`.
- [InsertAll](/operation/insertall): Parsed the first entity property fields if the `fields` argument is not defined.
- Enhancement: Introduce the `BaseDbSetting` class to cater a uniform `HashCode` generator. #369
- Adhoc: Sealed and exposed the `DbSettings`, `DbHelpers` and the `DbStatementBuilders` classes.
- Enhancement: Introduced the `DbConvertFieldResolver` as the base converter field.


### RepoDB (v1.10.4-beta2)

- Initial support of RepoDb.PostgreSql.


### RepoDB (v1.10.4-beta1)

- Error: Invalid expression. The property `Id` is not defined on a target type #364 - MySql Support.


### RepoDB (v1.10.3)

- Revert the recurrent calls to `DbFieldCache`.Get() in the `ExecuteQuery` method.


### RepoDB (v1.10.2)

- Bug (Community Request): The primary field is not found exception when primary key column name is different from `Primary` attribute property name is different while `Connection.Update` is called. [#356](https://github.com/mikependon/RepoDb/issues/356)
- Bug: Set the return value of `Max` and `Min` operations to object. [#357](https://github.com/mikependon/RepoDb/issues/357)
- Performance: Refactor to remove the recurrent calls to `DbFieldCache`.Get() in the `ExecuteQuery` method.


### RepoDB (v1.10.2-alpha2)

- Bug: Set the return value of `Max` and `Min` operations to object. [#357](https://github.com/mikependon/RepoDb/issues/357)
- Refactor to remove the recurrent calls to `DbFieldCache`.Get() in the `ExecuteQuery` method.


### RepoDB (v1.10.2-alpha1)

- Bug (Community Request): The primary field is not found exception when primary key column name is different from `Primary` attribute property name is different while `Connection.Update` is called. [#356](https://github.com/mikependon/RepoDb/issues/356)


### RepoDB (v1.10.1)

- Removed the NetFramework Specific Library at Nuget.
- Supported the RepoDb.MySql extended library.


### RepoDB (v1.10.0)

- Breaking changes from the previous versions.
- This release contains major code refactoring for performance optimization purposes.
- Feature: Introduced the support `IDbSetting`. Used for other data providers extensibility complete support.
- Feature: Introduced `DbSettingMapper` class.
- Feature: Supported `Upsert` operations (abstracted with [Merge](/operation/merge) operation) for the data providers that does not support multi-statement execution and `MERGE` command.
- Feature: Added support to `Average` and `AverageAll` (with its `Async` version).
- Feature: Added support to `Exists` (with its `Async` version).
- Feature: Added support to `Max` and `MaxAll` (with its `Async` version).
- Feature: Added support to `Min` and `MinAll` (with its `Async` version).
- Feature: Added support to `Sum` and `SumAll` (with its `Async` version).
- Feature: Create an extended method `DbConnection.GetLastInsertedIdentity()` for other data providers extensibility complete support.
- Enhancement: Introduced `[QueryGroup](/class/querygroup).IsForUpdate()` method.
- Enhancement: Splitted the `SqlServerStatementBuilder` to a `BaseStatementBuilder`. Further supports for other data providers base statement building.
- Enhancement: Supported `IResolver` for 7 generic types.
- Refactoring: Renamed the `SqlDbHelper` to `SqlServerDbHelper`.
- Refactoring: Renamed the `SqlStatementBuilder` to `SqlServerStatementBuilder`.
- Test: Added an extensive Unit/Integration Tests for `Average`, `Exists`, `Max`, `Min`, `Sum` (and all its `Async` operations).
- Test: Added an extensive Unit Tests for `[QueryGroup](/class/querygroup).GetString()` and `QueryField.GetString()`.
- Bug: Where expression using IEnumerable`s contains throws error when using inherited class property [#301](https://github.com/mikependon/RepoDb/issues/301)


### RepoDB (v1.9.11)

- Stable release.
- Enhancement: Check current transaction (System.Transactions.Transaction.Current) before applying an explicit System.Data.`IDbTransaction` object. [#279](https://github.com/mikependon/RepoDb/issues/279)
- Enhancement: Table Hints is not passing properly in the `BatchQuery`. [#283](https://github.com/mikependon/RepoDb/issues/283)


### RepoDB (v1.9.10)

- Stable release.
- v1.9.9 changes + more Integration Tests for `DbConnection`.


### RepoDB (v1.9.9)

- Bug: `SqlException`: Login failed for user `xxx`
- Bug: Calling [InsertAll](/operation/insertall) with `MapAttribute` leads to `System.NullReferenceException`: Object reference not set to an instance of an object. [#274](https://github.com/mikependon/RepoDb/issues/274)
- Bug: `SqlDbHelper.GetFields` is failing if the transaction object is present. [#278](https://github.com/mikependon/RepoDb/issues/278)
- Enhancement: Remove database streaming when extracting table schema.
- Enhancement: Add `AsFields()` extended methods for the `IEnumerable` of `DbField` objects
#273
- Enhancement: Add `DbFieldCache.GetAsync` method. [#275](https://github.com/mikependon/RepoDb/issues/275)
- Enhancement: Add `DataEntityDataReader` into [BulkInsert](/operation/bulkinsert) that accepts TableName and Entities [#271](https://github.com/mikependon/RepoDb/issues/271)
- Enhancement: Add `AsFields()` extended methods for the `IEnumerable` of `DbField` objects.
- To Consider: Enable [BulkInsert](/operation/bulkinsert) with System.`DataTable` [#277](https://github.com/mikependon/RepoDb/issues/277)
- Test: Add IntegrationTests on [BulkInsert](/operation/bulkinsert) that accepts DataEntities and TableName.
- Refactoring: Refactor the code snippets for `DbFieldCache` to accept `IDbTransaction` objects. These affected too many chain of calls.
- Refactoring: Removed the `ToLower()` and replaced by `StringComparer.OrdinalIgnoreCase`.


### RepoDB (v1.9.9-beta5)

- Bug: `SqlDbHelper.GetFields` is failing if the transaction object is present. [#278](https://github.com/mikependon/RepoDb/issues/278)
- Refactoring: Refactor the code snippets for `DbFieldCache` to accept `IDbTransaction` objects. These affected too many chain of calls.


### RepoDB (v1.9.9-beta4)

- To Consider: Enable [BulkInsert](/operation/bulkinsert) with System.`DataTable` [#277](https://github.com/mikependon/RepoDb/issues/277)
- v1.9.9 release candidate


### RepoDB (v1.9.9-beta3)

- Enhancement: Add `DbFieldCache.GetAsync` method. [#275](https://github.com/mikependon/RepoDb/issues/275)
- Enhancement: Add `DataEntityDataReader` into [BulkInsert](/operation/bulkinsert) that accepts TableName and Entities [#271](https://github.com/mikependon/RepoDb/issues/271)
- Enhancement: Add `AsFields()` extended methods for the `IEnumerable<DbField>`
- Test: Add IntegrationTests on [BulkInsert](/operation/bulkinsert) that accepts DataEntities and TableName.


### RepoDB (v1.9.9-beta2)

- Enhancement: Add `AsFields()` extended methods for the `IEnumerable<DbField>` [#273](https://github.com/mikependon/RepoDb/issues/273)
- Bug: Calling [InsertAll](/operation/insertall) with `MapAttribute` leads to `System.NullReferenceException`: Object reference not set to an instance of an object. [#274](https://github.com/mikependon/RepoDb/issues/274)


### RepoDB (v1.9.9-beta1)

- Bug: SqlException: Login failed for user `xxx`
- Enhancement: Remove database streaming when extracting table schema.


### RepoDB (v1.9.8)

- Stable release of RepoDb.
- Enum Supports.
- Unorganized Table/Column Supports.
- Bug Fixes.


### RepoDB (v1.9.8-beta4)

- Title: A hybrid ORM library for .NET.
- Fix: Fixed the issue in the `[QueryGroup](/class/querygroup).Fix()` method if the depth of the Tree is at Level 4.


### RepoDB (v1.9.8-beta3)

- Fixed: Fixed the issue when using the Mapped/Quoted/Unorganized property in `[QueryGroup](/class/querygroup).Parse()` method.


### RepoDB (v1.9.8-beta2)

- Fixed: Failing operations on a purposely quoted class property. Reported by Christian Franck.


### RepoDB (v1.9.8-beta1)
     
- Requested: Document Enum Support [#261](https://github.com/mikependon/RepoDb/issues/261)
- Bug: Operations are failing on the Unorganized Table - by Christian Franck [#262](https://github.com/mikependon/RepoDb/issues/262)


### RepoDB (v1.9.7)

- Stable release with complete feature sets.
- Added netstandard2.0 as the default target framework at Nuget Package.


### RepoDB (v1.9.6)

- [Note] This version is the first ever version release with complete features. The next version will be only be bug-fixes from this version (if we found some).
- [Core] Optimize the Expression field iteration between the number of Class properties and `DbDataReader` columns. [#136](https://github.com/mikependon/RepoDb/issues/136)
- [Core] Add a pluggable interface/abstract for `DbProviderOperation` [#158](https://github.com/mikependon/RepoDb/issues/158)
- [Core] Add a `DbTransaction` object on [InsertAll](/operation/insertall), [MergeAll](/operation/mergeall), [UpdateAll](/operation/updateall) operations. [#213](https://github.com/mikependon/RepoDb/issues/213)
- [Test] Added an Integration Tests for `IdentityClassWithDifferentIdentity`.
- [Test] Add IntegrationTest for [UpdateAll](/operation/updateall) targeting certain columns. [#245](https://github.com/mikependon/RepoDb/issues/245)
- [Test] Add an `Async` method support to `QueryMultipleExtractor.Extract`. [#255](https://github.com/mikependon/RepoDb/issues/255)
- [Test] Add an `Async` method support to `QueryMultipleExtractor.Scalar`. [#256](https://github.com/mikependon/RepoDb/issues/256)
- [Test] Introduce UnitTest for IDbOperationProvider Interface. [#253](https://github.com/mikependon/RepoDb/issues/253)
- [Test] Create a test for `IStatementBuilder` for all `Async` operations for `DbConnection`, `DbRepository`, `BaseRepository`. [#218](https://github.com/mikependon/RepoDb/issues/218)
- [Test] Add more extensive UnitTest for `IN`,  `NOT IN`, `BETWEEN`,  `NOT BETWEEN`, `LIKE` and `NOT LIKE` operations. [#186](https://github.com/mikependon/RepoDb/issues/186)
- [Test] Create a much more extensive UnitTests for all Operations (`Equal`, `NotEqual`, `Between` ... ) [#178](https://github.com/mikependon/RepoDb/issues/178)
- [Test] Create an extensive IntegrationTests for `IN`,  `NOT IN`, `BETWEEN`,  `NOT BETWEEN`, `LIKE` and `NOT LIKE` operations. [#180](https://github.com/mikependon/RepoDb/issues/180)
- [Test] Create IntegrationTest for `DbTransaction` (Insert, [Merge](/operation/merge), Delete, [Update](/operation/update)) [#181](https://github.com/mikependon/RepoDb/issues/181)
- [Added] Introduce `SqlDbOperationProvider` Class. [#251](https://github.com/mikependon/RepoDb/issues/251)
- [Added] Introduce `DbOperationProviderMapper` Class. [#252](https://github.com/mikependon/RepoDb/issues/252)
- [Added] Introduce `IDbOperationProvider` Interface. [#250](https://github.com/mikependon/RepoDb/issues/250)
- [Adhoc] Add `BatchSize` in [BulkInsert](/operation/bulkinsert). [#257](https://github.com/mikependon/RepoDb/issues/257)
- [Adhoc] Remove all `obsolete` methods for v1.9.6. [#246](https://github.com/mikependon/RepoDb/issues/246)
- [Minor] Hide the exposed extended internal methods. [#244](https://github.com/mikependon/RepoDb/issues/244)


### RepoDB (v1.9.5)

- [Note] This version is the first ever version release with complete features. The next version will be only be bug-fixes from this version (if we found some).
- [Core] Introduce `UpdateMultiple`, different from [UpdateAll](/operation/updateall). [#94](https://github.com/mikependon/RepoDb/issues/94)
- [Core] Introduce the [UpdateAll](/operation/updateall) via ``PrimaryKey``. [#93](https://github.com/mikependon/RepoDb/issues/93)
- [Core] Introduce `Query` and `QueryAsync` Table-Based Calls [#176](https://github.com/mikependon/RepoDb/issues/176)
- [Core] Introduce `QueryAll` and `QueryAllAsync` Table-Based Calls [#221](https://github.com/mikependon/RepoDb/issues/221)
- [Core] Introduce `BatchQuery`, `BatchQueryAsync` Table-Based Calls [#175](https://github.com/mikependon/RepoDb/issues/175)
- [Core] Create an IL and Compiled Expressions for [Update](/operation/update), [Merge](/operation/merge), [Insert](/operation/insert) and [InsertAll](/operation/insertall) Parameter Passing [#197](https://github.com/mikependon/RepoDb/issues/197)
- [Core] Introduce the `InsertMultiple`, different from [InsertAll](/operation/insertall). [#92](https://github.com/mikependon/RepoDb/issues/92)
- [Core] Add ExecutionContext Cache for [Insert](/operation/insert). [#205](https://github.com/mikependon/RepoDb/issues/205)
- [Core] Add ExecutionContext Cache for [Merge](/operation/merge). [#206](https://github.com/mikependon/RepoDb/issues/206)
- [Core] Add ExecutionContext Cache for [Update](/operation/update). [#208](https://github.com/mikependon/RepoDb/issues/208)
- [Core] Add ExecutionContext Cache for [UpdateAll](/operation/updateall). [#209](https://github.com/mikependon/RepoDb/issues/209)
- [Core] Add ExecutionContext Cache for [MergeAll](/operation/mergeall). [#207](https://github.com/mikependon/RepoDb/issues/207)
- [Core] Re-enable the operation for [Update](/operation/update)via `DataEntity` object. [#188](https://github.com/mikependon/RepoDb/issues/188)
- [Performance] Create a cached Expression when setting back the `PrimaryKey` values in [Insert](/operation/insert) and [InsertAll](/operation/insertall). [#211](https://github.com/mikependon/RepoDb/issues/211)
- [Test] Add extensive IntegrationTests for type CRUD via TableName Calls. [#222](https://github.com/mikependon/RepoDb/issues/222)
- [Test] [Insert](/operation/insert) via TableName using Dynamic object with Invalid Column Casing [#223](https://github.com/mikependon/RepoDb/issues/223)
- [Test] Add more IntegrationTest for [UpdateAll](/operation/updateall). [#231](https://github.com/mikependon/RepoDb/issues/231)
- [Test] Add UnitTest for [MergeAll](/operation/mergeall) ITrace object. [#240](https://github.com/mikependon/RepoDb/issues/240)
- [Test] Added more extensive IntegrationTests for [MergeAll](/operation/mergeall) operation. [#242](https://github.com/mikependon/RepoDb/issues/242)
- [Test] Add UnitTest for [UpdateAll](/operation/updateall) (`IStatementBuilder`, ITrace, QueryBuilder) [#230](https://github.com/mikependon/RepoDb/issues/230)
- [Test] Add `UnitTest` for [InsertAll](/operation/insertall). [#214](https://github.com/mikependon/RepoDb/issues/214)
- [Bug] The version 1.9.2 is an (untagged) pre-release version. The Id property is failing on [Insert](/operation/insert) if the Data Type is not long [#215](https://github.com/mikependon/RepoDb/issues/215)
- [Bug] [Insert](/operation/insert) via TableName using Dynamic object with Invalid Column Casing [#223](https://github.com/mikependon/RepoDb/issues/223)
- [Bug] [Core] [Insert](/operation/insert) is failing for non-null (non-table) properties (XJNEN) [#212](https://github.com/mikependon/RepoDb/issues/212)
- [Bug] DbHelper: Script execution security related issue in the company (XJNEN) [#229](https://github.com/mikependon/RepoDb/issues/229)
- [Bug] Expression based using the `ToList().Contains()` is failing. But the `ToArray().Contains()` is working. XJNEN [#233](https://github.com/mikependon/RepoDb/issues/233)
- [Known-Bug] Error is thrown when calling the [UpdateAll](/operation/updateall) with dynamic entities (and the fields are not equals to the DB fields) and the `qualifiers` were not defined. [#232](https://github.com/mikependon/RepoDb/issues/232)
- [Adhoc] Call the `AsList()` method when calling the `[QueryGroup](/class/querygroup).GetString()` method. Support the case of XJNEN [#228](https://github.com/mikependon/RepoDb/issues/228)
- [Adhoc] Reviewed `BaseRepository`, `DbRepository`, `DbConnection` Async/Await Keywords
- [Adhoc] Reviewed UnitTests for the ITrace (`BaseRepository`, `DbRepository`, `DbConnection`)
- [Adhoc] Convert all Mappers to become a Resolvers by implementing the IResolver interface. [#227](https://github.com/mikependon/RepoDb/issues/227)
- [Adhoc] Remove all MapItem Classes from the Mappers. [#226](https://github.com/mikependon/RepoDb/issues/226)
- [Removed] TypeMapItem Class
- [Removed] DbIdentityCache Class


### RepoDB (v1.9.4)

- [Note] This version is the first ever version release with complete features. The next version will be only be bug-fixes from this version (if we found some).
- [Core] Introduce `UpdateMultiple`, different from [UpdateAll](/operation/updateall). [#94](https://github.com/mikependon/RepoDb/issues/94)
- [Core] Introduce the [UpdateAll](/operation/updateall) via ``PrimaryKey``. [#93](https://github.com/mikependon/RepoDb/issues/93)
- [Core] Introduce `Query` and `QueryAsync` Table-Based Calls [#176](https://github.com/mikependon/RepoDb/issues/176)
- [Core] Introduce `QueryAll` and `QueryAllAsync` Table-Based Calls [#221](https://github.com/mikependon/RepoDb/issues/221)
- [Core] Introduce `BatchQuery`, `BatchQueryAsync` Table-Based Calls [#175](https://github.com/mikependon/RepoDb/issues/175)
- [Core] Create an IL and Compiled Expressions for [Update](/operation/update), [Merge](/operation/merge), [Insert](/operation/insert) and [InsertAll](/operation/insertall) Parameter Passing [#197](https://github.com/mikependon/RepoDb/issues/197)
- [Core] Introduce the `InsertMultiple`, different from [InsertAll](/operation/insertall). [#92](https://github.com/mikependon/RepoDb/issues/92)
- [Core] Add ExecutionContext Cache for [Insert](/operation/insert). [#205](https://github.com/mikependon/RepoDb/issues/205)
- [Core] Add ExecutionContext Cache for [Merge](/operation/merge). [#206](https://github.com/mikependon/RepoDb/issues/206)
- [Core] Add ExecutionContext Cache for [Update](/operation/update). [#208](https://github.com/mikependon/RepoDb/issues/208)
- [Core] Add ExecutionContext Cache for [UpdateAll](/operation/updateall). [#209](https://github.com/mikependon/RepoDb/issues/209)
- [Core] Add ExecutionContext Cache for [MergeAll](/operation/mergeall). [#207](https://github.com/mikependon/RepoDb/issues/207)
- [Core] Re-enable the operation for [Update](/operation/update) via `DataEntity` object. [#188](https://github.com/mikependon/RepoDb/issues/188)
- [Performance] Create a cached Expression when setting back the `PrimaryKey` values in [Insert](/operation/insert) and [InsertAll](/operation/insertall). [#211](https://github.com/mikependon/RepoDb/issues/211)
- [Test] Add extensive IntegrationTests for type CRUD via TableName Calls. [#222](https://github.com/mikependon/RepoDb/issues/222)
- [Test] [Insert](/operation/insert) via TableName using Dynamic object with Invalid Column Casing [#223](https://github.com/mikependon/RepoDb/issues/223)
- [Test] Add more IntegrationTest for [UpdateAll](/operation/updateall). [#231](https://github.com/mikependon/RepoDb/issues/231)
- [Test] Add UnitTest for [MergeAll](/operation/mergeall) ITrace object. [#240](https://github.com/mikependon/RepoDb/issues/240)
- [Test] Added more extensive IntegrationTests for [MergeAll](/operation/mergeall) operation. [#242](https://github.com/mikependon/RepoDb/issues/242)
- [Test] Add UnitTest for [UpdateAll](/operation/updateall) (`IStatementBuilder`, ITrace, QueryBuilder) [#230](https://github.com/mikependon/RepoDb/issues/230)
- [Test] Add `UnitTest` for [InsertAll](/operation/insertall). [#214](https://github.com/mikependon/RepoDb/issues/214)
- [Bug] The version 1.9.2 is an (untagged) pre-release version. The Id property is failing on [Insert](/operation/insert) if the Data Type is not long [#215](https://github.com/mikependon/RepoDb/issues/215)
- [Bug] [Insert](/operation/insert) via TableName using Dynamic object with Invalid Column Casing [#223](https://github.com/mikependon/RepoDb/issues/223)
- [Bug] [Core] [Insert](/operation/insert) is failing for non-null (non-table) properties (XJNEN) [#212](https://github.com/mikependon/RepoDb/issues/212)
- [Bug] DbHelper: Script execution security related issue in the company (XJNEN) [#229](https://github.com/mikependon/RepoDb/issues/229)
- [Bug] Expression based using the `ToList().Contains()` is failing. But the `ToArray().Contains()` is working. XJNEN [#233](https://github.com/mikependon/RepoDb/issues/233)
- [Adhoc] Call the `AsList()` method when calling the `[QueryGroup](/class/querygroup).GetString()` method. Support the case of XJNEN [#228](https://github.com/mikependon/RepoDb/issues/228)
- [Adhoc] Reviewed `BaseRepository`, `DbRepository`, `DbConnection` Async/Await Keywords
- [Adhoc] Reviewed UnitTests for the ITrace (`BaseRepository`, `DbRepository`, `DbConnection`)
- [Adhoc] Convert all Mappers to become a Resolvers by implementing the IResolver interface. [#227](https://github.com/mikependon/RepoDb/issues/227)
- [Adhoc] Remove all `MapItem` Classes from the Mappers. [#226](https://github.com/mikependon/RepoDb/issues/226)
- [Removed] `TypeMapItem` Class
- [Removed] `DbIdentityCache` Class


### RepoDB (v1.9.3)

- [Core] Introduce ExecutionContext to hold the caching of the execution for [InsertAll](/operation/insertall). [#204](https://github.com/mikependon/RepoDb/issues/204)
- [Enhancement, Performance] [InsertAll](/operation/insertall) Compiled Expressions
- [Enhancement] Revisits the `DbField` for `Primary` and Identity Columns. [#182](https://github.com/mikependon/RepoDb/issues/182)
- [Enhancement] Add the `IdentityDbField` in both [Merge](/operation/merge) and [Update](/operation/update) SqlStatementBuilder. [#198](https://github.com/mikependon/RepoDb/issues/198)
- [Enhancement] Rename the `DataReaderConverter` to `DataReader`. [#200](https://github.com/mikependon/RepoDb/issues/200)
- [Enhancement] Add Flush method in the `CommandTextCache`, and exposed the class. [#220](https://github.com/mikependon/RepoDb/issues/220)
- [Performance] Create a cached Expression when setting back the `PrimaryKey` values in [Insert](/operation/insert) and [InsertAll](/operation/insertall). [#211](https://github.com/mikependon/RepoDb/issues/211)
- [Performance] Use the compiled function for inserting single `DataEntity` if the BatchSize is 1 for [InsertAll](/operation/insertall). [#217](https://github.com/mikependon/RepoDb/issues/217)
- [Fixed] Remove the [Insert](/operation/insert) and [InsertAll](/operation/insertall) identity conversion from SQL. [#203](https://github.com/mikependon/RepoDb/issues/203) - Fixed by introducing the `ConversionResolver` classes.
- [Test] Create UnitTests for (`DbConnection`, `DbRepository`, `BaseRepository`) [InsertAll](/operation/insertall) operation for `IStatementBuilder`. [#216](https://github.com/mikependon/RepoDb/issues/216)
- [Test] Add UnitTests for ClientTypeToSqlDbTypeResolver, SqlDbTypeNameToClientTypeResolver and SqlDbTypeToStringNameResolver [#219](https://github.com/mikependon/RepoDb/issues/219)
- [Added] `IConversionResolver`
- [Added] `ClientTypeToSqlDbTypeResolver`
- [Added] `SqlDbTypeNameToClientTypeResolver`
- [Added] `SqlDbTypeToStringNameResolver`
- [Added] `SqlVariant`
- [Added] `ParameterField`
- [Added] `InsertExecutionContext`
- [Added] `InsertExecutionContextCache`
- [Added] `InsertAllExecutionContext`
- [Added] `InsertAllExecutionContextCache`


### RepoDB (v1.9.2)

- [Core] Introduce the [InsertAll](/operation/insertall), different from `InsertMultiple`. [#91](https://github.com/mikependon/RepoDb/issues/91)
- [Core] Return the number of affected rows during [BulkInsert](/operation/bulkinsert) for `DbDataReader`. [#192](https://github.com/mikependon/RepoDb/issues/192)
- [Core] Add a `SetParameters` extended methods for `DbCommand` object. [#196](https://github.com/mikependon/RepoDb/issues/196)
- [Core, Requested] Re-enable the operation for [Delete](/operation/delete)via `DataEntity` object. [#185](https://github.com/mikependon/RepoDb/issues/185)
- [Core, Requested] Re-enable the operation for [Update](/operation/update)via `DataEntity` object. [#188](https://github.com/mikependon/RepoDb/issues/188)
- [Core, Requested] Add support to exclude non-table Class Properties in all Operations. [#189](https://github.com/mikependon/RepoDb/issues/189)
- [Adhoc, Requested] Expose the `DataEntityDataReader` Class. [#172](https://github.com/mikependon/RepoDb/issues/172)
- [Adhoc, Requested] Expose the `[QueryGroup](/class/querygroup).Fix()` method. [#179](https://github.com/mikependon/RepoDb/issues/179)
- [Adhoc] Revisit the `async Task` in all `DbRepository` methods. [#190](https://github.com/mikependon/RepoDb/issues/190)
- [Adhoc] Add a new repository method named `‘`EnsureOpenAsync`’`. [#111](https://github.com/mikependon/RepoDb/issues/111)
- [Test] Add an extensive IntegrationTests for the Entity with Extra Fields. [#183](https://github.com/mikependon/RepoDb/issues/183)
- [Test] Add all UnitTests for `Trace` call for all `Async` operations. [#193](https://github.com/mikependon/RepoDb/issues/193)
- [Test] Add UnitTest for [InsertAll](/operation/insertall). [#194](https://github.com/mikependon/RepoDb/issues/194)
- [Test] Add IntegrationTests for [InsertAll](/operation/insertall). [#195](https://github.com/mikependon/RepoDb/issues/195)
- [Test] Add more extensive UnitTest for `IN`,  `NOT IN`, `BETWEEN`,  `NOT BETWEEN`, `LIKE` and `NOT LIKE` operations. [#186](https://github.com/mikependon/RepoDb/issues/186)
- [Test] Add extensive IntegrationTests for ConnectionPersistency. [#191](https://github.com/mikependon/RepoDb/issues/191)
- [Enhancement] Auto-set the `PrimaryField` value of the object after calling the `Insert<T>` operation. [#187](https://github.com/mikependon/RepoDb/issues/187)


### RepoDB (v1.9.1)

- Stable Release of RepoDb.
- [Update] Exposed BulkCopyOptions and Transaction to [BulkInsert](/operation/bulkinsert) Operation.


### RepoDB (v1.9.0)

- [Core] Introduced table-based operations for  [Count](/operation/count), `[CountAll](/operation/countall)`, [Delete](/operation/delete), [DeleteAll](/operation/deleteall), [Insert](/operation/insert), [Merge](/operation/merge), `[Truncate](/operation/truncate)` and [Update](/operation/update).
- [Core] Introduced `[CountAll](/operation/countall)` and [QueryAll](/operation/queryall) operations.
- [Core] Introduced pluggable interface `DbHelpers`.
- [Core] Updated the `QueryBuilder` to remove the `TEntity` at class level (moved it to method level).
- [Core] Updated the `StatementBuilder` SQL Text generation via TableName.
- [Core] Supported `Dynamic`, `ExpandoObject`, `IDictionary<string, object>`, [QueryField](/class/queryfield), `IEnumerable<QueryField>` and `[QueryGroup](/class/querygroup)` objects in the `Execute<Method>` calls.
- [Added] `ExecuteScalar<T>` and `ExecuteScalarAsync<T>`
- [Added] `DbField`
- [Added] `DbFieldCache`
- [Removed] `AsyncResultExtractor`
- [Removed] `StatementBuilderMapItem`
- [Removed] `FieldDefinition`
- [Removed] `FieldDefinitionCache`
- [Renamed] `SqlHelper` to `SqlDbHelper`
- [Renamed] `PrimaryKeyCache` to `PrimaryCache`.
- [Renamed] `PrimaryKeyIdentityCache` to `PrimaryIdentityCache`
- [Optimization] CountAsync operation is now returning the `Task<int>` type instead of `Task<object>`.
- [Optimization] Allow passing of cache expiration time during [Query](/operation/query) and [QueryAll](/operation/queryall) calls.
- [Optimization, Pull-Request] Enumerations `Order`, `Conjunction` and `Operation` is now a pre-generated `int` values.
- Introduced complete sets of IntegrationTests and UnitTests in all of the changes mentioned above.
- See v1.9.0-beta1 and v1.9.0-beta2 for complete set of changes.


### RepoDB (v1.9.0-beta2)

- [Core] Make the `DbHelper` Pluggable by Provider. [#137](https://github.com/mikependon/RepoDb/issues/137)
- [Core] [NTH]: Support `InlineDelete(string tableName, object where ...)` [#113](https://github.com/mikependon/RepoDb/issues/113) -- Moved to Delete
- [Core] Add table based operations for  [Count](/operation/count), [Delete](/operation/delete), [DeleteAll](/operation/deleteall), [Insert](/operation/insert), [Merge](/operation/merge), [Truncate](/operation/truncate), [Update](/operation/update). [#159](https://github.com/mikependon/RepoDb/issues/159)
- [Core] Organize the ordering of the arguments in all operations. [#160](https://github.com/mikependon/RepoDb/issues/160)
- [Core] Introduce [CountAll](/operation/countall) operation. [#161](https://github.com/mikependon/RepoDb/issues/161)
- [Enhancement] Revisits the NET Framework custom method for GetCustomAttributes<T>. [#133](https://github.com/mikependon/RepoDb/issues/133)
- [Enhancement] Support passing of [QueryGroup](/class/querygroup), [QueryField](/class/queryfield), IEnumerable<QueryField> in the Execution<Method> Operations [#140](https://github.com/mikependon/RepoDb/issues/140)
- [Enhancement] Remove the `StatementBuilderMapItem` class if possible. [#139](https://github.com/mikependon/RepoDb/issues/139)
- [Enhancement] Remove the `Provider` Enumeration. [#138](https://github.com/mikependon/RepoDb/issues/138)
- [Enhancement] Reorder the parameter of for target table to [BulkInsert](/operation/bulkinsert)(TableName, `DbDataReader`). [#145](https://github.com/mikependon/RepoDb/issues/145)
- [Enhancement] Properly parse the type of the passed parameters when parsing the RawSql Array Parameters. [#147](https://github.com/mikependon/RepoDb/issues/147)
- [Enhancement] [NTH]: Support InlineInsert(string tableName, object param ...) [#114](https://github.com/mikependon/RepoDb/issues/114) -- Moved to [Insert](/operation/insert)
- [Enhancement] Implement the `prefix` as a passable argument when during conversion. [#148](https://github.com/mikependon/RepoDb/issues/148)
- [Enhancement] Add additional argument in the DataReaderConverter.ToEnumerable<T> method to support the calls to DbHelper.Get<T> method. [#142](https://github.com/mikependon/RepoDb/issues/142)
- [Enhancement] Add a caching mechanism for type [Field](/class/field) objects. [#157](https://github.com/mikependon/RepoDb/issues/157)
- [Enhancement] [Merge](/operation/merge) all inline operations into main operations (InlineMerge should be [Merge](/operation/merge)). [#156](https://github.com/mikependon/RepoDb/issues/156)
- [Adhoc] Created a new cache class named `DbIdentityCache`.
- [Adhoc] Renamed the `FieldDefinition` into `DbField`.
- [Adhoc] Renamed the `FieldDefinitionCache` to `DbFieldCache`.
- [Adhoc] Renamed the `SqlHelper` to `SqlDbHelper`.
- [Adhoc] Renamed the `PrimaryKeyCache` to `PrimaryCache`.
- [Adhoc] Renamed the `PrimaryKeyIdentityCache` to `PrimaryIdentityCache`.
- [Adhoc] Moved the `DbHelpers` into `RepoDb.`DbHelpers`.
- [Adhoc, Optimization] Made the `DbFieldCache` object more dynamic to any DB providers.
- [Test] Add additional logic in the Integration Tests of the `IStatementBuilder`, verify that the second call is not hitting the method. [#141](https://github.com/mikependon/RepoDb/issues/141)
- [Test] Add an extensive Unit/Integration Test for InlineInsert that targets a table name. [#146](https://github.com/mikependon/RepoDb/issues/146)
- [Test] Create UnitTests for [CountAll](/operation/countall). [#163](https://github.com/mikependon/RepoDb/issues/163)
- [Test] Add separate `IntegrationTests` for the RawSql ArrayValues [#168](https://github.com/mikependon/RepoDb/issues/168)
- [Test] Add separate `IntegrationTests` for different Execute<Method> parameters. [#169](https://github.com/mikependon/RepoDb/issues/169)
- [Test] Create IntegrationTests for QueryAll. [#167](https://github.com/mikependon/RepoDb/issues/167)
- [Test] Create IntegrationTests for [CountAll](/operation/countall). [#164](https://github.com/mikependon/RepoDb/issues/164)
- [Documentation] Document the [CountAll](/operation/countall) operation. [#162](https://github.com/mikependon/RepoDb/issues/162)
- [Documentation] Add a separate documentation entry for Execute<Method> with Array parameters argument. [#143](https://github.com/mikependon/RepoDb/issues/143)


### RepoDB (v1.9.0-beta1)

- [New] Updated the description to "A dynamic, lightweight, efficient and very fast Hybrid ORM library for .NET.".
- [New] Re-instate the row deletion by entity level (connection.Delete<T>(T entity)) [#112](https://github.com/mikependon/RepoDb/issues/112)
- [Bug] `Query` using Expression is failing for `Contains()` == `false` [#102](https://github.com/mikependon/RepoDb/issues/102)
- [Test] Create an Integration Tests for a model with much columns that the result of the [ExecuteQuery](/operation/executequery) [#103](https://github.com/mikependon/RepoDb/issues/103)
- [Test] Add Integration Tests for Execute<Methods> with IDictionary and ExpandoObject parameters. [#123](https://github.com/mikependon/RepoDb/issues/123)
- [Test] Add an intensive UnitTests for Cache ExpirationInMinutes in the `DbConnection`, `DbRepository` and `BaseRepository`. [#129](https://github.com/mikependon/RepoDb/issues/129)
- [Test] Add major Integration Tests for Caching for SqlConnection, `DbRepository`, `BaseRepository`. [#130](https://github.com/mikependon/RepoDb/issues/130)
- [Test] Add IntegrationTests for [Insert](/operation/insert)<TEntity, TResult> and InlineInsert<TEntity, TResult> [#132](https://github.com/mikependon/RepoDb/issues/132)
- [Enhancement, Major] Remove the TEntity in QueryBuilder, implement it like this QueryBuilder (instead of QueryBuilder<TEntity>) [#115](https://github.com/mikependon/RepoDb/issues/115)
- [Enhancement, Major] Remove the AsyncResultExtractor class. [#124](https://github.com/mikependon/RepoDb/issues/124)
- [Enhancement] Short datatype used for Enums [#107](https://github.com/mikependon/RepoDb/issues/107)
- [Enhancement] Remove the internal StringConstants class. [#117](https://github.com/mikependon/RepoDb/issues/117)
- [Enhancement] Make the `CountAsync` operation return type `long` instead of `object` without affecting the parallelism. [#108](https://github.com/mikependon/RepoDb/issues/108)
- [Enhancement] Add a new operational method ExecuteScalar<T> (and ExecuteScalarAsync<T>). [#121](https://github.com/mikependon/RepoDb/issues/121)
- [Enhancement] Support passing of IDictionary<string, object> as `param` in the Execute<Methods> operation. [#125](https://github.com/mikependon/RepoDb/issues/125)
- [Enhancement] Allow passing of cache expiration time during creation and in the repository. [#128](https://github.com/mikependon/RepoDb/issues/128)

### RepoDB (v1.8.4)

- Stable Spring Release of RepoDb. Enjoy!


### RepoDB (v1.8.3)

- Stable Spring Release of RepoDb. Enjoy!

### RepoDB (v1.8.2)

#### Updates

- Updated to again support the `BatchQuery` dynamic expression (first-level properties).
- Updated to again support the  [Count](/operation/count) dynamic expression (first-level properties).
- Updated to again support the `whereOrPrimaryKey` argument rather than `primaryKey` (first-level properties).

#### Added

- Additional Integration Tests for class/object mappings (CRUD).
- Additional Integration Tests for the `Dynamics` and `Expressions` query expression for `DbConnection`, `DbRepository` and ``BaseRepository``.


### RepoDB (v1.8.1)

### New Features

- New: Introduced the [ExecuteQueryMultiple](/operation/executequerymultiple) into the `DbRepository`.
- New: Introduced the `QueryMultiple` into the `DbRepository`.
- New: Introduced the `ConversionType` to let the users decide the type of the conversions. Accessible via `TypeMapper.ConversionType` property.

### Optimizations

- Optimization: Added a class-level checking when identifying the ``PrimaryKey`` of a class.
- Optimization: Supported the type conversions(if convertible) when querying the data from the database.
- Optimization: Simplified the extraction of the result of the [ExecuteQueryMultiple](/operation/executequerymultiple) via `Extract()` method.

#### Added

- Added: A class named `AsyncResultExtractor` to control the extraction of the result in the caller side for all `Async` methods of the ``BaseRepository`/DbRepository`.
- Added: A class named `QueryMultipleRequest` to handle the request when calling the `QueryMultiple` operation.
- Added: A class named `CommandArrayParameter` to hold the array parameters for Raw SQL statements.
- Added: A method named `Reset` for both [QueryField](/class/queryfield) and `[QueryGroup](/class/querygroup)` objects  allow the user to reinstate the instance of that object.
- Added: An operation named [BulkInsert](/operation/bulkinsert) at  `DbRepository` with `DbDataReader` as the parameter.
- Added: An argument named `hints` for both the `BatchQuery` and  [Count](/operation/count) operation.
- Added: An intensive `IntegrationTests` for all the different data types of the database (SQL Server) (Numbers, Spatials, Strings, Dates, Bytes, Others).
- Added: An intensive `IntegrationTests` for the data types conversions(i.e: String-to-Numbers (vice versa), String-to-Dates (vice versa), etc).
- Added: An intensive `IntegrationTests` for the invalid casings.
- Added: An intensive `IntegrationTests` for all the operations of the `DbConnection`, `DbRepository` and ``BaseRepository`` objects.

### Fixes

- Fixed: An issue in the `InlineMerge` if the primary key is not defined in the dynamic object.
- Fixed: An issue in the [Merge](/operation/merge) if the primary key is an identity.
- Fixed: An issue in the `QueryMultiple` if the same expression is are used multiple times.


### RepoDB (v1.8.1-beta1)

### New Features

- Introduced the [ExecuteQueryMultiple](/operation/executequerymultiple) into the `DbRepository`.
- Introduced the `QueryMultiple` into the `DbRepository`.
- Introduced the `ConversionType` to let the users decide the strictness of the conversions. Accesible via `TypeMapper.ConversionType` property.

#### Added

- In the `Async` methods, introduced the `AsyncResultExtractor` class to control the extraction of the result in the caller side.
- Supported [BulkInsert](/operation/bulkinsert) for `DbRepository` with `DbDataReader` as the parameter.
- Added an `IntegrationTests` for all the different data types of the database (SQL Server) (Numbers, Spatials, Strings, Dates, Bytes, Others).
- Added an `IntegrationTests` for the data types conversions(i.e: String-to-Numbers (vice versa), String-to-Dates (vice versa), etc).
- Added an `IntegrationTests` for the invalid casings.

### Optimizations

- Added a class-level checking when identifying the ``PrimaryKey`` of a class.
- Supported the type conversions(if convertible) when querying the data from the database.

### Todo for 1.8.1

- Complete sets of `IntegrationTests` for `DbConnection`, `DbRepository`, `BaseRepository` operations.
- The version 1.8.1 will be the highest production-grade release of the library.


### RepoDB (v1.8.0)

### New Features

- Introduced the support for `DbConnection.QueryMultiple`.
- Introduced the support for `DbConnection.ExecuteQueryMultiple`.

#### Added

- Added a class [QueryMultipleExtractor](/class/querymultipleextractor) to manage the extraction of the result of `DbConnection.ExecuteQueryMultiple` operation.
- Added a class named `CommandParameter` to handle the value of the parameter mapping into the target Type.
- Added a class named `QueryGroupTimeMap` to support the mapping of the [QueryGroup](/class/querygroup) into the Type.
- Introduced a `hints` argument in the `DbConnection.Query` operation.
- Added class `SqlTableHints`.
- Supported [BulkInsert](/operation/bulkinsert) for `DbDataReader`.

#### Removed

- Removed the `Operation.Any`.
- Removed the `Operation.All`.
- Removed the `orderBy` and `top` argument in the [Query](/operation/query) method with `primaryKey` argument.
- Removed the `DbConnection.BatchQuery` method with `primaryKey` argument.
- Removed the `DbConnection.Count` method with `primaryKey` argument.
- Removed the `DbConnection.Delete` method without the WHERE parameter.
- Removed the support on `dynamic` object query tree expressions.

### Discontinued

- Removed the attribute `Command`.
- Removed the attribute `Ignored`.

### Optimizations

- Revisits the way on how to map the `[QueryGroup](/class/querygroup)` list of [QueryField](/class/queryfield) into the data entity type.
- Refactor the Linq (IEnumerable<T>.ToList()) into an old-school (foreach / for (var i..)) approach.


### RepoDB (v1.8.0-beta5)

- (Major [Update](/operation/update)) Introduced the support for `DbConnection.QueryMultiple`.
- (Major [Update](/operation/update)) Introduced the support for `DbConnection.ExecuteQueryMultiple`.
- Added class [QueryMultipleExtractor](/class/querymultipleextractor).


### RepoDB (v1.8.0-beta4)

- Introduced a `hints` argument in the `DbConnection.Query` operation.
- Added class `SqlTableHints`.


### RepoDB (v1.8.0-beta3)

- Supported [BulkInsert](/operation/bulkinsert) for `DbDataReader`.
- Removed the `Operation.Any`.
- Removed the `Operation.All`.


### RepoDB (v1.8.0-beta2)

- Removed the `orderBy` and `top` argument in the [Query](/operation/query) method with `primaryKey` argument.
- Removed the `DbConnection.BatchQuery` method with `primaryKey` argument.
- Removed the `DbConnection.Count` method with `primaryKey` argument.
- Removed the `DbConnection.Delete` method without the WHERE parameter.


### RepoDB (v1.8.0-beta1)

- Remove the support on dynamic query tree expresssions.
- Removed the Command enumeration.
- Removed the Ignored attribute.


### RepoDB (v1.7.0)
   
- `Async` Method Calls Optimizations
- Expression-Based Queries
- Removed Support for Recursive Query
- Initial Support for Different Database Providers


### RepoDB (v1.7.0-beta5)
   
- Fixed the invalid binaries deployed at v1.7.0-beta4.
- Modified `async` operations implementation to leverage the awaitable features.
- Exposed the `IsForProvider` and `GetProvider` `DbConnection` extended methods.
- Introduced a `BulkInsertMapItem` object to provide ability to override the [BulkInsert](/operation/bulkinsert) operation default mappings.
- Removed the recursive query features (DataEntity, DataEntityChildItemData, DataEntityChildListData, RecursionManager, ForeignAttribute).


### RepoDB (v1.7.0-beta4)

- Modified `async` operations implementation to leverage the awaitable features.
- Exposed the `IsForProvider` and `GetProvider` `DbConnection` extended methods.
- Introduced a `BulkInsertMapItem` object to provide ability to override the [BulkInsert](/operation/bulkinsert) operation default mappings.
- Removed the recursive query features (DataEntity, DataEntityChildItemData, DataEntityChildListData, RecursionManager, ForeignAttribute).


### RepoDB (v1.7.0-beta3)

- Fixed Target Framework Referencing Issues of NuGet Package
- Added a new enumeration for data providers.
- Updated the statement builder mapper to use the Provider object instead of `DbConnection` type.


### RepoDB (v1.7.0-beta2)

- Introduced Expression-Based `Query` for Connection and Repository Operations
- Introduced Support to All (as `Operation.Al`l), Any (as `Operation.Any`), Contains (as `Operation.Like`, `Operation.NotLike`, `Operation.In`, Operation.NotIn`)
- Introduced an Expression-Based `qualifer` field for [Merge](/operation/merge) and `InlineMerge` operation
- Unit Test updates for `All`, `Any`, and `Contains` operation


### RepoDB (v1.7.0-beta1)

- Introduced Expression-Based `Query` for Connection and Repository Operations
- Introduced Expression-Based Parsing for [QueryGroup](/class/querygroup), [QueryField](/class/queryfield), [Field](/class/field), [OrderField](/class/orderfield)
- Introduced Array-Based Parameters when calling `ExecuteScalar`
- Removed Support for `DataEntityMapper` (Multiple Mapping)
- Bug Fixes: https://github.com/RepoDb/RepoDb/issues?q=is:issue+is:closed


### RepoDB (v1.6.4)

- Performance: Introduced the field definitions for NULL checks at IL. [#48](https://github.com/mikependon/RepoDb/issues/48)
- Performance: Added a compiled-functions (Expression) when converting the DataReader to Entity. FransBouma Recommendation #47


### RepoDB (v1.6.2)

- Performance: Introduced the field definitions for NULL checks at IL. [#48](https://github.com/mikependon/RepoDb/issues/48)
- Performance: Added a compiled-functions (Expression) when converting the DataReader to Entity. FransBouma Recommendation #47


### RepoDB (v1.6.0)

- Performance: Introduced the field definitions for NULL checks at IL. [#48](https://github.com/mikependon/RepoDb/issues/48)
- Performance: Added a compiled-functions (Expression) when converting the DataReader to Entity. FransBouma Recommendation #47


### RepoDB (v1.5.3)

- Optimization: This release has an extreme performance improvement. This is an update at v1.5.2.
- Bug: Fixed the packages.config dependencies issues.


### RepoDB (v1.5.2)

- Performance Optimization: This release has an extreme performance improvement.


### RepoDB (v1.5.0)

- Performance Optimization: This release has an extreme performance improvement.


### RepoDB (v1.3.5)

- Refactor: Removed the `DataEntity` base class (request from the community)
- Performance: Added a mechanism to cache the command texts
- Bug Fix: Exception is thrown at `Repository.Query` when `cacheKey` is present
- Bug Fix: Incorrect milliseconds is being saved for nullable `System.DateTime` properties


### RepoDB (v1.3.0)

- Refactor: Removed `DataEntity` - requested from the community
- Performance: Cached the command texts
- Bug Fix: Exception is thrown at `Repository.Query` when `cacheKey` is present
- Bug Fix: Incorrect milliseconds is being saved for nullable `System.DateTime` properties


### RepoDB (v1.2.0)

- Stable Release (v1.2.0)


### RepoDB (v1.2.0-beta5)

- Stabilization: Enabled the recursive query, recursion depth and cyclomatic stack overflow complexity features.


### RepoDB (v1.2.0-beta4)

- Stabilization: Enabled the Recursive `Query` feature.


### RepoDB (v1.2.0-beta3)

- Stabilizing: Added additional validator for query expressions.
- Stabilizing: Enabling the NULL values for [Field](/class/field) when composing a query expression.


### RepoDB (v1.2.0-beta2)

- Stabilizing: Enabled the (Field.Name = (object)null)
- Stabilizing: Enabled the Repository.Query if `PrimaryKey` is not Present


### RepoDB (v1.2.0-beta1)

- Beta Release 1


### RepoDB (v1.1.11)

- Supported multi-targeted framework (net40, netstandard1.3, netcore1.1)


### RepoDB (v1.1.10)

- Candidate for Beta Release


### RepoDB (v1.1.10-beta1)

- Supported multi-targeted framework (net40, netstandard1.3, netcore1.1)
- Beta release 1 for v1.2.0


### RepoDB (v1.1.9)

- Introduced the IDbConnection Extended Operational Methods.
- Optimized the `DbRepository` to use the IDbConnection Extended Operational Methods.
- Removes the `DbRepository` property at `BaseRepository` class.
- Made the `DbRepository` and `BaseRepository` Disposable.
- Introduced quoting on Fields and Tables when composing SQL statements (via SqlDbStatementBuilder).
- Documented the ConnectionPersistency, [DeleteAll](/operation/deleteall), InlineInsert, InlineMerge, InlineUpdate and [Truncate](/operation/truncate) operations.


### RepoDB (v1.1.8)

#### Updates for v1.1.7 and v1.1.8

- Supported identity primary key field identification from the database.
- Fixed the parallelism issues by removing the unnecessary cache classes from the library.
- Created a customized DataReader object for the [BulkInsert](/operation/bulkinsert) operation, for future support for the .Net Core.
- Introduced the repository [Truncate](/operation/truncate) operation.
- Supported the inline operations for [Insert](/operation/insert), [Merge](/operation/merge) and [Update](/operation/update).
- Added ConnectionPersistency capability for the repositories.
- Built on a lower target framework 4.0 for earlier compatibility.
- Next release is to support the .Net Core.


### RepoDB (v1.1.7)

- Supported identity primary key field identification from the database.
- Fixed the parallelism issues by removing the unnecessary cache classes from the library.
- Created a customized DataReader object for the [BulkInsert](/operation/bulkinsert) operation, for future support for the .Net Core.
- Introduced the repository [Truncate](/operation/truncate) operation.
- Supported the inline operations for [Insert](/operation/insert), [Merge](/operation/merge) and [Update](/operation/update).
- Added ConnectionPersistency capability for the repositories.
- Built on a lower target framework 4.0 for earlier compatibility.
- Next release is to support the .Net Core.


### RepoDB (v1.1.6)

- Supported identity primary key field identification from the database.
- Fixed the parallelism issues by removing the unnecessary cache objects from the library.
- Created a customized DataReader object for the [BulkInsert](/operation/bulkinsert) operation to support the .Net Core.
- Introduced the [Truncate](/operation/truncate) operation.
- Supported the inline operations for [Insert](/operation/insert), [Merge](/operation/merge) and [Update](/operation/update).
- Built on a lower target framework 4.0 for earlier compatibility.
- Next release is to support the .Net Core.


### RepoDB (v1.1.5)

- Built on a lower target framework 4.0 for earlier compatibility.
- Solution clean-up, removed interfaces that is not unnecessary for extensions.
- Updated the caching by adding the expiration feature in the CacheItem.
- Support identity primary field identification from the database.
- Next release is to support the .Net Core.


### RepoDB (v1.1.4)

- Built on a lower target framework 4.0 for earlier compatibility.
- Solution clean-up, removed interfaces that is not unnecessary for extensions.
- Updated the caching by adding the expiration feature in the CacheItem.
- Next release is to support the .Net Core.


### RepoDB (v1.1.3)

- Built on a target framework 4.0 for earlier compatibility
- Renamed CacheItem.Timestamp to CacheItem.CreatedDate
- Added CacheItem.IsExpired method
- Added CacheItem.Expiration property
- Removed ICacheItem
- Removed ITraceLog
- Removed ICancellableTraceLog
- Removed ITypeMap
- Removed IStatementBuilderMap
- Removed IQueryGroup
- Removed IQueryField
- Removed IParameter
- Removed IField
- Removed IOrderField
- Removed IDataEntityMap
- Removed IQueryBuilder
- Removed IDbRepository
- Removed IBaseRepository


### RepoDB (v1.1.2)

- Built on a target framework 4.0 for earlier compatibility
- Renamed CacheItem.Timestamp to CacheItem.CreatedDate
- Added CacheItem.IsExpired method
- Added CacheItem.Expiration property
- Removed ICacheItem
- Removed ITraceLog
- Removed ICancellableTraceLog
- Removed ITypeMap
- Removed IStatementBuilderMap
- Removed IQueryGroup
- Removed IQueryField
- Removed IParameter
- Removed IField
- Removed IOrderField
- Removed IDataEntityMap


### RepoDB (v1.1.1)

- Version 1.1.0


### RepoDB (v1.1.0)

- Version 1.1.0


### RepoDB (v1.0.20)

- Version 1.0.20


### RepoDB (v1.0.19)

- Version 1.0.19


### RepoDB (v1.0.18-beta01)

#### Updates
- Supported the `DbConnection`.ExecuteQuery<TEntity> method, to return the `IEnumerable` list of RepoDb.Interfaces.IDataEntity.
- IL Emit the conversion of System.Data.`DbDataReader` to System.Dynamic.DynamicObject when calling the `DbConnection`.ExecuteQuery method.


### RepoDB (v1.0.17-alpha3)

#### Updates

- Created a RepoDb.Reflection.ObjectConverter.
- Supported the `DbConnection`.ExecuteQuery<TEntity> method, to return the `IEnumerable` list of RepoDb.Interfaces.IDataEntity.

### Notes

- Next version will be the Beta version of the library.


### RepoDB (v1.0.17-alpha02)

#### Updates

- Created a RepoDb.Reflection.ObjectConverter.
- Supported the `DbConnection`.ExecuteQuery<TEntity> method, to return the `IEnumerable` list of RepoDb.Interfaces.IDataEntity.

### Notes

- Next version will be the Alpha version of the library.


### RepoDB (v1.0.16)

#### Updates

- Created a RepoDb.Reflection.ObjectConverter.
- Supported the `DbConnection`.ExecuteQuery<TEntity> method, to return the `IEnumerable` list of RepoDb.Interfaces.IDataEntity.

### Notes

- Next version will be the Alpha version of the library.


### RepoDB (v1.0.16-alpha-01)

#### Updates

- Created a RepoDb.Reflection.ObjectConverter.
- Supported the `DbConnection`.ExecuteQuery<TEntity> method, to return the `IEnumerable` list of RepoDb.Interfaces.IDataEntity.

### Notes

- Next version will be the Alpha version of the library.


### RepoDB (v1.0.15)

- Added RepoDb.Reflection.Delegates.DataReaderToEntityMapperDelegate
- Added RepoDb.Reflection.ConstructorInfoCache
- Added RepoDb.Reflection.DataReaderConverter
- Added RepoDb.Reflection.DelegateCache
- Added RepoDb.Reflection.DelegateFactory
- Added RepoDb.Reflection.MethodInfoCache
- Added RepoDb.Reflection.MethodInfoTypes
- Added RepoDb.Reflection.ReflectionFactory
- Added RepoDb.Reflection.TypeArrayCache
- Added RepoDb.Reflection.TypeCache
- Added RepoDb.Reflection.TypeTypes
- Added RepoDb.Attributes.CreateMethodInfoAttribute
- Returned IDataReader object when using the IDbConnection.ExecuteReader
- Fixed the IL Emitter when mapping DataReader to Null properties
- Added `ExecuteQuery` to IDbConnection extension
- Added BeforeExecuteQuery and AfterExecuteQuery trace methods
- Supported DataEntityMapper, DataEntityMap
- Supported the `DbRepository`.Count and `DbRepository`.CountBig operations
- Support Multi-Mapping for Class-Level


### RepoDB (v1.0.14)

- Reflection (IL Emitting)


### RepoDB (v1.0.13)

- Reflection (IL Emitting)


### RepoDB (v1.0.12)

- Same as RepoDB (v1.0.11)


## RepoDB (v1.0.11)

#### Updates

- Same as RepoDB (v1.0.10)

### Fixes

- Issue 2: `Operation.In` Exception is Thrown for Array Values
- Issue 1: Class Entity `Map` Attribute `PrimaryKey` Identification


### RepoDB (v1.0.10)

#### Updates

- Support Column-Based [Update](/operation/update) using Dynamics (new Repository.InlineUpdate operation)
- Supported `BatchQuery` Operation
- Supported [Field](/class/field)-Level Mappings
- Added the currently used IQueryBuilder on the `IStatementBuilder` methods
- Added QueryBuilderCache object
- Added ExecutionTime (Timespan) property in the TraceLog class
- Added CommandTypeCache object
- Cached the CommadType on every calls
- Removed the Create, Drop, Alter, Execute Command Enum Values (until being supported)
- Added ClassMapNameCache object
- Cache `Map`.Name on every calls
- Added PropertyCache object
- Supported Entity Property Caching
- Added PrimaryPropertyCache object
- Supported Entity `Primary` Property Caching
- Added ClassMapCache object
- Cached the `Map` attribute on every calls

### Fixes

- Issue 2: `Operation.In` Exception is Thrown for Array Values
- Issue 1: Class Entity `Map` Attribute `PrimaryKey` Identification


### RepoDB (v1.0.9)

- Renamed `ICache.Has` to `ICache.Contains`
- Removed `ICache.GetAll` and implement the `IEnumerable` interface instead
- Optimized the mapping for SqlBulkCopy for [BulkInsert](/operation/bulkinsert)


### RepoDB (v1.0.8)

- Fix the bug found when injecting the `IStatementBuilder` at the `BaseRepository`.
- Renamed argument name `orderFields` to `orderBy`.
- Renamed `ExecuteReaderEx` to [ExecuteReader](/operation/executereader) under Connection object.
- Added `Remove()` on the ICache
- Renamed ICache `Set()`  method to `Add()`
- Renamed `DbCacheItem` to `CacheItem`
- Remove the `sealed` keyword at `CacheItem` to make it inheritable


### RepoDB (v1.0.7)

#### Updates

- Support dynamic query objects for [QueryGroup](/class/querygroup)
- MemoryCache (ICache) object
- `Trace` (ITrace) object
- Added Constant class
- Added support for Operation.Like and Operation.NotLike
- Allow Querying, Deleting, Updating by `PrimaryKey` (when the value is passed in the method of WHERE argument)
- Support of Operation.Between and Operation.NotBetween
- Support `Operation.In` and Operation.NotIn
- Optimized Statement Builder (SqlDbStatementBuilder)
- Injectable Statement Builder
- Support TOP and ORDER BY
- Order.Ascending and Order.Descending
- Support StatementBuilderMapper, IStatementBuilderMapper, StatementBuilderMap, StatementBuilderMap
- Support ORDER BY parsing of the dynamic objects
- Added support for the new Operation.Any and Operation.All

#### Removed

- EventNotifier class has been obsolete by the `Trace` class


### RepoDB (v1.0.6)

#### Updates

- Support dynamic query objects for [QueryGroup](/class/querygroup)
- MemoryCache (ICache) object
- `Trace` (ITrace) object
- Added Constant class
- Added support for Operation.Like and Operation.NotLike
- Allow Querying, Deleting, Updating by `PrimaryKey` (when the value is passed in the method of WHERE argument)
- Support of Operation.Between and Operation.NotBetween
- Support `Operation.In` and Operation.NotIn
- Optimized Statement Builder (SqlDbStatementBuilder)
- Injectable Statement Builder
- Support TOP and ORDER BY
- Order.Ascending and Order.Descending
- Support StatementBuilderMapper, IStatementBuilderMapper, StatementBuilderMap, StatementBuilderMap
- Support ORDER BY parsing of the dynamic objects
- Added support for the new Operation.Any and Operation.All

#### Removed

- EventNotifier class has been obsolete by the `Trace` class


### RepoDB (v1.0.5)

#### Updates

- EntityNotBulkInsertableException supported when calling [BulkInsert](/operation/bulkinsert) with non SqlConnection connection object
- [BulkInsert](/operation/bulkinsert) optimization - ordering the columns based on the DB Table ordering (not on `DataEntity` properties ordering)
- Initial implementation for complex query ([QueryGroup](/class/querygroup))
- Added [QueryGroup](/class/querygroup) (IQueryGroup)
- Added Conjuctions for [QueryGroup](/class/querygroup)(s)
- Added OrQueryGroup
- Added AndQueryGroup
- Supported IFieldValue interface for [QueryField](/class/queryfield) - to support the [QueryGroup](/class/querygroup) parameterized approach
- Renamed [QueryField](/class/queryfield).Value to [QueryField](/class/queryfield).Parameter (with Name and Value properties) and change its Type from object to IParameter
- In QueryFields, if the Operation is `=` and the parameter Value is equals to NULL then we compose ([Field] IS NULL) string statement
- Solves the problem of: WHERE (SomeDate IS NULL)
- We also did the same thing for != (SomeDate IS NOT NULL)
- Used the `<>` instead of `!=` in InEquality comparer
- Supported EventNotifier (Tracing and Debugging purposes).
- You can listen on the following events to see the Statement and Object passed before DB executions
- BeforeQueryExecution
- AfterQueryExecution
- BeforeUpdateExecution
- AfterUpdateExecution
- BeforeDeleteExecution
- AfterDeleteExecution
- BeforeMergeExecution
- AfterMergeExecution
- BeforeInsertExecution
- AfterInsertExecution
- BeforeBulkInsertExecution
- AfterBulkInsertExecution
- BeforeExecuteNonQueryExecution
- AfterExecuteNonQueryExecution
- BeforeExecuteReaderExecution
- AfterExecuteReaderExecution
- BeforeExecuteScalarExecution
- AfterExecuteScalarExecution
- CancelledExecution


### RepoDB (v1.0.4)

- Bug Fix: Error when converting the SqlDataReader data back to the class object when the value is DBNull.Value
- Minor code optimizations and refactoring


### RepoDB (v1.0.3)

- Bug Fix: Error when converting the SqlDataReader data back to the class object when the value is DBNull.Value
- Minor code optimizations and refactoring


### RepoDB (v1.0.2)

- Converting DataReader to Object
- `Async` Calls (Task.Factory.StartNew)
- Added support to auto find (Id) property as prospected `PrimaryKey` if the [Primary] attribute is not on place


### RepoDB (v1.0.1)

- Initial Release for RepoDB (.Net Extension)
- Supported Dynamic `DbConnection`
- Supported Mapping Command Type (Entity Level)
- Supported ExecuteScalar, ExecuteNonQuery, ExecuteReader (DataEntity and ExpandoObject)
- Supported `Primary` Attribute (IsIdentity)
- Supported `BaseRepository` that uses the functionality of the `DbRepository`
- Supported the GetSqlStatement (Entity Level)
- Supported Object Driven approach when doing a query, delete, update and merge
- Supported [Merge](/operation/merge) Method (Entity Level only)
- Supported Bulk [Insert](/operation/insert) (SqlBulkCopy only)
- Supported to get the Connection at all Repositories
- Supported Transaction Handlers
- Supported `Async` methods
- Supported `DbRepository` property at the `BaseRepository`
- Supported Dynamic object returns for ExecuteReaderEx
- Supported code-guards at the `DbRepository` (Queryable, Insertable, Deletable, Mergeable, Updateable)
- Supported Type Mapper


### RepoDB (v1.0.0)

- Initial Release for RepoDB (.Net Extension)
- Supported Dynamic `DbConnection`
- Supported Mapping Command Type (Entity Level)
- Supported Execute Scalar
- Supported `Primary` Attribute (IsIdentity)
- Supported `BaseRepository` that uses the functionality of the `DbRepository`
- Supported the GetSqlStatement (Entity Level)
- Supported Object Driven approach when doing a query, delete, update and merge
- Supported [Merge](/operation/merge) Method (Entity Level only)
- Supported Bulk [Insert](/operation/insert) (SqlBulkCopy only)
- Supported to get the Connection at all Repositories
- Supported Transaction Handlers
- Supported `Async` methods
- Supported `DbRepository` property at the `BaseRepository`
- Supported Dynamic object returns for ExecuteReaderEx
- Supported code-guards at the `DbRepository` (Queryable, Insertable, Deletable, Mergeable, Updateable)
- Supported Type Mapper
