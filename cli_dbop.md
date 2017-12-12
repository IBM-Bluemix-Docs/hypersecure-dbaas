---

copyright:
  years: 2017
lastupdated: "2017-12-08"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}


# Database operation commands

These are the database operation commands:

- [database-create](#database_create)
- [database-list](#database_list)
- [database-delete](#database_delete)

## <a id="database_create"></a>database-create command

### Description

Creates a database. For MongoDB, a collection must also be created with the database.

### Usage

**database-create** *cluster_id* *database* *collection*

| Parameter        |  Description                 |
| :--------------- |  :---------------------------|
| *cluster_id*     |  The ID of the cluster       |
| *database*       |  The database name to create |
| *collection*     |  The collection name to create |


## <a id="database_list"></a>database-list command

### Description

Lists all the databases on the given cluster.

### Usage

**database-list** *cluster_id*

| Parameter        |  Description                 |
| :--------------- |  :---------------------------|
| *cluster_id*     |  The ID of the cluster       |


## <a id="database_delete"></a>database-delete command

### Description

Deletes a database.

### Usage

**database-delete** *cluster_id* *database*

| Parameter        |  Description                 |
| :--------------- |  :---------------------------|
| *cluster_id*     |  The ID of the cluster       |
| *database*       |  The name of the database to delete. | 
