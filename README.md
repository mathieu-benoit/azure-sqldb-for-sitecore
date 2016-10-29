This sample allows to create the 4 empty Azure Sql Databases. It's dedicated to create the 4 required (at least) databases for Sitecore but could be adapted for other considerations.

Furthermore, this sample is part of [one of my blog about restoring the 4 Sitecore databases via Visual Studio Team Services](https://alwaysupalwayson.blogspot.ca/2016/09/use-azure-sql-database-deployment-task.html).

The project/folder "ManageAzureSqlDatabasesAzureResourceGroup" consists on 2 files:
- CreateSitecoreAzureSqlDatabasesAndServer.ps1 - the powershell script to run to create the Azure Sql Databases and their associated server.
- CreateSitecoreAzureSqlDatabasesAndServer.json - the template as input for the above powershell script.
