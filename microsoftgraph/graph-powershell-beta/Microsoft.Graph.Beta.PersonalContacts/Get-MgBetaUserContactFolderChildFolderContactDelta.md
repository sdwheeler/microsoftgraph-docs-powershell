---
external help file: Microsoft.Graph.Beta.PersonalContacts-help.xml
Module Name: Microsoft.Graph.Beta.PersonalContacts
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.personalcontacts/get-mgbetausercontactfolderchildfoldercontactdelta
schema: 2.0.0
ms.subservice: outlook
---

# Get-MgBetaUserContactFolderChildFolderContactDelta

## SYNOPSIS
Get a set of contacts that have been added, deleted, or updated in a specified folder.
A delta function call for contacts in a folder is similar to a GET request, except that by appropriately applying state tokens in one or more of these calls, you can query for incremental changes in the contacts in that folder.
This allows you to maintain and synchronize a local store of a user's contacts without having to fetch the entire set of contacts from the server every time.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Get-MgUserContactFolderChildFolderContactDelta](/powershell/module/Microsoft.Graph.PersonalContacts/Get-MgUserContactFolderChildFolderContactDelta?view=graph-powershell-1.0)

## SYNTAX

### Delta (Default)
```
Get-MgBetaUserContactFolderChildFolderContactDelta -ContactFolderId <String> -ContactFolderId1 <String>
 -UserId <String> [-ExpandProperty <String[]>] [-Filter <String>] [-Property <String[]>] [-Search <String>]
 [-Skip <Int32>] [-Sort <String[]>] [-Top <Int32>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-PageSize <Int32>] [-All] [-CountVariable <String>] [<CommonParameters>]
```

### DeltaViaIdentity
```
Get-MgBetaUserContactFolderChildFolderContactDelta -InputObject <IPersonalContactsIdentity>
 [-ExpandProperty <String[]>] [-Filter <String>] [-Property <String[]>] [-Search <String>] [-Skip <Int32>]
 [-Sort <String[]>] [-Top <Int32>] [-Count] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

## DESCRIPTION
Get a set of contacts that have been added, deleted, or updated in a specified folder.
A delta function call for contacts in a folder is similar to a GET request, except that by appropriately applying state tokens in one or more of these calls, you can query for incremental changes in the contacts in that folder.
This allows you to maintain and synchronize a local store of a user's contacts without having to fetch the entire set of contacts from the server every time.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Contacts.Read, Contacts.ReadWrite,  |
| Delegated (personal Microsoft account) | Contacts.Read, Contacts.ReadWrite,  |
| Application | Contacts.Read, Contacts.ReadWrite,  |

## EXAMPLES

## PARAMETERS

### -All
List all pages.

```yaml
Type: SwitchParameter
Parameter Sets: Delta
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ContactFolderId
The unique identifier of contactFolder

```yaml
Type: String
Parameter Sets: Delta
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ContactFolderId1
The unique identifier of contactFolder

```yaml
Type: String
Parameter Sets: Delta
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Count
Include count of items

```yaml
Type: SwitchParameter
Parameter Sets: DeltaViaIdentity
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
Parameter Sets: Delta
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
Parameter Sets: (All)
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
Type: IPersonalContactsIdentity
Parameter Sets: DeltaViaIdentity
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
Parameter Sets: Delta
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
Parameter Sets: (All)
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
Parameter Sets: (All)
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
Parameter Sets: (All)
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
Parameter Sets: (All)
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
Parameter Sets: Delta
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

### Microsoft.Graph.Beta.PowerShell.Models.IPersonalContactsIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphContact
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<IPersonalContactsIdentity>`: Identity Parameter
  - `[ContactFolderId <String>]`: The unique identifier of contactFolder
  - `[ContactFolderId1 <String>]`: The unique identifier of contactFolder
  - `[ContactId <String>]`: The unique identifier of contact
  - `[ExtensionId <String>]`: The unique identifier of extension
  - `[UserId <String>]`: The unique identifier of user

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.personalcontacts/get-mgbetausercontactfolderchildfoldercontactdelta](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.personalcontacts/get-mgbetausercontactfolderchildfoldercontactdelta)

[https://learn.microsoft.com/graph/api/contact-delta?view=graph-rest-beta](https://learn.microsoft.com/graph/api/contact-delta?view=graph-rest-beta)
























