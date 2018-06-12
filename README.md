# Azure Table Operations
This code shows how to add entities to azure table and also how to get the table entities.

## How to Add entities?

You will need to have an azure storage account, you also need to create the table storage.

If you have all of above you can start by referencing `azure-storage.table.js` file in the HTML and jquery.

Get the token `'https://' + 'azurestorageacount' + '.azurewebsites.net/api/Key/' + 'table_endpoint'`

Define the tableUri then use it with the token that you get from azure api:

`var tableService = AzureStorage.Table.createTableServiceWithSas(tableUri, token);`

If you are adding objects you will have to stringfy them using `JSON.stringfy` method.

To get the clear idea you can check the `addTableEntity` on my code.

## How to get entities?


Check the `getTableEntity` function.

get more information [here](https://docs.microsoft.com/en-us/azure/cosmos-db/table-storage-overview)