---
external help file: Microsoft.Graph.Beta.Devices.CloudPrint-help.xml
Module Name: Microsoft.Graph.Beta.Devices.CloudPrint
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.cloudprint/new-mgbetaprintprintertasktrigger
schema: 2.0.0
ms.subservice: universal-print
---

# New-MgBetaPrintPrinterTaskTrigger

## SYNOPSIS
Create a new task trigger on the specified printer.
Currently, only one task trigger can be specified per printer, but this limit might be removed in the future.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgPrintPrinterTaskTrigger](/powershell/module/Microsoft.Graph.Devices.CloudPrint/New-MgPrintPrinterTaskTrigger?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaPrintPrinterTaskTrigger -PrinterId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Definition <IMicrosoftGraphPrintTaskDefinition>] [-Event <String>]
 [-Id <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Create
```
New-MgBetaPrintPrinterTaskTrigger -PrinterId <String> -BodyParameter <IMicrosoftGraphPrintTaskTrigger>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgBetaPrintPrinterTaskTrigger -InputObject <IDevicesCloudPrintIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Definition <IMicrosoftGraphPrintTaskDefinition>] [-Event <String>]
 [-Id <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgBetaPrintPrinterTaskTrigger -InputObject <IDevicesCloudPrintIdentity>
 -BodyParameter <IMicrosoftGraphPrintTaskTrigger> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new task trigger on the specified printer.
Currently, only one task trigger can be specified per printer, but this limit might be removed in the future.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Printer.ReadWrite.All, Printer.FullControl.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Not supported |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Devices.CloudPrint

$params = @{
	event = "jobStarted"
	"definition@odata.bind" = "https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c"
}

New-MgBetaPrintPrinterTaskTrigger -PrinterId $printerId -BodyParameter $params

```
This example shows how to use the New-MgBetaPrintPrinterTaskTrigger Cmdlet.


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
printTaskTrigger
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphPrintTaskTrigger
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

### -Definition
printTaskDefinition
To construct, see NOTES section for DEFINITION properties and create a hash table.

```yaml
Type: IMicrosoftGraphPrintTaskDefinition
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Event
printEvent

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
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

### -PrinterId
The unique identifier of printer

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

### Microsoft.Graph.Beta.PowerShell.Models.IDevicesCloudPrintIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphPrintTaskTrigger
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphPrintTaskTrigger
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphPrintTaskTrigger>`: printTaskTrigger
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Definition <IMicrosoftGraphPrintTaskDefinition>]`: printTaskDefinition
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[CreatedBy <IMicrosoftGraphAppIdentity>]`: appIdentity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[AppId <String>]`: Refers to the unique identifier representing application ID in the Microsoft Entra ID.
      - `[DisplayName <String>]`: Refers to the application name displayed in the Microsoft Entra admin center.
      - `[ServicePrincipalId <String>]`: Refers to the unique identifier indicating service principal ID in Microsoft Entra ID for the corresponding App.
      - `[ServicePrincipalName <String>]`: Refers to the Service Principal Name is the Application name in the tenant.
    - `[DisplayName <String>]`: The name of the printTaskDefinition.
    - `[Tasks <IMicrosoftGraphPrintTask- `[]`>]`: A list of tasks that have been created based on this definition.
The list includes currently running tasks and recently completed tasks.
Read-only.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Definition <IMicrosoftGraphPrintTaskDefinition>]`: printTaskDefinition
      - `[ParentUrl <String>]`: The URL for the print entity that triggered this task.
For example, https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}.
Read-only.
      - `[Status <IMicrosoftGraphPrintTaskStatus>]`: printTaskStatus
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Description <String>]`: A human-readable description of the current processing state of the printTask.
        - `[State <String>]`: printTaskProcessingState
      - `[Trigger <IMicrosoftGraphPrintTaskTrigger>]`: printTaskTrigger
  - `[Event <String>]`: printEvent

DEFINITION `<IMicrosoftGraphPrintTaskDefinition>`: printTaskDefinition
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[CreatedBy <IMicrosoftGraphAppIdentity>]`: appIdentity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AppId <String>]`: Refers to the unique identifier representing application ID in the Microsoft Entra ID.
    - `[DisplayName <String>]`: Refers to the application name displayed in the Microsoft Entra admin center.
    - `[ServicePrincipalId <String>]`: Refers to the unique identifier indicating service principal ID in Microsoft Entra ID for the corresponding App.
    - `[ServicePrincipalName <String>]`: Refers to the Service Principal Name is the Application name in the tenant.
  - `[DisplayName <String>]`: The name of the printTaskDefinition.
  - `[Tasks <IMicrosoftGraphPrintTask- `[]`>]`: A list of tasks that have been created based on this definition.
The list includes currently running tasks and recently completed tasks.
Read-only.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Definition <IMicrosoftGraphPrintTaskDefinition>]`: printTaskDefinition
    - `[ParentUrl <String>]`: The URL for the print entity that triggered this task.
For example, https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}.
Read-only.
    - `[Status <IMicrosoftGraphPrintTaskStatus>]`: printTaskStatus
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Description <String>]`: A human-readable description of the current processing state of the printTask.
      - `[State <String>]`: printTaskProcessingState
    - `[Trigger <IMicrosoftGraphPrintTaskTrigger>]`: printTaskTrigger
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Definition <IMicrosoftGraphPrintTaskDefinition>]`: printTaskDefinition
      - `[Event <String>]`: printEvent

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

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.cloudprint/new-mgbetaprintprintertasktrigger](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.cloudprint/new-mgbetaprintprintertasktrigger)

[https://learn.microsoft.com/graph/api/printer-post-tasktriggers?view=graph-rest-beta](https://learn.microsoft.com/graph/api/printer-post-tasktriggers?view=graph-rest-beta)























