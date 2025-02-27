# Azure-Event-Hubs
Serverless functions test lab on an outdated version of .NET 

## Create resources 
1. Create RG
az group create -l canadacentral -n cst8921
**Canada central works for all resources**

2. Create Resources

```bash
az deployment group create --resource-group cst8921 --template-uri https://raw.githubusercontent.com/Azure/azure-docs-json-samples/master/event-grid/EventHubsDataMigration.json --parameters eventHubNamespaceName=event-hub-kari0117 eventHubName=hubdatamigration sqlServerName=kari0117-sql-server sqlServerUserName=kariuki sqlServerPassword=Secur3Passw0rd! sqlServerDatabaseName=database-kari0117 storageName=k4ristore functionAppName=k4rifx
```
3. Publishing the code using Visual studio

