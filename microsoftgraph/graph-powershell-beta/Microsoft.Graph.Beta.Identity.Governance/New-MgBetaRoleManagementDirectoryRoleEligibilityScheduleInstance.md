---
external help file: Microsoft.Graph.Beta.Identity.Governance-help.xml
Module Name: Microsoft.Graph.Beta.Identity.Governance
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/new-mgbetarolemanagementdirectoryroleeligibilityscheduleinstance
schema: 2.0.0
---

# New-MgBetaRoleManagementDirectoryRoleEligibilityScheduleInstance

## SYNOPSIS
Create new navigation property to roleEligibilityScheduleInstances for roleManagement

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgRoleManagementDirectoryRoleEligibilityScheduleInstance](/powershell/module/Microsoft.Graph.Identity.Governance/New-MgRoleManagementDirectoryRoleEligibilityScheduleInstance?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaRoleManagementDirectoryRoleEligibilityScheduleInstance [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-AppScope <IMicrosoftGraphAppScope>] [-AppScopeId <String>]
 [-DirectoryScope <IMicrosoftGraphDirectoryObject>] [-DirectoryScopeId <String>] [-EndDateTime <DateTime>]
 [-Id <String>] [-MemberType <String>] [-Principal <IMicrosoftGraphDirectoryObject>] [-PrincipalId <String>]
 [-RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>] [-RoleDefinitionId <String>]
 [-RoleEligibilityScheduleId <String>] [-StartDateTime <DateTime>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaRoleManagementDirectoryRoleEligibilityScheduleInstance
 -BodyParameter <IMicrosoftGraphUnifiedRoleEligibilityScheduleInstance> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to roleEligibilityScheduleInstances for roleManagement

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

### -AppScope
appScope
To construct, see NOTES section for APPSCOPE properties and create a hash table.

```yaml
Type: IMicrosoftGraphAppScope
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppScopeId
Identifier of the app-specific scope when the assignment or role eligibility is scoped to an app.
The scope of an assignment or role eligibility determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.

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

### -BodyParameter
unifiedRoleEligibilityScheduleInstance
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleEligibilityScheduleInstance
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

### -DirectoryScope
directoryObject
To construct, see NOTES section for DIRECTORYSCOPE properties and create a hash table.

```yaml
Type: IMicrosoftGraphDirectoryObject
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DirectoryScopeId
Identifier of the directory object representing the scope of the assignment or role eligibility.
The scope of an assignment or role eligibility determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.

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

### -EndDateTime
Time that the roleEligibilityScheduleInstance will expire.

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

### -MemberType
Membership type of the assignment.
It can either be Inherited, Direct, or Group.

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

### -Principal
directoryObject
To construct, see NOTES section for PRINCIPAL properties and create a hash table.

```yaml
Type: IMicrosoftGraphDirectoryObject
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PrincipalId
Identifier of the principal that has been granted the role assignment or that's eligible for a role.

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

### -RoleDefinition
unifiedRoleDefinition
To construct, see NOTES section for ROLEDEFINITION properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleDefinition
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RoleDefinitionId
Identifier of the unifiedRoleDefinition object that is being assigned to the principal or that the principal is eligible for.

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

### -RoleEligibilityScheduleId
Identifier of the parent roleEligibilitySchedule for this instance.

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

### -StartDateTime
Time that the roleEligibilityScheduleInstance will start.

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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphUnifiedRoleEligibilityScheduleInstance
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphUnifiedRoleEligibilityScheduleInstance
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

APPSCOPE `<IMicrosoftGraphAppScope>`: appScope
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DisplayName <String>]`: Provides the display name of the app-specific resource represented by the app scope.
Provided for display purposes since appScopeId is often an immutable, non-human-readable ID.
Read only.
  - `[Type <String>]`: Describes the type of app-specific resource represented by the app scope.
For display purposes, so a user interface can convey to the user the kind of app specific resource represented by the app scope.
Read only.

BODYPARAMETER `<IMicrosoftGraphUnifiedRoleEligibilityScheduleInstance>`: unifiedRoleEligibilityScheduleInstance
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: Provides the display name of the app-specific resource represented by the app scope.
Provided for display purposes since appScopeId is often an immutable, non-human-readable ID.
Read only.
    - `[Type <String>]`: Describes the type of app-specific resource represented by the app scope.
For display purposes, so a user interface can convey to the user the kind of app specific resource represented by the app scope.
Read only.
  - `[AppScopeId <String>]`: Identifier of the app-specific scope when the assignment or role eligibility is scoped to an app.
The scope of an assignment or role eligibility determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
  - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment or role eligibility.
The scope of an assignment or role eligibility determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
  - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
  - `[PrincipalId <String>]`: Identifier of the principal that has been granted the role assignment or that's eligible for a role.
  - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AllowedPrincipalTypes <String>]`: allowedRolePrincipalTypes
    - `[Description <String>]`: The description for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
    - `[DisplayName <String>]`: The display name for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
Required. 
Supports $filter (eq and startsWith).
    - `[InheritsPermissionsFrom <IMicrosoftGraphUnifiedRoleDefinition- `[]`>]`: Read-only collection of role definitions that the given role definition inherits from.
Only Microsoft Entra built-in roles support this attribute.
    - `[IsBuiltIn <Boolean?>]`: Flag indicating if the unifiedRoleDefinition is part of the default set included with the product or custom.
Read-only. 
Supports $filter (eq).
    - `[IsEnabled <Boolean?>]`: Flag indicating if the role is enabled for assignment.
If false the role is not available for assignment.
Read-only when isBuiltIn is true.
    - `[IsPrivileged <Boolean?>]`: Flag indicating if the role is privileged.
Microsoft Entra ID defines a role as privileged if it contains at least one sensitive resource action in the rolePermissions and allowedResourceActions objects.
Applies only for actions in the microsoft.directory resource namespace.
Read-only.
Supports $filter (eq).
    - `[ResourceScopes <String- `[]`>]`: List of scopes permissions granted by the role definition apply to.
Currently only / is supported.
Read-only when isBuiltIn is true.
DO NOT USE.
This will be deprecated soon.
Attach scope to role assignment.
    - `[RolePermissions <IMicrosoftGraphUnifiedRolePermission- `[]`>]`: List of permissions included in the role.
Read-only when isBuiltIn is true.
Required.
      - `[AllowedResourceActions <String- `[]`>]`: Set of tasks that can be performed on a resource.
      - `[Condition <String>]`: Optional constraints that must be met for the permission to be effective.
Not supported for custom roles.
      - `[ExcludedResourceActions <String- `[]`>]`: 
    - `[TemplateId <String>]`: Custom template identifier that can be set when isBuiltIn is false.
This identifier is typically used if one needs an identifier to be the same across different directories.
Read-only when isBuiltIn is true.
    - `[Version <String>]`: Indicates the version of the unifiedRoleDefinition object.
Read-only when isBuiltIn is true.
  - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal or that the principal is eligible for.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[EndDateTime <DateTime?>]`: Time that the roleEligibilityScheduleInstance will expire.
  - `[MemberType <String>]`: Membership type of the assignment.
It can either be Inherited, Direct, or Group.
  - `[RoleEligibilityScheduleId <String>]`: Identifier of the parent roleEligibilitySchedule for this instance.
  - `[StartDateTime <DateTime?>]`: Time that the roleEligibilityScheduleInstance will start.

DIRECTORYSCOPE `<IMicrosoftGraphDirectoryObject>`: directoryObject
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.

PRINCIPAL `<IMicrosoftGraphDirectoryObject>`: directoryObject
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.

ROLEDEFINITION `<IMicrosoftGraphUnifiedRoleDefinition>`: unifiedRoleDefinition
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AllowedPrincipalTypes <String>]`: allowedRolePrincipalTypes
  - `[Description <String>]`: The description for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
  - `[DisplayName <String>]`: The display name for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
Required. 
Supports $filter (eq and startsWith).
  - `[InheritsPermissionsFrom <IMicrosoftGraphUnifiedRoleDefinition- `[]`>]`: Read-only collection of role definitions that the given role definition inherits from.
Only Microsoft Entra built-in roles support this attribute.
  - `[IsBuiltIn <Boolean?>]`: Flag indicating if the unifiedRoleDefinition is part of the default set included with the product or custom.
Read-only. 
Supports $filter (eq).
  - `[IsEnabled <Boolean?>]`: Flag indicating if the role is enabled for assignment.
If false the role is not available for assignment.
Read-only when isBuiltIn is true.
  - `[IsPrivileged <Boolean?>]`: Flag indicating if the role is privileged.
Microsoft Entra ID defines a role as privileged if it contains at least one sensitive resource action in the rolePermissions and allowedResourceActions objects.
Applies only for actions in the microsoft.directory resource namespace.
Read-only.
Supports $filter (eq).
  - `[ResourceScopes <String- `[]`>]`: List of scopes permissions granted by the role definition apply to.
Currently only / is supported.
Read-only when isBuiltIn is true.
DO NOT USE.
This will be deprecated soon.
Attach scope to role assignment.
  - `[RolePermissions <IMicrosoftGraphUnifiedRolePermission- `[]`>]`: List of permissions included in the role.
Read-only when isBuiltIn is true.
Required.
    - `[AllowedResourceActions <String- `[]`>]`: Set of tasks that can be performed on a resource.
    - `[Condition <String>]`: Optional constraints that must be met for the permission to be effective.
Not supported for custom roles.
    - `[ExcludedResourceActions <String- `[]`>]`: 
  - `[TemplateId <String>]`: Custom template identifier that can be set when isBuiltIn is false.
This identifier is typically used if one needs an identifier to be the same across different directories.
Read-only when isBuiltIn is true.
  - `[Version <String>]`: Indicates the version of the unifiedRoleDefinition object.
Read-only when isBuiltIn is true.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/new-mgbetarolemanagementdirectoryroleeligibilityscheduleinstance](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/new-mgbetarolemanagementdirectoryroleeligibilityscheduleinstance)
























