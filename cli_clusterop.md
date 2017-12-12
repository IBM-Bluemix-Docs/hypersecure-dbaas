---

copyright:
  years: 2017
lastupdated: "2017-12-12"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}


# Cluster operation commands

These are the cluster operation commands:

- [cluster-create](#cluster_create)
- [cluster-list](#cluster_list)
- [cluster-show](#cluster_show)
- [cluster-delete](#cluster_delete)

## <a id="cluster_create"></a>cluster-create command

### Description

Creates a database cluster.

The command returns immediately with cluster status of BUILD. After about 30 seconds, a cluster status of RUNNING becomes available. To get the updated cluster status, run the [cluster-list](#cluster_list) or [cluster-show](#cluster_show) command.

This command requires that you accept the IBM license. Therefore, when issuing the command, preface it with the **\./dmclient --accept-license** option, as in this example:

```
**\./dmclient --accept-license cluster-create myClusterName user password**
```

### Usage

**cluster-create** *cluster_name* *admin_name* *admin_password*

| Parameter        |  Description                                                    |
| :--------------- |  :------------------------------------------------------------- |
| *cluster_name*   |  The cluster name to create                                     |
| *admin_name*     |  The database administrator name to manage the database cluster |
| *admin_password* |  The password of database administrator                         |

## <a id="cluster_list"></a>cluster-list command

### Description

Lists all the clusters that have been created.

### Usage
**cluster-list**

The command has no parameters.

## <a id="cluster_show"></a>cluster-show command

### Description

Shows the details of the specified cluster, including information about each replica member.  

### Usage
**cluster-show** *cluster_id*

| Parameter        |  Description                                                    |
| :--------------- |  :------------------------------------------------------------- |
| *cluster_id*     |  The ID of the cluster, as shown in the [cluster-list](#cluster_list) command |


## <a id="cluster_delete"></a>cluster-delete command

### Description

Deletes a cluster. Once the cluster is deleted, all the data is lost.

### Usage

**cluster-delete** *cluster_id*

| Parameter        |  Description                                                    |
| :--------------- |  :------------------------------------------------------------- |
| *cluster_id*     |  The ID of the cluster, as shown in the [cluster-list](#cluster_list) command |
