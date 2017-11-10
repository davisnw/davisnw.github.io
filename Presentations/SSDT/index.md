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