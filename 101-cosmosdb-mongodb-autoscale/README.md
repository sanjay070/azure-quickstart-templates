# Create an Azure Cosmos account for MongoDB API (3.2 or 3.6) with autoscale shared database throughput with two collections

![Azure Public Test Date](https://azurequickstartsservice.blob.core.windows.net/badges/101-cosmosdb-mongodb-autoscale/PublicLastTestDate.svg)
![Azure Public Test Result](https://azurequickstartsservice.blob.core.windows.net/badges/101-cosmosdb-mongodb-autoscale/PublicDeployment.svg)

![Azure US Gov Last Test Date](https://azurequickstartsservice.blob.core.windows.net/badges/101-cosmosdb-mongodb-autoscale/FairfaxLastTestDate.svg)
![Azure US Gov Last Test Result](https://azurequickstartsservice.blob.core.windows.net/badges/101-cosmosdb-mongodb-autoscale/FairfaxDeployment.svg)

![Best Practice Check](https://azurequickstartsservice.blob.core.windows.net/badges/101-cosmosdb-mongodb-autoscale/BestPracticeResult.svg)
![Cred Scan Check](https://azurequickstartsservice.blob.core.windows.net/badges/101-cosmosdb-mongodb-autoscale/CredScanResult.svg)

This template creates an Azure Cosmos account for MongoDB API, provisioned for two regions, then provision a database with autoscale throughput shared across 2 collections.

Below are the parameters which can be user configured in the parameters file or template including:

- **Consistency Level:** Select from one of the 5 consistency levels: Strong, Bounded Staleness, Session, Consistent Prefix, Eventual.
- **Primary Region:** Enter location for the primary region.
- **Secondary Region:** Enter location for the secondary region.
- **Automatic Failover:** Select whether to enable automatic failover on the account
- **Database Name:** Enter the database name for the account.
- **Server Version:** Select the MongoDB server version (default is 3.6).
- **Collection 1 Name:** Enter the name for the first collection.
- **Collection 2 Name:** Enter the name for the second collection.
- **Throughput Policy:** Select Manual or Autoscale throughput policy.
- **Manual Provisioned Throughput:** Enter the shared RU/s for the database when Throughput Policy is Manual (default 400).
- **Max Autoscale Throughput:** Enter the shared maximum RU/s for the database when Throughput Policy is Autoscale (default 4000).

[![Deploy To Azure](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2F101-cosmosdb-mongodb-autoscale%2Fazuredeploy.json)  [![Visualize](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.svg?sanitize=true)](http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2F101-cosmosdb-mongodb-autoscale%2Fazuredeploy.json)
