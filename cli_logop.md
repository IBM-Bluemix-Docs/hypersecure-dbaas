---

copyright:
  years: 2017
lastupdated: "2017-12-08"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}

## Log operation commands

These are the log operation commands:

- [log-list](#log_list)
- [log-get](#log_get)


## <a id="log_list"></a>log-list command

### Description

Lists all the log files on an instance.

### Usage

**log-list** *instance_id*

| Parameter        |  Description                  |
| :--------------- |  :--------------------------- |
| *instance_id*    |  The ID of the instance       |


## <a id="log_get"></a>log-get command

### Description

Downloads a log file from an instance.

### Usage

**log-get** *instance_id* *filename*

| Parameter        |  Description                  |
| :--------------- |  :--------------------------- |
| *instance_id*    |  The ID of the instance       |
| *filename*       |  The name of the log file to download |
