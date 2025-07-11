---
external help file: Microsoft.Graph.Beta.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Beta.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/new-mgbetapolicyrolemanagementpolicyassignment
schema: 2.0.0
---

# New-MgBetaPolicyRoleManagementPolicyAssignment

## SYNOPSIS
Create new navigation property to roleManagementPolicyAssignments for policies

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgPolicyRoleManagementPolicyAssignment](/powershell/module/Microsoft.Graph.Identity.SignIns/New-MgPolicyRoleManagementPolicyAssignment?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaPolicyRoleManagementPolicyAssignment [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Id <String>] [-Policy <IMicrosoftGraphUnifiedRoleManagementPolicy>]
 [-PolicyId <String>] [-RoleDefinitionId <String>] [-ScopeId <String>] [-ScopeType <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaPolicyRoleManagementPolicyAssignment
 -BodyParameter <IMicrosoftGraphUnifiedRoleManagementPolicyAssignment> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to roleManagementPolicyAssignments for policies

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

### -BodyParameter
unifiedRoleManagementPolicyAssignment
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleManagementPolicyAssignment
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

### -Policy
unifiedRoleManagementPolicy
To construct, see NOTES section for POLICY properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleManagementPolicy
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PolicyId
The id of the policy.
Inherited from entity.

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

### -RoleDefinitionId
For Microsoft Entra roles policy, it's the identifier of the role definition object where the policy applies.
For PIM for groups membership and ownership, it's either member or owner.
Supports $filter (eq).

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

### -ScopeId
The identifier of the scope where the policy is assigned.
Can be / for the tenant or a group ID.
Required.

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

### -ScopeType
The type of the scope where the policy is assigned.
One of Directory, DirectoryRole, Group.
Required.

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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphUnifiedRoleManagementPolicyAssignment
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphUnifiedRoleManagementPolicyAssignment
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphUnifiedRoleManagementPolicyAssignment>`: unifiedRoleManagementPolicyAssignment
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Policy <IMicrosoftGraphUnifiedRoleManagementPolicy>]`: unifiedRoleManagementPolicy
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Description <String>]`: Description for the policy.
    - `[DisplayName <String>]`: Display name for the policy.
    - `[EffectiveRules <IMicrosoftGraphUnifiedRoleManagementPolicyRule- `[]`>]`: The list of effective rules like approval rules and expiration rules evaluated based on inherited referenced rules.
For example, if there is a tenant-wide policy to enforce enabling an approval rule, the effective rule will be to enable approval even if the policy has a rule to disable approval.
Supports $expand.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Target <IMicrosoftGraphUnifiedRoleManagementPolicyRuleTarget>]`: unifiedRoleManagementPolicyRuleTarget
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Caller <String>]`: The type of caller that's the target of the policy rule.
Allowed values are: None, Admin, EndUser.
        - `[EnforcedSettings <String- `[]`>]`: The list of role settings that are enforced and cannot be overridden by child scopes.
Use All for all settings.
        - `[InheritableSettings <String- `[]`>]`: The list of role settings that can be inherited by child scopes.
Use All for all settings.
        - `[Level <String>]`: The role assignment type that's the target of policy rule.
Allowed values are: Eligibility, Assignment.
        - `[Operations <String- `[]`>]`: The role management operations that are the target of the policy rule.
Allowed values are: All, Activate, Deactivate, Assign, Update, Remove, Extend, Renew.
        - `[TargetObjects <IMicrosoftGraphDirectoryObject- `[]`>]`: 
          - `[Id <String>]`: The unique identifier for an entity.
Read-only.
          - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[IsOrganizationDefault <Boolean?>]`: This can only be set to true for a single tenant-wide policy which will apply to all scopes and roles.
Set the scopeId to / and scopeType to Directory.
Supports $filter (eq, ne).
    - `[LastModifiedBy <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
      - `[Id <String>]`: The identifier of the identity.
This property is read-only.
    - `[LastModifiedDateTime <DateTime?>]`: The time when the role setting was last modified.
    - `[Rules <IMicrosoftGraphUnifiedRoleManagementPolicyRule- `[]`>]`: The collection of rules like approval rules and expiration rules.
Supports $expand.
    - `[ScopeId <String>]`: The identifier of the scope where the policy is created.
Can be / for the tenant or a group ID.
Required.
    - `[ScopeType <String>]`: The type of the scope where the policy is created.
One of Directory, DirectoryRole, Group.
Required.
  - `[PolicyId <String>]`: The id of the policy.
Inherited from entity.
  - `[RoleDefinitionId <String>]`: For Microsoft Entra roles policy, it's the identifier of the role definition object where the policy applies.
For PIM for groups membership and ownership, it's either member or owner.
Supports $filter (eq).
  - `[ScopeId <String>]`: The identifier of the scope where the policy is assigned. 
Can be / for the tenant or a group ID.
Required.
  - `[ScopeType <String>]`: The type of the scope where the policy is assigned.
One of Directory, DirectoryRole, Group.
Required.

POLICY `<IMicrosoftGraphUnifiedRoleManagementPolicy>`: unifiedRoleManagementPolicy
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Description <String>]`: Description for the policy.
  - `[DisplayName <String>]`: Display name for the policy.
  - `[EffectiveRules <IMicrosoftGraphUnifiedRoleManagementPolicyRule- `[]`>]`: The list of effective rules like approval rules and expiration rules evaluated based on inherited referenced rules.
For example, if there is a tenant-wide policy to enforce enabling an approval rule, the effective rule will be to enable approval even if the policy has a rule to disable approval.
Supports $expand.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Target <IMicrosoftGraphUnifiedRoleManagementPolicyRuleTarget>]`: unifiedRoleManagementPolicyRuleTarget
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Caller <String>]`: The type of caller that's the target of the policy rule.
Allowed values are: None, Admin, EndUser.
      - `[EnforcedSettings <String- `[]`>]`: The list of role settings that are enforced and cannot be overridden by child scopes.
Use All for all settings.
      - `[InheritableSettings <String- `[]`>]`: The list of role settings that can be inherited by child scopes.
Use All for all settings.
      - `[Level <String>]`: The role assignment type that's the target of policy rule.
Allowed values are: Eligibility, Assignment.
      - `[Operations <String- `[]`>]`: The role management operations that are the target of the policy rule.
Allowed values are: All, Activate, Deactivate, Assign, Update, Remove, Extend, Renew.
      - `[TargetObjects <IMicrosoftGraphDirectoryObject- `[]`>]`: 
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  - `[IsOrganizationDefault <Boolean?>]`: This can only be set to true for a single tenant-wide policy which will apply to all scopes and roles.
Set the scopeId to / and scopeType to Directory.
Supports $filter (eq, ne).
  - `[LastModifiedBy <IMicrosoftGraphIdentity>]`: identity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
    - `[Id <String>]`: The identifier of the identity.
This property is read-only.
  - `[LastModifiedDateTime <DateTime?>]`: The time when the role setting was last modified.
  - `[Rules <IMicrosoftGraphUnifiedRoleManagementPolicyRule- `[]`>]`: The collection of rules like approval rules and expiration rules.
Supports $expand.
  - `[ScopeId <String>]`: The identifier of the scope where the policy is created.
Can be / for the tenant or a group ID.
Required.
  - `[ScopeType <String>]`: The type of the scope where the policy is created.
One of Directory, DirectoryRole, Group.
Required.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/new-mgbetapolicyrolemanagementpolicyassignment](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/new-mgbetapolicyrolemanagementpolicyassignment)
























