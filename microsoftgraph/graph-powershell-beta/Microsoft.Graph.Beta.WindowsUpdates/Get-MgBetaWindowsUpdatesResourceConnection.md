---
external help file: Microsoft.Graph.Beta.WindowsUpdates-help.xml
Module Name: Microsoft.Graph.Beta.WindowsUpdates
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.windowsupdates/get-mgbetawindowsupdatesresourceconnection
schema: 2.0.0
ms.subservice: windows-autopatch
ms.subservice: windows-autopatch
---

# Get-MgBetaWindowsUpdatesResourceConnection

## SYNOPSIS
Read the properties and relationships of a resourceConnection object.

## SYNTAX

### List (Default)
```
Get-MgBetaWindowsUpdatesResourceConnection [-ExpandProperty <String[]>] [-Property <String[]>]
 [-Filter <String>] [-Search <String>] [-Skip <Int32>] [-Sort <String[]>] [-Top <Int32>]
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PageSize <Int32>] [-All]
 [-CountVariable <String>] [<CommonParameters>]
```

### Get
```
Get-MgBetaWindowsUpdatesResourceConnection -ResourceConnectionId <String> [-ExpandProperty <String[]>]
 [-Property <String[]>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgBetaWindowsUpdatesResourceConnection -InputObject <IWindowsUpdatesIdentity> [-ExpandProperty <String[]>]
 [-Property <String[]>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

## DESCRIPTION
Read the properties and relationships of a resourceConnection object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | WindowsUpdates.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | WindowsUpdates.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.WindowsUpdates

Get-MgBetaWindowsUpdatesResourceConnection

```
This example shows how to use the Get-MgBetaWindowsUpdatesResourceConnection Cmdlet.


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
Type: IWindowsUpdatesIdentity
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

### -ResourceConnectionId
The unique identifier of resourceConnection

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

### Microsoft.Graph.Beta.PowerShell.Models.IWindowsUpdatesIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphWindowsUpdatesResourceConnection
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<IWindowsUpdatesIdentity>`: Identity Parameter
  - `[ApplicableContentCatalogEntryId <String>]`: The unique identifier of applicableContent
  - `[ApplicableContentDeviceMatchDeviceId <String>]`: The unique identifier of applicableContentDeviceMatch
  - `[CatalogEntryId <String>]`: The unique identifier of catalogEntry
  - `[CatalogId <String>]`: Usage: catalogID='{catalogID}'
  - `[ComplianceChangeId <String>]`: The unique identifier of complianceChange
  - `[DaysInPast <Int32?>]`: Usage: daysInPast={daysInPast}
  - `[DeploymentId <String>]`: The unique identifier of deployment
  - `[EditionId <String>]`: The unique identifier of edition
  - `[KbNumber <Int32?>]`: Usage: kbNumber={kbNumber}
  - `[KnownIssueId <String>]`: The unique identifier of knownIssue
  - `[ProductId <String>]`: The unique identifier of product
  - `[ProductRevisionId <String>]`: The unique identifier of productRevision
  - `[ResourceConnectionId <String>]`: The unique identifier of resourceConnection
  - `[UpdatableAssetId <String>]`: The unique identifier of updatableAsset
  - `[UpdatePolicyId <String>]`: The unique identifier of updatePolicy

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.windowsupdates/get-mgbetawindowsupdatesresourceconnection](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.windowsupdates/get-mgbetawindowsupdatesresourceconnection)

[https://learn.microsoft.com/graph/api/windowsupdates-resourceconnection-get?view=graph-rest-beta](https://learn.microsoft.com/graph/api/windowsupdates-resourceconnection-get?view=graph-rest-beta)

[https://learn.microsoft.com/graph/api/adminwindowsupdates-list-resourceconnections?view=graph-rest-beta](https://learn.microsoft.com/graph/api/adminwindowsupdates-list-resourceconnections?view=graph-rest-beta)























