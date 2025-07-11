---
external help file: Microsoft.Graph.Beta.Identity.DirectoryManagement-help.xml
Module Name: Microsoft.Graph.Beta.Identity.DirectoryManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/new-mgbetadirectoryexternaluserprofile
schema: 2.0.0
---

# New-MgBetaDirectoryExternalUserProfile

## SYNOPSIS
Create new navigation property to externalUserProfiles for directory

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaDirectoryExternalUserProfile [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Address <IMicrosoftGraphPhysicalOfficeAddress>] [-CompanyName <String>] [-CreatedBy <String>]
 [-CreatedDateTime <DateTime>] [-DeletedDateTime <DateTime>] [-Department <String>] [-DisplayName <String>]
 [-Id <String>] [-IsDiscoverable] [-IsEnabled] [-JobTitle <String>] [-PhoneNumber <String>]
 [-SupervisorId <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Create
```
New-MgBetaDirectoryExternalUserProfile -BodyParameter <Hashtable> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to externalUserProfiles for directory

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | ExternalUserProfile.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | ExternalUserProfile.ReadWrite.All,  |

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

### -Address
physicalOfficeAddress
To construct, see NOTES section for ADDRESS properties and create a hash table.

```yaml
Type: IMicrosoftGraphPhysicalOfficeAddress
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
externalUserProfile

```yaml
Type: Hashtable
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CompanyName
The company name of the external user profile.
Supports $filter (eq, startswith).

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

### -CreatedBy
The object ID of the user who created the external user profile.
Read-only.
Not nullable.

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

### -CreatedDateTime
Date and time when this external user was created.
Not nullable.
Read-only.

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

### -DeletedDateTime
Date and time when this object was deleted.
Always null when the object hasn't been deleted.

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

### -Department
The department of the external user profile.

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

### -DisplayName
The display name of the external user profile.

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

### -IsDiscoverable
Represents whether the external user profile is discoverable in the directory.
When true, this external profile shows up in Teams search.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsEnabled
Represents whether the external user profile is enabled in the directory.
This property is peer to the accountEnabled property on the user object.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -JobTitle
The job title of the external user profile.

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

### -PhoneNumber
The phone number of the external user profile.
Must be in E164 format.

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

### -SupervisorId
The object ID of the supervisor of the external user profile.
Supports $filter (eq, startswith).

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

### System.Collections.Hashtable
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphExternalUserProfile
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ADDRESS `<IMicrosoftGraphPhysicalOfficeAddress>`: physicalOfficeAddress
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[City <String>]`: The city.
  - `[CountryOrRegion <String>]`: The country or region.
It's a free-format string value, for example, 'United States'.
  - `[OfficeLocation <String>]`: Office location such as building and office number for an organizational contact.
  - `[PostalCode <String>]`: The postal code.
  - `[State <String>]`: The state.
  - `[Street <String>]`: The street.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/new-mgbetadirectoryexternaluserprofile](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/new-mgbetadirectoryexternaluserprofile)
























