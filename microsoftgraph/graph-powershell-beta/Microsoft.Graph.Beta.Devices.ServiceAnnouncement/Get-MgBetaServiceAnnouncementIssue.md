---
external help file: Microsoft.Graph.Beta.Devices.ServiceAnnouncement-help.xml
Module Name: Microsoft.Graph.Beta.Devices.ServiceAnnouncement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.serviceannouncement/get-mgbetaserviceannouncementissue
schema: 2.0.0
ms.subservice: service-communications
ms.subservice: service-communications
---

# Get-MgBetaServiceAnnouncementIssue

## SYNOPSIS
Retrieve the properties and relationships of a serviceHealthIssue object.
This operation retrieves a specified service health issue for tenant.
The operation returns an error if the issue does not exist for the tenant.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Get-MgServiceAnnouncementIssue](/powershell/module/Microsoft.Graph.Devices.ServiceAnnouncement/Get-MgServiceAnnouncementIssue?view=graph-powershell-1.0)

## SYNTAX

### List (Default)
```
Get-MgBetaServiceAnnouncementIssue [-ExpandProperty <String[]>] [-Property <String[]>] [-Filter <String>]
 [-Search <String>] [-Skip <Int32>] [-Sort <String[]>] [-Top <Int32>] [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-PageSize <Int32>] [-All] [-CountVariable <String>]
 [<CommonParameters>]
```

### Get
```
Get-MgBetaServiceAnnouncementIssue -ServiceHealthIssueId <String> [-ExpandProperty <String[]>]
 [-Property <String[]>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgBetaServiceAnnouncementIssue -InputObject <IDevicesServiceAnnouncementIdentity>
 [-ExpandProperty <String[]>] [-Property <String[]>] [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [<CommonParameters>]
```

## DESCRIPTION
Retrieve the properties and relationships of a serviceHealthIssue object.
This operation retrieves a specified service health issue for tenant.
The operation returns an error if the issue does not exist for the tenant.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | ServiceHealth.Read.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | ServiceHealth.Read.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Devices.ServiceAnnouncement

Get-MgBetaServiceAnnouncementIssue

```
This example shows how to use the Get-MgBetaServiceAnnouncementIssue Cmdlet.


## PARAMETERS

### -All
List all pages.

```yaml
Type: SwitchParameter
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -CountVariable
Specifies a count of the total number of items in a collection.
By default, this variable will be set in the global scope.

```yaml
Type: String
Parameter Sets: List
Aliases: CV

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExpandProperty
Expand related entities

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Expand

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Filter
Filter items by property values

```yaml
Type: String
Parameter Sets: List
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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IDevicesServiceAnnouncementIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PageSize
Sets the page size of results.

```yaml
Type: Int32
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Property
Select properties to be returned

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Select

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

### -Search
Search items by search phrases

```yaml
Type: String
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServiceHealthIssueId
The unique identifier of serviceHealthIssue

```yaml
Type: String
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Skip
Skip the first n items

```yaml
Type: Int32
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Sort
Order items by property values

```yaml
Type: String[]
Parameter Sets: List
Aliases: OrderBy

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Top
Show only the first n items

```yaml
Type: Int32
Parameter Sets: List
Aliases: Limit

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IDevicesServiceAnnouncementIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphServiceHealthIssue
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<IDevicesServiceAnnouncementIdentity>`: Identity Parameter
  - `[ServiceAnnouncementAttachmentId <String>]`: The unique identifier of serviceAnnouncementAttachment
  - `[ServiceHealthId <String>]`: The unique identifier of serviceHealth
  - `[ServiceHealthIssueId <String>]`: The unique identifier of serviceHealthIssue
  - `[ServiceUpdateMessageId <String>]`: The unique identifier of serviceUpdateMessage

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.serviceannouncement/get-mgbetaserviceannouncementissue](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.serviceannouncement/get-mgbetaserviceannouncementissue)

[https://learn.microsoft.com/graph/api/servicehealthissue-get?view=graph-rest-beta](https://learn.microsoft.com/graph/api/servicehealthissue-get?view=graph-rest-beta)

[https://learn.microsoft.com/graph/api/serviceannouncement-list-issues?view=graph-rest-beta](https://learn.microsoft.com/graph/api/serviceannouncement-list-issues?view=graph-rest-beta)























