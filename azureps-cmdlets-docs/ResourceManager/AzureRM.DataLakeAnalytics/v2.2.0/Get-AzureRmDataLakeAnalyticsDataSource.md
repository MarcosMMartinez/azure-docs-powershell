---
external help file: Microsoft.Azure.Commands.DataLakeAnalytics.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: AE303B81-6754-40DD-9B53-19A2D4893832
---

# Get-AzureRmDataLakeAnalyticsDataSource

## SYNOPSIS
Gets a Data Lake Analytics data source.

## SYNTAX

### List all data sources (Default)
```
Get-AzureRmDataLakeAnalyticsDataSource [-Account] <String> [[-ResourceGroupName] <String>] [<CommonParameters>]
```

### Get a Blob storage account
```
Get-AzureRmDataLakeAnalyticsDataSource [-Account] <String> [-Blob] <String> [[-ResourceGroupName] <String>]
 [<CommonParameters>]
```

### Get a Data Lake Store account
```
Get-AzureRmDataLakeAnalyticsDataSource [-Account] <String> [-DataLakeStore] <String>
 [[-ResourceGroupName] <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmDataLakeAnalyticsDataSource** cmdlet gets an Azure Data Lake Analytics data source.

## EXAMPLES

### Example 1: Get a data source from an account
```
PS C:\>Get-AzureRmDataLakeAnalyticsDataSource -AccountName "ContosoAdlA" -DataLakeStore "ContosoAdls"
```

This command gets a Data Lake Store data source named ContosoAdls from a Data Lake Analytics account.

### Example 2: Get the list of Data Lake Store accounts in a Data Lake Analytics account
```
PS C:\>Get-AzureRmDataLakeAnalyticsDataSource -AccountName "ContosoAdlA" -DataSource "DataLakeStore"
```

This command gets all Data Lake Store accounts from a Data Lake Analytics account.

## PARAMETERS

### -Account
Specifies the Data Lake Analytics account that this cmdlet gets data sources.

```yaml
Type: String
Parameter Sets: (All)
Aliases: AccountName

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the resource group name that contains the data source.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DataLakeStore
Specifies the name of the Data Lake Store account.

```yaml
Type: String
Parameter Sets: Get a Data Lake Store account
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Blob
Specifies the name of the Azure Blob Storage data source.

```yaml
Type: String
Parameter Sets: Get a Blob storage account
Aliases: AzureBlob

Required: True
Position: 1
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

[Add-AzureRmDataLakeAnalyticsDataSource](./Add-AzureRmDataLakeAnalyticsDataSource.md)

[Remove-AzureRmDataLakeAnalyticsDataSource](./Remove-AzureRmDataLakeAnalyticsDataSource.md)

[Set-AzureRmDataLakeAnalyticsDataSource](./Set-AzureRmDataLakeAnalyticsDataSource.md)


