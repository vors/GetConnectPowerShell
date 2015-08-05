# GetConnectPowerShell

PowerShell module that provides an API for http://getconnect.io/

## Getting started

### Initialize API keys

```powershell
Set-ConnectApiKey -ProjectId <Project Id (short string)> -KeyType PushQuery -ApiKey <Push/Query API key (long string)>
```

### Push events

```powershell
Push-ConnectEvent -CollectionName test-collection -event @{
  customer = @{
    firstName = 'Tom'
    lastName = 'Smith'
  }
  id = '1849506679'
  product = '12 red roses'
  purchasePrice = '34.95'
}
```

### Export events

```powershell
Get-ConnectEvents -CollectionName test-collection
```
