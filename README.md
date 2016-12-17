 This sample allows to create the 4 empty Azure Sql Databases on an Elastic Pool by ARM Template deployment. It's dedicated to create the 4 required (at least) databases for Sitecore but could be adapted for other considerations.

Furthermore, this sample is part of [one of my blog about restoring the 4 Sitecore DACPACs via Visual Studio Team Services (VSTS)](https://alwaysupalwayson.blogspot.ca/2016/09/use-azure-sql-database-deployment-task.html).

The project/folder "ManageAzureSqlDatabasesAzureResourceGroup" consists on 2 files:
- [CreateSitecoreAzureSqlDatabasesAndServer.ps1](/ManageAzureSqlDbAzureResourceGroup/CreateSitecoreAzureSqlDatabasesAndServer.ps1) - the powershell script to run to create the Azure Sql Databases and their associated server.
- [CreateSitecoreAzureSqlDatabasesAndServer.json](/ManageAzureSqlDbAzureResourceGroup/CreateSitecoreAzureSqlDatabasesAndServer.json) - the template as input for the above powershell script.

If you have an Azure Account you could also use the following button to use the Azure Template Deployment tool (this will just create the Azure services but won't restore the databases. Restoring the dacpacs is part of the VSTS tasks):

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fmathieu-benoit%2Fazure-sqldb-for-sitecore%2Fmaster%2FManageAzureSqlDbAzureResourceGroup%2FCreateSitecoreAzureSqlDatabasesAndServer.json" target="_">![Deploy to Azure](http://azuredeploy.net/deploybutton.png)</a>
