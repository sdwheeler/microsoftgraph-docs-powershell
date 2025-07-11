---
external help file: Microsoft.Graph.Reports-help.xml
Module Name: Microsoft.Graph.Reports
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.reports/new-mgreportpartnerbillingmanifest
schema: 2.0.0
---

# New-MgReportPartnerBillingManifest

## SYNOPSIS
Create new navigation property to manifests for reports

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaReportPartnerBillingManifest](/powershell/module/Microsoft.Graph.Beta.Reports/New-MgBetaReportPartnerBillingManifest?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgReportPartnerBillingManifest [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-BlobCount <Int32>] [-Blobs <IMicrosoftGraphPartnersBillingBlob[]>] [-CreatedDateTime <DateTime>]
 [-DataFormat <String>] [-ETag <String>] [-Id <String>] [-PartitionType <String>] [-PartnerTenantId <String>]
 [-RootDirectory <String>] [-SasToken <String>] [-SchemaVersion <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgReportPartnerBillingManifest -BodyParameter <IMicrosoftGraphPartnersBillingManifest>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to manifests for reports

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BlobCount
The total file count for this partner tenant ID.

```yaml
Type: Int32
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Blobs
A collection of blob objects that contain details of all the files for the partner tenant ID.
To construct, see NOTES section for BLOBS properties and create a hash table.

```yaml
Type: IMicrosoftGraphPartnersBillingBlob[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
manifest
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphPartnersBillingManifest
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreatedDateTime
The date and time when a manifest resource was created.
The timestamp type represents date and time information using ISO 8601 format and is always in UTC.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DataFormat
The billing data file format.
The possible value is: compressedJSONLines.
Each blob is a compressed file and data in the file is in JSON lines format.
Decompress the file to access the data.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ETag
Version of data represented by the manifest.
Any change in eTag indicates a new data version.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Headers
Optional headers that will be added to the request.

```yaml
Type: IDictionary
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Id
The unique identifier for an entity.
Read-only.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PartitionType
Indicates the division of data.
If a given partition has more than the supported number, the data is split into multiple files, each file representing a specific partitionValue.
By default, the data in the file is partitioned by the number of line items.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PartnerTenantId
The Microsoft Entra tenant ID of the partner.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResponseHeadersVariable
Optional Response Headers Variable.

```yaml
Type: String
Parameter Sets: (All)
Aliases: RHV

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RootDirectory
The root directory that contains all the files.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SasToken
The SAS token for accessing the directory or an individual file in the directory.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SchemaVersion
The version of the manifest schema.

```yaml
Type: String
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphPartnersBillingManifest
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphPartnersBillingManifest
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BLOBS `<IMicrosoftGraphPartnersBillingBlob- `[]`>`: A collection of blob objects that contain details of all the files for the partner tenant ID.
  - `[Name <String>]`: The blob name.
  - `[PartitionValue <String>]`: The partition that contains the file.
A large partition is split into multiple files, each with the same partitionValue.

BODYPARAMETER `<IMicrosoftGraphPartnersBillingManifest>`: manifest
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[BlobCount <Int32?>]`: The total file count for this partner tenant ID.
  - `[Blobs <IMicrosoftGraphPartnersBillingBlob- `[]`>]`: A collection of blob objects that contain details of all the files for the partner tenant ID.
    - `[Name <String>]`: The blob name.
    - `[PartitionValue <String>]`: The partition that contains the file.
A large partition is split into multiple files, each with the same partitionValue.
  - `[CreatedDateTime <DateTime?>]`: The date and time when a manifest resource was created.
The timestamp type represents date and time information using ISO 8601 format and is always in UTC.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[DataFormat <String>]`: The billing data file format.
The possible value is: compressedJSONLines.
Each blob is a compressed file and data in the file is in JSON lines format.
Decompress the file to access the data.
  - `[ETag <String>]`: Version of data represented by the manifest.
Any change in eTag indicates a new data version.
  - `[PartitionType <String>]`: Indicates the division of data.
If a given partition has more than the supported number, the data is split into multiple files, each file representing a specific partitionValue.
By default, the data in the file is partitioned by the number of line items.
  - `[PartnerTenantId <String>]`: The Microsoft Entra tenant ID of the partner.
  - `[RootDirectory <String>]`: The root directory that contains all the files.
  - `[SasToken <String>]`: The SAS token for accessing the directory or an individual file in the directory.
  - `[SchemaVersion <String>]`: The version of the manifest schema.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.reports/new-mgreportpartnerbillingmanifest](https://learn.microsoft.com/powershell/module/microsoft.graph.reports/new-mgreportpartnerbillingmanifest)
























