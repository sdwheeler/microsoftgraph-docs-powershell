---
external help file: Microsoft.Graph.Beta.Identity.Partner-help.xml
Module Name: Microsoft.Graph.Beta.Identity.Partner
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.partner/update-mgbetatenantrelationshipdelegatedadminrelationshipaccessassignment
schema: 2.0.0
ms.subservice: partner-customer-administration
---

# Update-MgBetaTenantRelationshipDelegatedAdminRelationshipAccessAssignment

## SYNOPSIS
Update the properties of a delegatedAdminAccessAssignment object.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgTenantRelationshipDelegatedAdminRelationshipAccessAssignment](/powershell/module/Microsoft.Graph.Identity.Partner/Update-MgTenantRelationshipDelegatedAdminRelationshipAccessAssignment?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaTenantRelationshipDelegatedAdminRelationshipAccessAssignment
 -DelegatedAdminAccessAssignmentId <String> -DelegatedAdminRelationshipId <String>
 [-ResponseHeadersVariable <String>] [-AccessContainer <IMicrosoftGraphDelegatedAdminAccessContainer>]
 [-AccessDetails <IMicrosoftGraphDelegatedAdminAccessDetails>] [-AdditionalProperties <Hashtable>]
 [-CreatedDateTime <DateTime>] [-Id <String>] [-LastModifiedDateTime <DateTime>] [-Status <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaTenantRelationshipDelegatedAdminRelationshipAccessAssignment
 -DelegatedAdminAccessAssignmentId <String> -DelegatedAdminRelationshipId <String>
 -BodyParameter <IMicrosoftGraphDelegatedAdminAccessAssignment> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaTenantRelationshipDelegatedAdminRelationshipAccessAssignment
 -InputObject <IIdentityPartnerIdentity> [-ResponseHeadersVariable <String>]
 [-AccessContainer <IMicrosoftGraphDelegatedAdminAccessContainer>]
 [-AccessDetails <IMicrosoftGraphDelegatedAdminAccessDetails>] [-AdditionalProperties <Hashtable>]
 [-CreatedDateTime <DateTime>] [-Id <String>] [-LastModifiedDateTime <DateTime>] [-Status <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaTenantRelationshipDelegatedAdminRelationshipAccessAssignment
 -InputObject <IIdentityPartnerIdentity> -BodyParameter <IMicrosoftGraphDelegatedAdminAccessAssignment>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the properties of a delegatedAdminAccessAssignment object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | DelegatedAdminRelationship.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | DelegatedAdminRelationship.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Identity.Partner

$params = @{
	accessDetails = @{
		unifiedRoles = @(
			@{
				roleDefinitionId = "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
			}
			@{
				roleDefinitionId = "44367163-eba1-44c3-98af-f5787879f96a"
			}
			@{
				roleDefinitionId = "729827e3-9c14-49f7-bb1b-9608f156bbb8"
			}
		)
	}
}

Update-MgBetaTenantRelationshipDelegatedAdminRelationshipAccessAssignment -DelegatedAdminRelationshipId $delegatedAdminRelationshipId -DelegatedAdminAccessAssignmentId $delegatedAdminAccessAssignmentId -BodyParameter $params

```
This example shows how to use the Update-MgBetaTenantRelationshipDelegatedAdminRelationshipAccessAssignment Cmdlet.


## PARAMETERS

### -AccessContainer
delegatedAdminAccessContainer
To construct, see NOTES section for ACCESSCONTAINER properties and create a hash table.

```yaml
Type: IMicrosoftGraphDelegatedAdminAccessContainer
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AccessDetails
delegatedAdminAccessDetails
To construct, see NOTES section for ACCESSDETAILS properties and create a hash table.

```yaml
Type: IMicrosoftGraphDelegatedAdminAccessDetails
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
delegatedAdminAccessAssignment
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphDelegatedAdminAccessAssignment
Parameter Sets: Update, UpdateViaIdentity
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

### -CreatedDateTime
The date and time in ISO 8601 format and in UTC time when the access assignment was created.
Read-only.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DelegatedAdminAccessAssignmentId
The unique identifier of delegatedAdminAccessAssignment

```yaml
Type: String
Parameter Sets: UpdateExpanded, Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DelegatedAdminRelationshipId
The unique identifier of delegatedAdminRelationship

```yaml
Type: String
Parameter Sets: UpdateExpanded, Update
Aliases:

Required: True
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Type: IIdentityPartnerIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -LastModifiedDateTime
The date and time in ISO 8601 and in UTC time when this access assignment was last modified.
Read-only.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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

### -Status
delegatedAdminAccessAssignmentStatus

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IIdentityPartnerIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphDelegatedAdminAccessAssignment
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphDelegatedAdminAccessAssignment
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ACCESSCONTAINER `<IMicrosoftGraphDelegatedAdminAccessContainer>`: delegatedAdminAccessContainer
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AccessContainerId <String>]`: The identifier of the access container (for example, a security group).
For 'securityGroup' access containers, this must be a valid ID of a Microsoft Entra security group in the Microsoft partner's tenant.
  - `[AccessContainerType <String>]`: delegatedAdminAccessContainerType

ACCESSDETAILS `<IMicrosoftGraphDelegatedAdminAccessDetails>`: delegatedAdminAccessDetails
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[UnifiedRoles <IMicrosoftGraphUnifiedRole- `[]`>]`: The directory roles that the Microsoft partner is assigned in the customer tenant.
    - `[RoleDefinitionId <String>]`: The unified role definition ID of the directory role.
Refer to unifiedRoleDefinition resource.

BODYPARAMETER `<IMicrosoftGraphDelegatedAdminAccessAssignment>`: delegatedAdminAccessAssignment
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AccessContainer <IMicrosoftGraphDelegatedAdminAccessContainer>]`: delegatedAdminAccessContainer
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AccessContainerId <String>]`: The identifier of the access container (for example, a security group).
For 'securityGroup' access containers, this must be a valid ID of a Microsoft Entra security group in the Microsoft partner's tenant.
    - `[AccessContainerType <String>]`: delegatedAdminAccessContainerType
  - `[AccessDetails <IMicrosoftGraphDelegatedAdminAccessDetails>]`: delegatedAdminAccessDetails
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[UnifiedRoles <IMicrosoftGraphUnifiedRole- `[]`>]`: The directory roles that the Microsoft partner is assigned in the customer tenant.
      - `[RoleDefinitionId <String>]`: The unified role definition ID of the directory role.
Refer to unifiedRoleDefinition resource.
  - `[CreatedDateTime <DateTime?>]`: The date and time in ISO 8601 format and in UTC time when the access assignment was created.
Read-only.
  - `[LastModifiedDateTime <DateTime?>]`: The date and time in ISO 8601 and in UTC time when this access assignment was last modified.
Read-only.
  - `[Status <String>]`: delegatedAdminAccessAssignmentStatus

INPUTOBJECT `<IIdentityPartnerIdentity>`: Identity Parameter
  - `[DelegatedAdminAccessAssignmentId <String>]`: The unique identifier of delegatedAdminAccessAssignment
  - `[DelegatedAdminCustomerId <String>]`: The unique identifier of delegatedAdminCustomer
  - `[DelegatedAdminRelationshipId <String>]`: The unique identifier of delegatedAdminRelationship
  - `[DelegatedAdminRelationshipOperationId <String>]`: The unique identifier of delegatedAdminRelationshipOperation
  - `[DelegatedAdminRelationshipRequestId <String>]`: The unique identifier of delegatedAdminRelationshipRequest
  - `[DelegatedAdminServiceManagementDetailId <String>]`: The unique identifier of delegatedAdminServiceManagementDetail

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.partner/update-mgbetatenantrelationshipdelegatedadminrelationshipaccessassignment](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.partner/update-mgbetatenantrelationshipdelegatedadminrelationshipaccessassignment)

[https://learn.microsoft.com/graph/api/delegatedadminaccessassignment-update?view=graph-rest-beta](https://learn.microsoft.com/graph/api/delegatedadminaccessassignment-update?view=graph-rest-beta)























