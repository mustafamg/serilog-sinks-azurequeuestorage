
23-NOV-2018 Implementation of an Azure storage queue sink based off the Azure table storage sink:
            https://github.com/serilog/serilog-sinks-azuretablestorage

            Certain functionality/code removed from the queue sink likely needs to be restored
            (this was built in less than a day to address a particular scenario).
            
            Usage:
            
            Usage follows Serilog.Sinks.AzureTableStorage except:
            - "WriteTo" is AzureQueueStorage instead of AzureTableStorage
            - "storageTableName" is "storageQueueName" (and use an existing queue's name as a parameter)
            
            "connectionString" is still a valid storage account connection string, in this case where the queue is defined.
            