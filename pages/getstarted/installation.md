---
layout: default
sidebar: getstarted
title: "Installation of Nuget Packages"
description: "Learn on how to install RepoDB library on your Project/Solution."
permalink: /tutorial/installation
tags: [repodb, tutorial, installation, orm, hybrid-orm, sqlserver, sqlite, mysql, postgresql]
parent: TUTORIAL
---

# Installation

The packages can be installed using the Package Manager Console window.

### Raw SQLs

If you wish to work only with raw-SQLs.

```csharp
> Install-Package RepoDb
```

> It supports all kinds of RDBMS data providers.

### SQL Server

If you wish to work with [SQL Server](https://www.nuget.org/packages/RepoDb.SqlServer).

```csharp
> Install-Package RepoDb.SqlServer
```

Or, if you are to work with the bulk operations.

```csharp
> Install-Package RepoDb.SqlServer.BulkOperations
```

Then, call the bootstrapper to initialize the needed references.

```csharp
RepoDb.SqlServerBootstrap.Initialize();
```

### SQLite (System)

If you wish to work with [SQLite](https://www.nuget.org/packages/RepoDb.SQLite.System).

```csharp
> Install-Package RepoDb.SQLite.System
```

Then, call the bootstrapper to initialize the needed references.

```csharp
RepoDb.SQLiteBootstrap.Initialize();
```

### SQLite (Microsoft)

If you wish to work with [SQLite](https://www.nuget.org/packages/RepoDb.Sqlite.Microsoft).

```csharp
> Install-Package RepoDb.Sqlite.Microsoft
```

Then, call the bootstrapper to initialize the needed references.

```csharp
RepoDb.SqliteBootstrap.Initialize();
```

### MySQL

If you wish to work with [MySQL](https://www.nuget.org/packages/RepoDb.MySql).

```csharp
> Install-Package RepoDb.MySql
```

Then, call the bootstrapper to initialize the needed references.

```csharp
RepoDb.MySqlBootstrap.Initialize();
```

### MySqlConnector

If you wish to work with [MySQL](https://www.nuget.org/packages/RepoDb.MySqlConnector).

```csharp
> Install-Package RepoDb.MySqlConnectorBootstrap.Initialize();
```

Then, call the bootstrapper to initialize the needed references.

```csharp
RepoDb.MySqlBootstrap.Initialize();
```

### PostgreSQL

If you wish to work with [PostgreSQL](https://www.nuget.org/packages/RepoDb.PostgreSql).

```csharp
> Install-Package RepoDb.PostgreSql
```

Then, call the bootstrapper to initialize the needed references.

```csharp
RepoDb.PostgreSqlBootstrap.Initialize();
```

> Please visit our [documentation](/docs) page to learn more about this library.
