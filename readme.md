# SQL Team Repository
All sql related documentation and ***sample sql code*** are managed using this repository.

Below is the beloved sql code.

```sql
select * from sys.index_resumable_operations 
```

or Powershell
```PowerShell   
    $SubscriptionID = '0e6e9ede-e794-4d39-bd16-cdc402faee39'
    Connect-AzAccount | Out-Null
    $AuthHeader = Get-AuthHeader -SubscriptionID $SubscriptionID
    $ResourceListUri = "https://management.azure.com/subscriptions/$SubscriptionID/resources?api-version=2021-04-01"
    $Resources = (Invoke-RestMethod -URI $ResourceListUri -Method Get -Headers $authHeader -verbose:$false).Value
    $Resources

```

 Use this repo for;
 1. documentation purposes
 1. sample queries
 1. for fun