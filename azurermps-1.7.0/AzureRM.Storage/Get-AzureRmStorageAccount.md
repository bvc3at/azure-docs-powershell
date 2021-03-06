---
external help file: Microsoft.Azure.Commands.Management.Storage.dll-Help.xml
ms.assetid: E6A13F25-4565-4AB1-8690-A292C89C9C43
online version: 
schema: 2.0.0
---

# Get-AzureRmStorageAccount

## SYNOPSIS
Gets a Storage account.

## SYNTAX

### AccountNameParameterSet
```
Get-AzureRmStorageAccount [-ResourceGroupName] <String> [-Name] <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

### ResourceGroupParameterSet
```
Get-AzureRmStorageAccount [[-ResourceGroupName] <String>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmStorageAccount** cmdlet gets a specified Storage account or all of the Storage accounts in a resource group or the subscription.

## EXAMPLES

### Example 1: Get a specified storage account
```
PS C:\>Get-AzureRmStorageAccount -ResourceGroupName "RG01" -AccountName "MyStorageAccount"
```

This command gets the specified Storage account.

### Example 2: Get all Storage accounts in a resource group
```
PS C:\>Get-AzureRmStorageAccount -ResourceGroupName "RG01"
```

This command gets all of the Storage accounts in a resource group.

### Example 3:  Get all Storage accounts in the subscription
```
PS C:\>Get-AzureRmStorageAccount
```

This command gets all of the Storage accounts in the subscription.

## PARAMETERS

### -InformationAction
Specifies how this cmdlet responds to an information event.

The acceptable values for this parameter are:

- Continue
- Ignore
- Inquire
- SilentlyContinue
- Stop
- Suspend

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Specifies an information variable.

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the Storage account to get.

```yaml
Type: String
Parameter Sets: AccountNameParameterSet
Aliases: StorageAccountName, AccountName

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group that contains the Storage account to get.

```yaml
Type: String
Parameter Sets: AccountNameParameterSet
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: ResourceGroupParameterSet
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzureRmStorageAccount](./New-AzureRmStorageAccount.md)

[Remove-AzureRmStorageAccount](./Remove-AzureRmStorageAccount.md)

[Set-AzureRmStorageAccount](./Set-AzureRmStorageAccount.md)


