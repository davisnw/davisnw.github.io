---
layout: page
---

# SSDT
Sql Server Data Tools (SSDT) provides a database project for managing Sql Server Databases. To my knowledge, it only supports Sql Server (or Azure variants thereof).
SSDT appears to be available with any valid Visual Studio license, including Community Edition.

These notes are based on Visual Studio 2017 version 15.4.3 and SSDT version 15.1.61707.200 on Windows 10.

# Installing SSDT
There are several different ways to get SSDT, including downloading directly from Microsoft.com [Download SQL Server Data Tools (SSDT)](https://docs.microsoft.com/en-us/sql/ssdt/download-sql-server-data-tools-ssdt). Note that this page may include preview versions.

However, in my experience the most reliable means to get SSDT is to use the Visual Studio 2017 installer. If you already have Visual Studio 2017 installed, one way to launch it is to:
 * go to "Apps and Features"
 * locate the entry for "Microsoft Visual Studio 2017"
 * click "Modify"
 * Once the visual studio installer launches, select the product you have installed, and click "Modify".  You should then be presented with "workloads".

 Alternately, just re-downloading the Visual Studio 2017 installer and launching it should also work.

 Once you have "workloads" up:
  * Select the "Data storage and processing" workload
  * Then select "Sql Server Data Tools"
  ![alt text](SSDTWorkloadInstall.png "SSDT Workload Install")

# Importing a database with SSDT
If you already have a database that you now want to bring into SSDT, you can easily import its schema into a database project.  This provides several advantages including easy integration with source control and database object validity checks - we will explore these in more detail later.

To import a database schema into a new project you can use the following steps:
 1. Create a new database project ![alt text](NewSSDTProject.png "New SSDT Project")
 1. Right-click the database project, choose "Import" and "Database" ![alt text](ImportDatabase1.png "Import Database 1")
 1. Fill out the database connection, choose the import options, and click start ![alt text](ImportDatabase2.png "Import Database 2")
	* Note: There are several different options for the default structure of the files in the imported project.  I generally prefer "Schema\Object", but afterwards manually move the schema create script under each schema folder.  SSDT actually doesn't care how the files are structured - it only requires that the create scripts be valid.
 1. You now have a database project that you can commit to source control, just like any other source code.  With the import options shown in the previous screen shot, Schemas will be under the "Security" folder, and each object will be in a folder corresponding to the schema name with sub-folders per "major" db object type. Again, you can re-arrange folder structures however you wish. ![alt text](ImportDatabase3.png "Import Database 3")

# Building database projects

# Extended Properties (and data dictionary)

# Schema Comparison and Syncing

# Refactor Log

# Project properties

# SSDT Variables and Sql Command

# Database References

# "End State" Deployment and data management

# Generating Scripts with Publish

# Generating Scripts with Schema Compare

# Publishing with dacpac

# Column Ordering

# A note on source control

# Integrating with automated builds

# A note on EF / ORM syncing

# Pre and Post deployment scripts

# Sql Server CLR

# Data Comparison

# Static Data

# Tsql Code Analysis