---
external help file: Microsoft.Graph.Beta.DeviceManagement.Enrollment-help.xml
Module Name: Microsoft.Graph.Beta.DeviceManagement.Enrollment
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.enrollment/new-mgbetarolemanagementexchangeroledefinitioninheritpermissionfrom
schema: 2.0.0
---

# New-MgBetaRoleManagementExchangeRoleDefinitionInheritPermissionFrom

## SYNOPSIS
Create new navigation property to inheritsPermissionsFrom for roleManagement

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaRoleManagementExchangeRoleDefinitionInheritPermissionFrom -UnifiedRoleDefinitionId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-AllowedPrincipalTypes <String>]
 [-Description <String>] [-DisplayName <String>] [-Id <String>]
 [-InheritsPermissionsFrom <IMicrosoftGraphUnifiedRoleDefinition[]>] [-IsBuiltIn] [-IsEnabled] [-IsPrivileged]
 [-ResourceScopes <String[]>] [-RolePermissions <IMicrosoftGraphUnifiedRolePermission[]>]
 [-TemplateId <String>] [-Version <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaRoleManagementExchangeRoleDefinitionInheritPermissionFrom -UnifiedRoleDefinitionId <String>
 -BodyParameter <IMicrosoftGraphUnifiedRoleDefinition> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgBetaRoleManagementExchangeRoleDefinitionInheritPermissionFrom
 -InputObject <IDeviceManagementEnrollmentIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-AllowedPrincipalTypes <String>] [-Description <String>]
 [-DisplayName <String>] [-Id <String>] [-InheritsPermissionsFrom <IMicrosoftGraphUnifiedRoleDefinition[]>]
 [-IsBuiltIn] [-IsEnabled] [-IsPrivileged] [-ResourceScopes <String[]>]
 [-RolePermissions <IMicrosoftGraphUnifiedRolePermission[]>] [-TemplateId <String>] [-Version <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgBetaRoleManagementExchangeRoleDefinitionInheritPermissionFrom
 -InputObject <IDeviceManagementEnrollmentIdentity> -BodyParameter <IMicrosoftGraphUnifiedRoleDefinition>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to inheritsPermissionsFrom for roleManagement

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowedPrincipalTypes
allowedRolePrincipalTypes

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
unifiedRoleDefinition
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleDefinition
Parameter Sets: Create, CreateViaIdentity
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

### -Description
The description for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
The display name for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
Required.
Supports $filter (eq and startsWith).

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InheritsPermissionsFrom
Read-only collection of role definitions that the given role definition inherits from.
Only Microsoft Entra built-in roles support this attribute.
To construct, see NOTES section for INHERITSPERMISSIONSFROM properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleDefinition[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Type: IDeviceManagementEnrollmentIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsBuiltIn
Flag indicating if the unifiedRoleDefinition is part of the default set included with the product or custom.
Read-only.
Supports $filter (eq).

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsEnabled
Flag indicating if the role is enabled for assignment.
If false the role is not available for assignment.
Read-only when isBuiltIn is true.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsPrivileged
Flag indicating if the role is privileged.
Microsoft Entra ID defines a role as privileged if it contains at least one sensitive resource action in the rolePermissions and allowedResourceActions objects.
Applies only for actions in the microsoft.directory resource namespace.
Read-only.
Supports $filter (eq).

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceScopes
List of scopes permissions granted by the role definition apply to.
Currently only / is supported.
Read-only when isBuiltIn is true.
DO NOT USE.
This will be deprecated soon.
Attach scope to role assignment.

```yaml
Type: String[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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

### -RolePermissions
List of permissions included in the role.
Read-only when isBuiltIn is true.
Required.
To construct, see NOTES section for ROLEPERMISSIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRolePermission[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TemplateId
Custom template identifier that can be set when isBuiltIn is false.
This identifier is typically used if one needs an identifier to be the same across different directories.
Read-only when isBuiltIn is true.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UnifiedRoleDefinitionId
The unique identifier of unifiedRoleDefinition

```yaml
Type: String
Parameter Sets: CreateExpanded, Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Version
Indicates the version of the unifiedRoleDefinition object.
Read-only when isBuiltIn is true.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IDeviceManagementEnrollmentIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphUnifiedRoleDefinition
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphUnifiedRoleDefinition
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphUnifiedRoleDefinition>`: unifiedRoleDefinition
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

INHERITSPERMISSIONSFROM `<IMicrosoftGraphUnifiedRoleDefinition- `[]`>`: Read-only collection of role definitions that the given role definition inherits from.
Only Microsoft Entra built-in roles support this attribute.
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

INPUTOBJECT `<IDeviceManagementEnrollmentIdentity>`: Identity Parameter
  - `[AndroidDeviceOwnerEnrollmentProfileId <String>]`: The unique identifier of androidDeviceOwnerEnrollmentProfile
  - `[AndroidForWorkEnrollmentProfileId <String>]`: The unique identifier of androidForWorkEnrollmentProfile
  - `[AppScopeId <String>]`: The unique identifier of appScope
  - `[AppleEnrollmentProfileAssignmentId <String>]`: The unique identifier of appleEnrollmentProfileAssignment
  - `[AppleUserInitiatedEnrollmentProfileId <String>]`: The unique identifier of appleUserInitiatedEnrollmentProfile
  - `[CustomAppScopeId <String>]`: The unique identifier of customAppScope
  - `[DepOnboardingSettingId <String>]`: The unique identifier of depOnboardingSetting
  - `[DeviceEnrollmentConfigurationId <String>]`: The unique identifier of deviceEnrollmentConfiguration
  - `[DeviceManagementAutopilotEventId <String>]`: The unique identifier of deviceManagementAutopilotEvent
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[EnrollmentConfigurationAssignmentId <String>]`: The unique identifier of enrollmentConfigurationAssignment
  - `[EnrollmentProfileId <String>]`: The unique identifier of enrollmentProfile
  - `[ExpiringBeforeDateTime <String>]`: Usage: expiringBeforeDateTime='{expiringBeforeDateTime}'
  - `[ImportedAppleDeviceIdentityId <String>]`: The unique identifier of importedAppleDeviceIdentity
  - `[ImportedDeviceIdentityId <String>]`: The unique identifier of importedDeviceIdentity
  - `[ImportedWindowsAutopilotDeviceIdentityId <String>]`: The unique identifier of importedWindowsAutopilotDeviceIdentity
  - `[UnifiedRbacResourceActionId <String>]`: The unique identifier of unifiedRbacResourceAction
  - `[UnifiedRbacResourceNamespaceId <String>]`: The unique identifier of unifiedRbacResourceNamespace
  - `[UnifiedRoleAssignmentId <String>]`: The unique identifier of unifiedRoleAssignment
  - `[UnifiedRoleAssignmentMultipleId <String>]`: The unique identifier of unifiedRoleAssignmentMultiple
  - `[UnifiedRoleDefinitionId <String>]`: The unique identifier of unifiedRoleDefinition
  - `[UnifiedRoleDefinitionId1 <String>]`: The unique identifier of unifiedRoleDefinition
  - `[WindowsAutopilotDeploymentProfileAssignmentId <String>]`: The unique identifier of windowsAutopilotDeploymentProfileAssignment
  - `[WindowsAutopilotDeploymentProfileId <String>]`: The unique identifier of windowsAutopilotDeploymentProfile
  - `[WindowsAutopilotDeviceIdentityId <String>]`: The unique identifier of windowsAutopilotDeviceIdentity
  - `[WindowsFeatureUpdateProfileAssignmentId <String>]`: The unique identifier of windowsFeatureUpdateProfileAssignment
  - `[WindowsFeatureUpdateProfileId <String>]`: The unique identifier of windowsFeatureUpdateProfile

ROLEPERMISSIONS `<IMicrosoftGraphUnifiedRolePermission- `[]`>`: List of permissions included in the role.
Read-only when isBuiltIn is true.
Required.
  - `[AllowedResourceActions <String- `[]`>]`: Set of tasks that can be performed on a resource.
  - `[Condition <String>]`: Optional constraints that must be met for the permission to be effective.
Not supported for custom roles.
  - `[ExcludedResourceActions <String- `[]`>]`:

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.enrollment/new-mgbetarolemanagementexchangeroledefinitioninheritpermissionfrom](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.enrollment/new-mgbetarolemanagementexchangeroledefinitioninheritpermissionfrom)
























