---
external help file: Microsoft.Graph.Beta.DeviceManagement.Enrollment-help.xml
Module Name: Microsoft.Graph.Beta.DeviceManagement.Enrollment
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.enrollment/set-mgbetadevicemanagementwindowsautopilotdeviceidentityresourceaccounttodevice
schema: 2.0.0
---

# Set-MgBetaDeviceManagementWindowsAutopilotDeviceIdentityResourceAccountToDevice

## SYNOPSIS
Assigns resource account to Autopilot devices.

## SYNTAX

### AssignExpanded (Default)
```
Set-MgBetaDeviceManagementWindowsAutopilotDeviceIdentityResourceAccountToDevice
 -WindowsAutopilotDeviceIdentityId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-AddressableUserName <String>] [-ResourceAccountName <String>]
 [-UserPrincipalName <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Assign
```
Set-MgBetaDeviceManagementWindowsAutopilotDeviceIdentityResourceAccountToDevice
 -WindowsAutopilotDeviceIdentityId <String>
 -BodyParameter <IPaths1G076VfDevicemanagementWindowsautopilotdeviceidentitiesWindowsautopilotdeviceidentityIdMicrosoftGraphAssignresourceaccounttodevicePostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### AssignViaIdentityExpanded
```
Set-MgBetaDeviceManagementWindowsAutopilotDeviceIdentityResourceAccountToDevice
 -InputObject <IDeviceManagementEnrollmentIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-AddressableUserName <String>] [-ResourceAccountName <String>]
 [-UserPrincipalName <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### AssignViaIdentity
```
Set-MgBetaDeviceManagementWindowsAutopilotDeviceIdentityResourceAccountToDevice
 -InputObject <IDeviceManagementEnrollmentIdentity>
 -BodyParameter <IPaths1G076VfDevicemanagementWindowsautopilotdeviceidentitiesWindowsautopilotdeviceidentityIdMicrosoftGraphAssignresourceaccounttodevicePostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Assigns resource account to Autopilot devices.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | DeviceManagementServiceConfig.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | DeviceManagementServiceConfig.ReadWrite.All,  |

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: AssignExpanded, AssignViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AddressableUserName


```yaml
Type: String
Parameter Sets: AssignExpanded, AssignViaIdentityExpanded
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
Type: IPaths1G076VfDevicemanagementWindowsautopilotdeviceidentitiesWindowsautopilotdeviceidentityIdMicrosoftGraphAssignresourceaccounttodevicePostRequestbodyContentApplicationJsonSchema
Parameter Sets: Assign, AssignViaIdentity
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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IDeviceManagementEnrollmentIdentity
Parameter Sets: AssignViaIdentityExpanded, AssignViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PassThru
Returns true when the command succeeds

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceAccountName


```yaml
Type: String
Parameter Sets: AssignExpanded, AssignViaIdentityExpanded
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

### -UserPrincipalName


```yaml
Type: String
Parameter Sets: AssignExpanded, AssignViaIdentityExpanded
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

### -WindowsAutopilotDeviceIdentityId
The unique identifier of windowsAutopilotDeviceIdentity

```yaml
Type: String
Parameter Sets: AssignExpanded, Assign
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

### Microsoft.Graph.Beta.PowerShell.Models.IDeviceManagementEnrollmentIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IPaths1G076VfDevicemanagementWindowsautopilotdeviceidentitiesWindowsautopilotdeviceidentityIdMicrosoftGraphAssignresourceaccounttodevicePostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPaths1G076VfDevicemanagementWindowsautopilotdeviceidentitiesWindowsautopilotdeviceidentityIdMicrosoftGraphAssignresourceaccounttodevicePostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AddressableUserName <String>]`: 
  - `[ResourceAccountName <String>]`: 
  - `[UserPrincipalName <String>]`: 

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

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.enrollment/set-mgbetadevicemanagementwindowsautopilotdeviceidentityresourceaccounttodevice](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.enrollment/set-mgbetadevicemanagementwindowsautopilotdeviceidentityresourceaccounttodevice)
























