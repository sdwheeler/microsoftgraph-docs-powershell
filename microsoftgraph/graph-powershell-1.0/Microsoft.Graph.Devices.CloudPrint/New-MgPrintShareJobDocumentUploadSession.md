---
external help file: Microsoft.Graph.Devices.CloudPrint-help.xml
Module Name: Microsoft.Graph.Devices.CloudPrint
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.devices.cloudprint/new-mgprintsharejobdocumentuploadsession
schema: 2.0.0
ms.subservice: universal-print
---

# New-MgPrintShareJobDocumentUploadSession

## SYNOPSIS
Create an upload session that allows an app to iteratively upload ranges of a binary file linked to the print document.
As part of the response, this action returns an upload URL that can be used in subsequent sequential PUT queries.
Request headers for each PUT operation can be used to specify the exact range of bytes to be uploaded.
This allows transfer to be resumed, in case the network connection is dropped during upload.

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaPrintShareJobDocumentUploadSession](/powershell/module/Microsoft.Graph.Beta.Devices.CloudPrint/New-MgBetaPrintShareJobDocumentUploadSession?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgPrintShareJobDocumentUploadSession -PrintDocumentId <String> -PrintJobId <String>
 -PrinterShareId <String> [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Properties <IMicrosoftGraphPrintDocumentUploadProperties>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgPrintShareJobDocumentUploadSession -PrintDocumentId <String> -PrintJobId <String>
 -PrinterShareId <String>
 -BodyParameter <IPathsCv1Pi3PrintSharesPrintershareIdJobsPrintjobIdDocumentsPrintdocumentIdMicrosoftGraphCreateuploadsessionPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgPrintShareJobDocumentUploadSession -InputObject <IDevicesCloudPrintIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Properties <IMicrosoftGraphPrintDocumentUploadProperties>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgPrintShareJobDocumentUploadSession -InputObject <IDevicesCloudPrintIdentity>
 -BodyParameter <IPathsCv1Pi3PrintSharesPrintershareIdJobsPrintjobIdDocumentsPrintdocumentIdMicrosoftGraphCreateuploadsessionPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create an upload session that allows an app to iteratively upload ranges of a binary file linked to the print document.
As part of the response, this action returns an upload URL that can be used in subsequent sequential PUT queries.
Request headers for each PUT operation can be used to specify the exact range of bytes to be uploaded.
This allows transfer to be resumed, in case the network connection is dropped during upload.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | PrintJob.Create, PrintJob.ReadWrite.All, PrintJob.ReadWrite,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | PrintJob.ReadWrite.All,  |

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Type: IPathsCv1Pi3PrintSharesPrintershareIdJobsPrintjobIdDocumentsPrintdocumentIdMicrosoftGraphCreateuploadsessionPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Create, CreateViaIdentity
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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IDevicesCloudPrintIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PrintDocumentId
The unique identifier of printDocument

```yaml
Type: String
Parameter Sets: CreateExpanded, Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PrinterShareId
The unique identifier of printerShare

```yaml
Type: String
Parameter Sets: CreateExpanded, Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PrintJobId
The unique identifier of printJob

```yaml
Type: String
Parameter Sets: CreateExpanded, Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Properties
printDocumentUploadProperties
To construct, see NOTES section for PROPERTIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphPrintDocumentUploadProperties
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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

### Microsoft.Graph.PowerShell.Models.IDevicesCloudPrintIdentity
### Microsoft.Graph.PowerShell.Models.IPathsCv1Pi3PrintSharesPrintershareIdJobsPrintjobIdDocumentsPrintdocumentIdMicrosoftGraphCreateuploadsessionPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphUploadSession
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPathsCv1Pi3PrintSharesPrintershareIdJobsPrintjobIdDocumentsPrintdocumentIdMicrosoftGraphCreateuploadsessionPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Properties <IMicrosoftGraphPrintDocumentUploadProperties>]`: printDocumentUploadProperties
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ContentType <String>]`: The document's content (MIME) type.
    - `[DocumentName <String>]`: The document's name.
    - `[Size <Int64?>]`: The document's size in bytes.

INPUTOBJECT `<IDevicesCloudPrintIdentity>`: Identity Parameter
  - `[GroupId <String>]`: The unique identifier of group
  - `[PrintConnectorId <String>]`: The unique identifier of printConnector
  - `[PrintDocumentId <String>]`: The unique identifier of printDocument
  - `[PrintJobId <String>]`: The unique identifier of printJob
  - `[PrintOperationId <String>]`: The unique identifier of printOperation
  - `[PrintServiceEndpointId <String>]`: The unique identifier of printServiceEndpoint
  - `[PrintServiceId <String>]`: The unique identifier of printService
  - `[PrintTaskDefinitionId <String>]`: The unique identifier of printTaskDefinition
  - `[PrintTaskId <String>]`: The unique identifier of printTask
  - `[PrintTaskTriggerId <String>]`: The unique identifier of printTaskTrigger
  - `[PrinterId <String>]`: The unique identifier of printer
  - `[PrinterShareId <String>]`: The unique identifier of printerShare
  - `[UserId <String>]`: The unique identifier of user

PROPERTIES `<IMicrosoftGraphPrintDocumentUploadProperties>`: printDocumentUploadProperties
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ContentType <String>]`: The document's content (MIME) type.
  - `[DocumentName <String>]`: The document's name.
  - `[Size <Int64?>]`: The document's size in bytes.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.devices.cloudprint/new-mgprintsharejobdocumentuploadsession](https://learn.microsoft.com/powershell/module/microsoft.graph.devices.cloudprint/new-mgprintsharejobdocumentuploadsession)

[https://learn.microsoft.com/graph/api/printdocument-createuploadsession?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/printdocument-createuploadsession?view=graph-rest-1.0)
























