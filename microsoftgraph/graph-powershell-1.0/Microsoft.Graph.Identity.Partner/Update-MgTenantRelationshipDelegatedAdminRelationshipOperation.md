---
external help file: Microsoft.Graph.Identity.Partner-help.xml
Module Name: Microsoft.Graph.Identity.Partner
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.partner/update-mgtenantrelationshipdelegatedadminrelationshipoperation
schema: 2.0.0
---

# Update-MgTenantRelationshipDelegatedAdminRelationshipOperation

## SYNOPSIS
Update the navigation property operations in tenantRelationships

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaTenantRelationshipDelegatedAdminRelationshipOperation](/powershell/module/Microsoft.Graph.Beta.Identity.Partner/Update-MgBetaTenantRelationshipDelegatedAdminRelationshipOperation?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgTenantRelationshipDelegatedAdminRelationshipOperation -DelegatedAdminRelationshipId <String>
 -DelegatedAdminRelationshipOperationId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-CreatedDateTime <DateTime>] [-Data <String>] [-Id <String>]
 [-LastModifiedDateTime <DateTime>] [-OperationType <String>] [-Status <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgTenantRelationshipDelegatedAdminRelationshipOperation -DelegatedAdminRelationshipId <String>
 -DelegatedAdminRelationshipOperationId <String>
 -BodyParameter <IMicrosoftGraphDelegatedAdminRelationshipOperation> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgTenantRelationshipDelegatedAdminRelationshipOperation -InputObject <IIdentityPartnerIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-CreatedDateTime <DateTime>]
 [-Data <String>] [-Id <String>] [-LastModifiedDateTime <DateTime>] [-OperationType <String>]
 [-Status <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgTenantRelationshipDelegatedAdminRelationshipOperation -InputObject <IIdentityPartnerIdentity>
 -BodyParameter <IMicrosoftGraphDelegatedAdminRelationshipOperation> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property operations in tenantRelationships

## EXAMPLES

## PARAMETERS

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
delegatedAdminRelationshipOperation
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphDelegatedAdminRelationshipOperation
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
The time in ISO 8601 format and in UTC time when the long-running operation was created.
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

### -Data
The data (payload) for the operation.
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

### -DelegatedAdminRelationshipOperationId
The unique identifier of delegatedAdminRelationshipOperation

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
The time in ISO 8601 format and in UTC time when the long-running operation was last modified.
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

### -OperationType
delegatedAdminRelationshipOperationType

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
longRunningOperationStatus

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

### Microsoft.Graph.PowerShell.Models.IIdentityPartnerIdentity
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphDelegatedAdminRelationshipOperation
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphDelegatedAdminRelationshipOperation
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphDelegatedAdminRelationshipOperation>`: delegatedAdminRelationshipOperation
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[CreatedDateTime <DateTime?>]`: The time in ISO 8601 format and in UTC time when the long-running operation was created.
Read-only.
  - `[Data <String>]`: The data (payload) for the operation.
Read-only.
  - `[LastModifiedDateTime <DateTime?>]`: The time in ISO 8601 format and in UTC time when the long-running operation was last modified.
Read-only.
  - `[OperationType <String>]`: delegatedAdminRelationshipOperationType
  - `[Status <String>]`: longRunningOperationStatus

INPUTOBJECT `<IIdentityPartnerIdentity>`: Identity Parameter
  - `[DelegatedAdminAccessAssignmentId <String>]`: The unique identifier of delegatedAdminAccessAssignment
  - `[DelegatedAdminCustomerId <String>]`: The unique identifier of delegatedAdminCustomer
  - `[DelegatedAdminRelationshipId <String>]`: The unique identifier of delegatedAdminRelationship
  - `[DelegatedAdminRelationshipOperationId <String>]`: The unique identifier of delegatedAdminRelationshipOperation
  - `[DelegatedAdminRelationshipRequestId <String>]`: The unique identifier of delegatedAdminRelationshipRequest
  - `[DelegatedAdminServiceManagementDetailId <String>]`: The unique identifier of delegatedAdminServiceManagementDetail

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.partner/update-mgtenantrelationshipdelegatedadminrelationshipoperation](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.partner/update-mgtenantrelationshipdelegatedadminrelationshipoperation)
























