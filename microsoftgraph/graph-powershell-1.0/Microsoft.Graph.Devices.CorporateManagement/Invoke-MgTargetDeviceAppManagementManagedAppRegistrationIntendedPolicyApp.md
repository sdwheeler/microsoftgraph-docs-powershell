---
external help file: Microsoft.Graph.Devices.CorporateManagement-help.xml
Module Name: Microsoft.Graph.Devices.CorporateManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.devices.corporatemanagement/invoke-mgtargetdeviceappmanagementmanagedappregistrationintendedpolicyapp
schema: 2.0.0
---

# Invoke-MgTargetDeviceAppManagementManagedAppRegistrationIntendedPolicyApp

## SYNOPSIS
Not yet documented

> [!NOTE]
> To view the beta release of this cmdlet, view [Invoke-MgBetaTargetDeviceAppManagementManagedAppRegistrationIntendedPolicyApp](/powershell/module/Microsoft.Graph.Beta.Devices.CorporateManagement/Invoke-MgBetaTargetDeviceAppManagementManagedAppRegistrationIntendedPolicyApp?view=graph-powershell-beta)

## SYNTAX

### TargetExpanded (Default)
```
Invoke-MgTargetDeviceAppManagementManagedAppRegistrationIntendedPolicyApp -ManagedAppPolicyId <String>
 -ManagedAppRegistrationId <String> [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Apps <IMicrosoftGraphManagedMobileApp[]>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Target
```
Invoke-MgTargetDeviceAppManagementManagedAppRegistrationIntendedPolicyApp -ManagedAppPolicyId <String>
 -ManagedAppRegistrationId <String>
 -BodyParameter <IPaths1Mv9GnvDeviceappmanagementManagedappregistrationsManagedappregistrationIdIntendedpoliciesManagedapppolicyIdMicrosoftGraphTargetappsPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### TargetViaIdentityExpanded
```
Invoke-MgTargetDeviceAppManagementManagedAppRegistrationIntendedPolicyApp
 -InputObject <IDevicesCorporateManagementIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Apps <IMicrosoftGraphManagedMobileApp[]>] [-Headers <IDictionary>]
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### TargetViaIdentity
```
Invoke-MgTargetDeviceAppManagementManagedAppRegistrationIntendedPolicyApp
 -InputObject <IDevicesCorporateManagementIdentity>
 -BodyParameter <IPaths1Mv9GnvDeviceappmanagementManagedappregistrationsManagedappregistrationIdIntendedpoliciesManagedapppolicyIdMicrosoftGraphTargetappsPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Not yet documented

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | DeviceManagementApps.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | DeviceManagementApps.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All,  |

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: TargetExpanded, TargetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Apps

To construct, see NOTES section for APPS properties and create a hash table.

```yaml
Type: IMicrosoftGraphManagedMobileApp[]
Parameter Sets: TargetExpanded, TargetViaIdentityExpanded
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
Type: IPaths1Mv9GnvDeviceappmanagementManagedappregistrationsManagedappregistrationIdIntendedpoliciesManagedapppolicyIdMicrosoftGraphTargetappsPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Target, TargetViaIdentity
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
Type: IDevicesCorporateManagementIdentity
Parameter Sets: TargetViaIdentityExpanded, TargetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ManagedAppPolicyId
The unique identifier of managedAppPolicy

```yaml
Type: String
Parameter Sets: TargetExpanded, Target
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ManagedAppRegistrationId
The unique identifier of managedAppRegistration

