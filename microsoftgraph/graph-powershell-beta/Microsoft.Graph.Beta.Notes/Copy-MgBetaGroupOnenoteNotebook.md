---
external help file: Microsoft.Graph.Beta.Notes-help.xml
Module Name: Microsoft.Graph.Beta.Notes
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.notes/copy-mgbetagrouponenotenotebook
schema: 2.0.0
ms.subservice: onenote
---

# Copy-MgBetaGroupOnenoteNotebook

## SYNOPSIS
Copies a notebook to the Notebooks folder in the destination Documents library.
The folder is created if it doesn't exist.
For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Copy-MgGroupOnenoteNotebook](/powershell/module/Microsoft.Graph.Notes/Copy-MgGroupOnenoteNotebook?view=graph-powershell-1.0)

## SYNTAX

### CopyExpanded (Default)
```
Copy-MgBetaGroupOnenoteNotebook -GroupId <String> -NotebookId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-GroupId1 <String>] [-NotebookFolder <String>] [-RenameAs <String>]
 [-SiteCollectionId <String>] [-SiteId <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CopyViaIdentityExpanded
```
Copy-MgBetaGroupOnenoteNotebook [-GroupId <String>] -InputObject <INotesIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-NotebookFolder <String>]
 [-RenameAs <String>] [-SiteCollectionId <String>] [-SiteId <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Copy
```
Copy-MgBetaGroupOnenoteNotebook -GroupId <String> -NotebookId <String>
 -BodyParameter <IPaths1Nalx8HGroupsGroupIdOnenoteNotebooksNotebookIdMicrosoftGraphCopynotebookPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CopyViaIdentity
```
Copy-MgBetaGroupOnenoteNotebook -InputObject <INotesIdentity>
 -BodyParameter <IPaths1Nalx8HGroupsGroupIdOnenoteNotebooksNotebookIdMicrosoftGraphCopynotebookPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Copies a notebook to the Notebooks folder in the destination Documents library.
The folder is created if it doesn't exist.
For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Notes.Create, Notes.ReadWrite.All, Notes.ReadWrite,  |
| Delegated (personal Microsoft account) | Notes.Create, Notes.ReadWrite,  |
| Application | Notes.ReadWrite.All,  |

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CopyExpanded, CopyViaIdentityExpanded
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
Type: IPaths1Nalx8HGroupsGroupIdOnenoteNotebooksNotebookIdMicrosoftGraphCopynotebookPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Copy, CopyViaIdentity
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

### -GroupId
The unique identifier of group

```yaml
Type: String
Parameter Sets: CopyExpanded, Copy
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: CopyViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GroupId1


```yaml
Type: String
Parameter Sets: CopyExpanded
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
Parameter Sets: CopyViaIdentityExpanded, CopyViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -NotebookFolder


```yaml
Type: String
Parameter Sets: CopyExpanded, CopyViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NotebookId
The unique identifier of notebook

```yaml
Type: String
Parameter Sets: CopyExpanded, Copy
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RenameAs


```yaml
Type: String
Parameter Sets: CopyExpanded, CopyViaIdentityExpanded
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

### -SiteCollectionId


```yaml
Type: String
Parameter Sets: CopyExpanded, CopyViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SiteId


```yaml
Type: String
Parameter Sets: CopyExpanded, CopyViaIdentityExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.INotesIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IPaths1Nalx8HGroupsGroupIdOnenoteNotebooksNotebookIdMicrosoftGraphCopynotebookPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphOnenoteOperation
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPaths1Nalx8HGroupsGroupIdOnenoteNotebooksNotebookIdMicrosoftGraphCopynotebookPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[GroupId <String>]`: 
  - `[NotebookFolder <String>]`: 
  - `[RenameAs <String>]`: 
  - `[SiteCollectionId <String>]`: 
  - `[SiteId <String>]`: 

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

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.notes/copy-mgbetagrouponenotenotebook](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.notes/copy-mgbetagrouponenotenotebook)

[https://learn.microsoft.com/graph/api/notebook-copynotebook?view=graph-rest-beta](https://learn.microsoft.com/graph/api/notebook-copynotebook?view=graph-rest-beta)
























