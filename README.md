# azure-cosmos-change-feed-gremlin

Consume the CosmosDB/Gremlin Change Feed with an Azure Function

## Steps to Create, Test, Deploy

- Provision an Azure CosmosDB account, with Graph/Gremlin API
- Created a graph named **npm** in the **dev** database in CosmosDB, with partition key **/pk**
- Create an Azure Functions App on your workstation in Visual Studio
  - I used VS for macOS
  - Created a a new Azure Functions project called **CosmosGremlinTrigger**
  - Added minor edits to **CosmosGremlinTrigger.cs** to iterate the docs and log them as JSON.
  - Added the following line to **CosmosGremlinTrigger.cs** to automatically create the **leases** collection:
```
CreateLeaseCollectionIfNotExists = true,
```
- Build the project on the command line:
```

```

- Note: Previous sample Graph App here, but unrelated to this **azure-cosmos-change-feed-gremlin** repo:
  - https://github.com/Azure-Samples/azure-cosmos-db-graph-npm-bom-sample


## Create the Project