```yaml
Type: String
Parameter Sets: TargetExpanded, Target
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
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

### Microsoft.Graph.PowerShell.Models.IDevicesCorporateManagementIdentity
### Microsoft.Graph.PowerShell.Models.IPaths1Mv9GnvDeviceappmanagementManagedappregistrationsManagedappregistrationIdIntendedpoliciesManagedapppolicyIdMicrosoftGraphTargetappsPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

APPS `<IMicrosoftGraphManagedMobileApp- `[]`>`: .
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[MobileAppIdentifier <IMicrosoftGraphMobileAppIdentifier>]`: The identifier for a mobile app.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Version <String>]`: Version of the entity.

BODYPARAMETER `<IPaths1Mv9GnvDeviceappmanagementManagedappregistrationsManagedappregistrationIdIntendedpoliciesManagedapppolicyIdMicrosoftGraphTargetappsPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Apps <IMicrosoftGraphManagedMobileApp- `[]`>]`:
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[MobileAppIdentifier <IMicrosoftGraphMobileAppIdentifier>]`: The identifier for a mobile app.
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Version <String>]`: Version of the entity.

INPUTOBJECT `<IDevicesCorporateManagementIdentity>`: Identity Parameter
  - `[AndroidManagedAppProtectionId <String>]`: The unique identifier of androidManagedAppProtection
  - `[DefaultManagedAppProtectionId <String>]`: The unique identifier of defaultManagedAppProtection
  - `[DeviceCompliancePolicyStateId <String>]`: The unique identifier of deviceCompliancePolicyState
  - `[DeviceConfigurationStateId <String>]`: The unique identifier of deviceConfigurationState
  - `[DeviceInstallStateId <String>]`: The unique identifier of deviceInstallState
  - `[DeviceLogCollectionResponseId <String>]`: The unique identifier of deviceLogCollectionResponse
  - `[DeviceManagementTroubleshootingEventId <String>]`: The unique identifier of deviceManagementTroubleshootingEvent
  - `[IosManagedAppProtectionId <String>]`: The unique identifier of iosManagedAppProtection
  - `[ManagedAppOperationId <String>]`: The unique identifier of managedAppOperation
  - `[ManagedAppPolicyId <String>]`: The unique identifier of managedAppPolicy
  - `[ManagedAppRegistrationId <String>]`: The unique identifier of managedAppRegistration
  - `[ManagedAppStatusId <String>]`: The unique identifier of managedAppStatus
  - `[ManagedDeviceId <String>]`: The unique identifier of managedDevice
  - `[ManagedDeviceMobileAppConfigurationAssignmentId <String>]`: The unique identifier of managedDeviceMobileAppConfigurationAssignment
  - `[ManagedDeviceMobileAppConfigurationDeviceStatusId <String>]`: The unique identifier of managedDeviceMobileAppConfigurationDeviceStatus
  - `[ManagedDeviceMobileAppConfigurationId <String>]`: The unique identifier of managedDeviceMobileAppConfiguration
  - `[ManagedDeviceMobileAppConfigurationUserStatusId <String>]`: The unique identifier of managedDeviceMobileAppConfigurationUserStatus
  - `[ManagedEBookAssignmentId <String>]`: The unique identifier of managedEBookAssignment
  - `[ManagedEBookId <String>]`: The unique identifier of managedEBook
  - `[ManagedMobileAppId <String>]`: The unique identifier of managedMobileApp
  - `[MdmWindowsInformationProtectionPolicyId <String>]`: The unique identifier of mdmWindowsInformationProtectionPolicy
  - `[MobileAppAssignmentId <String>]`: The unique identifier of mobileAppAssignment
  - `[MobileAppCategoryId <String>]`: The unique identifier of mobileAppCategory
  - `[MobileAppContentFileId <String>]`: The unique identifier of mobileAppContentFile
  - `[MobileAppContentId <String>]`: The unique identifier of mobileAppContent
  - `[MobileAppId <String>]`: The unique identifier of mobileApp
  - `[MobileContainedAppId <String>]`: The unique identifier of mobileContainedApp
  - `[TargetedManagedAppConfigurationId <String>]`: The unique identifier of targetedManagedAppConfiguration
  - `[TargetedManagedAppPolicyAssignmentId <String>]`: The unique identifier of targetedManagedAppPolicyAssignment
  - `[UserId <String>]`: The unique identifier of user
  - `[UserInstallStateSummaryId <String>]`: The unique identifier of userInstallStateSummary
  - `[VppTokenId <String>]`: The unique identifier of vppToken
  - `[WindowsDeviceMalwareStateId <String>]`: The unique identifier of windowsDeviceMalwareState
  - `[WindowsInformationProtectionAppLockerFileId <String>]`: The unique identifier of windowsInformationProtectionAppLockerFile
  - `[WindowsInformationProtectionPolicyId <String>]`: The unique identifier of windowsInformationProtectionPolicy

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.devices.corporatemanagement/invoke-mgtargetdeviceappmanagementmanagedappregistrationintendedpolicyapp](https://learn.microsoft.com/powershell/module/microsoft.graph.devices.corporatemanagement/invoke-mgtargetdeviceappmanagementmanagedappregistrationintendedpolicyapp)

[https://learn.microsoft.com/graph/api/intune-mam-managedappprotection-targetapps?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/intune-mam-managedappprotection-targetapps?view=graph-rest-1.0)
























