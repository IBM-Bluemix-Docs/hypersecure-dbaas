---

copyright:
  years: 2017
lastupdated: "2017-12-08"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}


# Database user operation commands

These are the database user operation commands:

- [user-create](#user_create)
- [user-list](#user_list)
- [user-show](#user_show)
- [user-delete](#user_delete)


## <a id="user_create"></a>user-create command

### Description

Creates one or more database users.

### Usage

**user-create** *cluster_id* *database.username* *password* \[*db_name* \[*db_name* ...\]\]

| Parameter        |  Description                  |
| :--------------- |  :--------------------------- |
| *cluster_id*     |  The ID of the cluster        |
| *database.username* | The authentication database name and a username to create, separated by a period |
| *password*       | The login password for this user. |
| *db_name*        | An optional parameter specifying the name of a database for which the user will have read and write access |


## <a id="user_list"></a>user-list command

### Description

Lists all the database users.

### Usage

**user-list** *cluster_id*

| Parameter        |  Description                  |
| :--------------- |  :--------------------------- |
| *cluster_id*    |  The ID of the cluster       |


## <a id="user_show"></a>user-show command

### Description

Shows details about a database user.

### Usage

**user-show** *cluster_id* *database.username*

| Parameter        |  Description                  |
| :--------------- |  :--------------------------- |
| *cluster_id*    |  The ID of the cluster       |
| *database.username* | The authentication database name and the user name, separated by a period |


## <a id="user_delete"></a>user-delete command

### Description

Deletes a database user.

### Usage

**user-delete** *cluster_id* *database.username*

| Parameter        |  Description                  |
| :--------------- |  :--------------------------- |
| *cluster_id*    |  The ID of the cluster       |
| *database.username* | The authentication database name and the user name, separated by a period |
