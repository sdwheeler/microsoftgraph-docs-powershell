---
external help file: Microsoft.Graph.Beta.Notes-help.xml
Module Name: Microsoft.Graph.Beta.Notes
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.notes/get-mgbetauseronenotesectiongroup
schema: 2.0.0
---

# Get-MgBetaUserOnenoteSectionGroup

## SYNOPSIS
The section groups in all OneNote notebooks that the user or group owns.
Read-only.
Nullable.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Get-MgUserOnenoteSectionGroup](/powershell/module/Microsoft.Graph.Notes/Get-MgUserOnenoteSectionGroup?view=graph-powershell-1.0)

## SYNTAX

### List (Default)
```
Get-MgBetaUserOnenoteSectionGroup -UserId <String> [-ExpandProperty <String[]>] [-Property <String[]>]
 [-Filter <String>] [-Search <String>] [-Skip <Int32>] [-Sort <String[]>] [-Top <Int32>]
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PageSize <Int32>] [-All]
 [-CountVariable <String>] [<CommonParameters>]
```

### List1
```
Get-MgBetaUserOnenoteSectionGroup -SectionGroupId <String> -UserId <String> [-ExpandProperty <String[]>]
 [-Property <String[]>] [-Filter <String>] [-Search <String>] [-Skip <Int32>] [-Sort <String[]>] [-Top <Int32>]
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PageSize <Int32>] [-All]
 [-CountVariable <String>] [<CommonParameters>]
```

### Get1
```
Get-MgBetaUserOnenoteSectionGroup -SectionGroupId <String> -UserId <String> -SectionGroupId1 <String>
 [-ExpandProperty <String[]>] [-Property <String[]>] [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [<CommonParameters>]
```

### Get
```
Get-MgBetaUserOnenoteSectionGroup -SectionGroupId <String> -UserId <String> [-ExpandProperty <String[]>]
 [-Property <String[]>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

### GetViaIdentity1
```
Get-MgBetaUserOnenoteSectionGroup -InputObject <INotesIdentity> [-ExpandProperty <String[]>]
 [-Property <String[]>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgBetaUserOnenoteSectionGroup -InputObject <INotesIdentity> [-ExpandProperty <String[]>]
 [-Property <String[]>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

## DESCRIPTION
The section groups in all OneNote notebooks that the user or group owns.
Read-only.
Nullable.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Notes.Create, Notes.ReadWrite.All, Notes.ReadWrite, Notes.Read.All, Notes.Read,  |
| Delegated (personal Microsoft account) | Notes.Create, Notes.ReadWrite, Notes.Read,  |
| Application | Notes.Read.All, Notes.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Notes

# A UPN can also be used as -UserId.
Get-MgBetaUserOnenoteSectionGroup -UserId $userId

```
This example shows how to use the Get-MgBetaUserOnenoteSectionGroup Cmdlet.


## PARAMETERS

### -All
List all pages.

```yaml
Type: SwitchParameter
Parameter Sets: List, List1
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
Parameter Sets: List, List1
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
Parameter Sets: List, List1
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
Type: INotesIdentity
Parameter Sets: GetViaIdentity1, GetViaIdentity
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
Parameter Sets: List, List1
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
Parameter Sets: List, List1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SectionGroupId
The unique identifier of sectionGroup

```yaml
Type: String
Parameter Sets: List1, Get1, Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SectionGroupId1
The unique identifier of sectionGroup

```yaml
Type: String
Parameter Sets: Get1
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
Parameter Sets: List, List1
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
Parameter Sets: List, List1
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
Parameter Sets: List, List1
Aliases: Limit

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserId
The unique identifier of user

```yaml
Type: String
Parameter Sets: List, List1, Get1, Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.Beta.PowerShell.Models.INotesIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSectionGroup
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<INotesIdentity>`: Identity Parameter
  - `[GroupId <String>]`: The unique identifier of group
  - `[IncludePersonalNotebooks <Boolean?>]`: Usage: includePersonalNotebooks={includePersonalNotebooks}
  - `[NotebookId <String>]`: The unique identifier of notebook
  - `[OnenoteOperationId <String>]`: The unique identifier of onenoteOperation
  - `[OnenotePageId <String>]`: The unique identifier of onenotePage
  - `[OnenoteResourceId <String>]`: The unique identifier of onenoteResource
  - `[OnenoteSectionId <String>]`: The unique identifier of onenoteSection
  - `[Path <String>]`: Usage: path='{path}'
  - `[SectionGroupId <String>]`: The unique identifier of sectionGroup
  - `[SectionGroupId1 <String>]`: The unique identifier of sectionGroup
  - `[SiteId <String>]`: The unique identifier of site
  - `[UserId <String>]`: The unique identifier of user

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.notes/get-mgbetauseronenotesectiongroup](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.notes/get-mgbetauseronenotesectiongroup)























