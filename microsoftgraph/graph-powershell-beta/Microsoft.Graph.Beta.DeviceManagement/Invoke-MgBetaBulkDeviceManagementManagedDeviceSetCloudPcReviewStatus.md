---
external help file: Microsoft.Graph.Beta.DeviceManagement-help.xml
Module Name: Microsoft.Graph.Beta.DeviceManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement/invoke-mgbetabulkdevicemanagementmanageddevicesetcloudpcreviewstatus
schema: 2.0.0
ms.subservice: cloud-pc
---

# Invoke-MgBetaBulkDeviceManagementManagedDeviceSetCloudPcReviewStatus

## SYNOPSIS
Invoke action bulkSetCloudPcReviewStatus

## SYNTAX

### BulkExpanded (Default)
```
Invoke-MgBetaBulkDeviceManagementManagedDeviceSetCloudPcReviewStatus [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ManagedDeviceIds <String[]>]
 [-ReviewStatus <IMicrosoftGraphCloudPcReviewStatus>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Bulk
```
Invoke-MgBetaBulkDeviceManagementManagedDeviceSetCloudPcReviewStatus
 -BodyParameter <IPaths19Pmn9HDevicemanagementManageddevicesMicrosoftGraphBulksetcloudpcreviewstatusPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Invoke action bulkSetCloudPcReviewStatus

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | CloudPC.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | CloudPC.ReadWrite.All,  |

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: BulkExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter

To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPaths19Pmn9HDevicemanagementManageddevicesMicrosoftGraphBulksetcloudpcreviewstatusPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Bulk
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

### -ManagedDeviceIds


```yaml
Type: String[]
Parameter Sets: BulkExpanded
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

### -ReviewStatus
cloudPcReviewStatus
To construct, see NOTES section for REVIEWSTATUS properties and create a hash table.

```yaml
Type: IMicrosoftGraphCloudPcReviewStatus
Parameter Sets: BulkExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IPaths19Pmn9HDevicemanagementManageddevicesMicrosoftGraphBulksetcloudpcreviewstatusPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphCloudPcBulkRemoteActionResult
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPaths19Pmn9HDevicemanagementManageddevicesMicrosoftGraphBulksetcloudpcreviewstatusPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ManagedDeviceIds <String- `[]`>]`: 
  - `[ReviewStatus <IMicrosoftGraphCloudPcReviewStatus>]`: cloudPcReviewStatus
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AccessTier <String>]`: cloudPcBlobAccessTier
    - `[AzureStorageAccountId <String>]`: The resource ID of the Azure Storage account in which the Cloud PC snapshot is being saved.
    - `[AzureStorageAccountName <String>]`: The name of the Azure Storage account in which the Cloud PC snapshot is being saved.
    - `[AzureStorageContainerName <String>]`: The name of the container in an Azure Storage account in which the Cloud PC snapshot is being saved.
    - `[InReview <Boolean?>]`: True if the Cloud PC is set to in review by the administrator.
    - `[RestorePointDateTime <DateTime?>]`: The specific date and time of the Cloud PC snapshot that was taken and saved automatically, when the Cloud PC is set to in review.
The timestamp is shown in ISO 8601 format and Coordinated Universal Time (UTC).
For example, midnight UTC on Jan 1, 2014 appears as 2014-01-01T00:00:00Z.
    - `[ReviewStartDateTime <DateTime?>]`: The specific date and time when the Cloud PC was set to in review.
The timestamp is shown in ISO 8601 format and Coordinated Universal Time (UTC).
For example, midnight UTC on Jan 1, 2014 appears as 2014-01-01T00:00:00Z.
    - `[SubscriptionId <String>]`: The ID of the Azure subscription in which the Cloud PC snapshot is being saved, in GUID format.
    - `[SubscriptionName <String>]`: The name of the Azure subscription in which the Cloud PC snapshot is being saved.
    - `[UserAccessLevel <String>]`: cloudPcUserAccessLevel

REVIEWSTATUS `<IMicrosoftGraphCloudPcReviewStatus>`: cloudPcReviewStatus
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AccessTier <String>]`: cloudPcBlobAccessTier
  - `[AzureStorageAccountId <String>]`: The resource ID of the Azure Storage account in which the Cloud PC snapshot is being saved.
  - `[AzureStorageAccountName <String>]`: The name of the Azure Storage account in which the Cloud PC snapshot is being saved.
  - `[AzureStorageContainerName <String>]`: The name of the container in an Azure Storage account in which the Cloud PC snapshot is being saved.
  - `[InReview <Boolean?>]`: True if the Cloud PC is set to in review by the administrator.
  - `[RestorePointDateTime <DateTime?>]`: The specific date and time of the Cloud PC snapshot that was taken and saved automatically, when the Cloud PC is set to in review.
The timestamp is shown in ISO 8601 format and Coordinated Universal Time (UTC).
For example, midnight UTC on Jan 1, 2014 appears as 2014-01-01T00:00:00Z.
  - `[ReviewStartDateTime <DateTime?>]`: The specific date and time when the Cloud PC was set to in review.
The timestamp is shown in ISO 8601 format and Coordinated Universal Time (UTC).
For example, midnight UTC on Jan 1, 2014 appears as 2014-01-01T00:00:00Z.
  - `[SubscriptionId <String>]`: The ID of the Azure subscription in which the Cloud PC snapshot is being saved, in GUID format.
  - `[SubscriptionName <String>]`: The name of the Azure subscription in which the Cloud PC snapshot is being saved.
  - `[UserAccessLevel <String>]`: cloudPcUserAccessLevel

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement/invoke-mgbetabulkdevicemanagementmanageddevicesetcloudpcreviewstatus](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement/invoke-mgbetabulkdevicemanagementmanageddevicesetcloudpcreviewstatus)

[https://learn.microsoft.com/graph/api/manageddevice-bulksetcloudpcreviewstatus?view=graph-rest-beta](https://learn.microsoft.com/graph/api/manageddevice-bulksetcloudpcreviewstatus?view=graph-rest-beta)
























