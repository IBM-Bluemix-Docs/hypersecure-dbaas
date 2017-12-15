---

copyright:
  years: 2017
lastupdated: "2017-12-15"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Getting started with IBM HyperSecure DBaaS
{: #gettingstarted}

{{site.data.keyword.ihsdbaas_full}} is an {{site.data.keyword.cloud}} service that provides databases on demand.
It offers a flexible and scalable platform that allows you to quickly and easily
provision and manage your database of choice.
{: shortdesc}

This {{site.data.keyword.cloud_notm}} offering provides MongoDB database clusters. Each database
cluster comprises one primary database instance and two database instance
replicas that back up the primary one.

With {{site.data.keyword.ihsdbaas_full}}, you can create database clusters in the {{site.data.keyword.cloud_notm}},
manage database instances, administer database users, and create and
monitor databases.

## Data security and privacy

{{site.data.keyword.IBM}} hosts your databases in a highly available and secure environment:
<ul>
<li>The underlying technologies prevent {{site.data.keyword.IBM_notm}} or a third party from being able to
access your data.
<p>The Secure Service Container (SSC) technology protects the system via a
tamper-proof environment. Access to the system is restricted and is only enabled
through well-defined RESTful APIs.</p></li>
<li>Data is encrypted at rest and in flight.</li>
<li>The system hardware, the system configuration, and the database setup ensure
high availability.</li>
</ul>

##Creating a database cluster

To create a database cluster, you simply enter the required values in the
IBM HyperSecure DBaaS catalog details view and click **Create**.

After you have created the database cluster, {{site.data.keyword.IBM}} provides you the hostname and the port
numbers of the three created database instances. You can now use this information
and the user credentials you specified in the catalog to create and access your
databases.

##Managing the database cluster

In a database cluster, you can create databases, manage the database instances,
create or delete users, and get the database logs.

{{site.data.keyword.ihsdbaas_full}} provides the DBaaS Manager, which manages and
intelligently schedules your requests based on the available resources.

You can address requests to the DBaaS Manager through one of these interfaces:
<ul>
<li>The Web User Interface</li>
<li>The RESTful API</li>
<li>The command-line interface (CLI)</li>
</ul>

## Accessing the database

After creating a database, you can use the mongo shell, your favorite
MongoDB driver, or tools like MongoDB Compass to manage the database itself.

The IBM HyperSecure DBaaS dashboard provides the necessary information to connect to a database.
You can copy the provided mongo shell command to your clipboard,
insert the Database Admin Name as --username option,
the Database Admin Password as --password option,
and add the options --ssl and --sslAllowInvalidCertificates for a secure data transfer
to set up the MongoDB tools accordingly.
