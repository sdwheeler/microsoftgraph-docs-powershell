---
external help file: Microsoft.Graph.Beta.Security-help.xml
Module Name: Microsoft.Graph.Beta.Security
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/new-mgbetasecuritylabelcategory
schema: 2.0.0
ms.subservice: security
---

# New-MgBetaSecurityLabelCategory

## SYNOPSIS
Create a new categoryTemplate object.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgSecurityLabelCategory](/powershell/module/Microsoft.Graph.Security/New-MgSecurityLabelCategory?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaSecurityLabelCategory [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-CreatedBy <IMicrosoftGraphIdentitySet>] [-CreatedDateTime <DateTime>] [-DisplayName <String>] [-Id <String>]
 [-Subcategories <IMicrosoftGraphSecuritySubcategoryTemplate[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaSecurityLabelCategory -BodyParameter <IMicrosoftGraphSecurityCategoryTemplate>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new categoryTemplate object.

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	"@odata.type" = "#microsoft.graph.security.categoryTemplate"
	displayName = "Accounts Payable"
}

New-MgBetaSecurityLabelCategory -BodyParameter $params

```
This example shows how to use the New-MgBetaSecurityLabelCategory Cmdlet.


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

### -BodyParameter
categoryTemplate
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityCategoryTemplate
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

### -CreatedBy
identitySet
To construct, see NOTES section for CREATEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentitySet
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreatedDateTime
Represents the date and time in which the filePlanDescriptorTemplate is created.
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

### -DisplayName
Unique string that defines a filePlanDescriptorTemplate name.

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

### -Subcategories
Represents all subcategories under a particular category.
To construct, see NOTES section for SUBCATEGORIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecuritySubcategoryTemplate[]
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSecurityCategoryTemplate
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSecurityCategoryTemplate
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphSecurityCategoryTemplate>`: categoryTemplate
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
      - `[Id <String>]`: The identifier of the identity.
This property is read-only.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
Read-only.
  - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Subcategories <IMicrosoftGraphSecuritySubcategoryTemplate- `[]`>]`: Represents all subcategories under a particular category.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
Read-only.
    - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.

CREATEDBY `<IMicrosoftGraphIdentitySet>`: identitySet
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Application <IMicrosoftGraphIdentity>]`: identity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
    - `[Id <String>]`: The identifier of the identity.
This property is read-only.
  - `[Device <IMicrosoftGraphIdentity>]`: identity
  - `[User <IMicrosoftGraphIdentity>]`: identity

SUBCATEGORIES `<IMicrosoftGraphSecuritySubcategoryTemplate- `[]`>`: Represents all subcategories under a particular category.
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
      - `[Id <String>]`: The identifier of the identity.
This property is read-only.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[CreatedDateTime <DateTime?>]`: Represents the date and time in which the filePlanDescriptorTemplate is created.
Read-only.
  - `[DisplayName <String>]`: Unique string that defines a filePlanDescriptorTemplate name.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/new-mgbetasecuritylabelcategory](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/new-mgbetasecuritylabelcategory)

[https://learn.microsoft.com/graph/api/security-labelsroot-post-categories?view=graph-rest-beta](https://learn.microsoft.com/graph/api/security-labelsroot-post-categories?view=graph-rest-beta)























