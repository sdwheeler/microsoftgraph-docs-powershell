---
external help file: Microsoft.Graph.Beta.Devices.CorporateManagement-help.xml
Module Name: Microsoft.Graph.Beta.Devices.CorporateManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.corporatemanagement/update-mgbetadeviceappmanagementtargetedmanagedappconfigurationsetting
schema: 2.0.0
---

# Update-MgBetaDeviceAppManagementTargetedManagedAppConfigurationSetting

## SYNOPSIS
Update the navigation property settings in deviceAppManagement

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaDeviceAppManagementTargetedManagedAppConfigurationSetting
 -DeviceManagementConfigurationSettingId <String> -TargetedManagedAppConfigurationId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-Id <String>]
 [-SettingDefinitions <IMicrosoftGraphDeviceManagementConfigurationSettingDefinition[]>]
 [-SettingInstance <IMicrosoftGraphDeviceManagementConfigurationSettingInstance>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaDeviceAppManagementTargetedManagedAppConfigurationSetting
 -DeviceManagementConfigurationSettingId <String> -TargetedManagedAppConfigurationId <String>
 -BodyParameter <IMicrosoftGraphDeviceManagementConfigurationSetting> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaDeviceAppManagementTargetedManagedAppConfigurationSetting
 -InputObject <IDevicesCorporateManagementIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Id <String>]
 [-SettingDefinitions <IMicrosoftGraphDeviceManagementConfigurationSettingDefinition[]>]
 [-SettingInstance <IMicrosoftGraphDeviceManagementConfigurationSettingInstance>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaDeviceAppManagementTargetedManagedAppConfigurationSetting
 -InputObject <IDevicesCorporateManagementIdentity>
 -BodyParameter <IMicrosoftGraphDeviceManagementConfigurationSetting> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property settings in deviceAppManagement

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All,  |

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
Setting instance within policy
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphDeviceManagementConfigurationSetting
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

### -DeviceManagementConfigurationSettingId
The unique identifier of deviceManagementConfigurationSetting

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
Type: IDevicesCorporateManagementIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

### -SettingDefinitions
List of related Setting Definitions.
This property is read-only.
To construct, see NOTES section for SETTINGDEFINITIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphDeviceManagementConfigurationSettingDefinition[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SettingInstance
Setting instance within policy
To construct, see NOTES section for SETTINGINSTANCE properties and create a hash table.

```yaml
Type: IMicrosoftGraphDeviceManagementConfigurationSettingInstance
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TargetedManagedAppConfigurationId
The unique identifier of targetedManagedAppConfiguration

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

### Microsoft.Graph.Beta.PowerShell.Models.IDevicesCorporateManagementIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphDeviceManagementConfigurationSetting
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphDeviceManagementConfigurationSetting
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphDeviceManagementConfigurationSetting>`: Setting instance within policy
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[SettingDefinitions <IMicrosoftGraphDeviceManagementConfigurationSettingDefinition- `[]`>]`: List of related Setting Definitions.
This property is read-only.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AccessTypes <String>]`: deviceManagementConfigurationSettingAccessTypes
    - `[Applicability <IMicrosoftGraphDeviceManagementConfigurationSettingApplicability>]`: deviceManagementConfigurationSettingApplicability
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Description <String>]`: description of the setting
      - `[DeviceMode <DeviceManagementConfigurationDeviceMode?>]`: Describes applicability for the mode the device is in
      - `[Platform <DeviceManagementConfigurationPlatforms?>]`: Supported platform types.
      - `[Technologies <DeviceManagementConfigurationTechnologies?>]`: Describes which technology this setting can be deployed with
    - `[BaseUri <String>]`: Base CSP Path
    - `[CategoryId <String>]`: Specify category in which the setting is under.
Support $filters.
    - `[Description <String>]`: Description of the setting.
    - `[DisplayName <String>]`: Name of the setting.
For example: Allow Toast.
    - `[HelpText <String>]`: Help text of the setting.
Give more details of the setting.
    - `[InfoUrls <String- `[]`>]`: List of links more info for the setting can be found at.
    - `[Keywords <String- `[]`>]`: Tokens which to search settings on
    - `[Name <String>]`: Name of the item
    - `[Occurrence <IMicrosoftGraphDeviceManagementConfigurationSettingOccurrence>]`: deviceManagementConfigurationSettingOccurrence
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[MaxDeviceOccurrence <Int32?>]`: Maximum times setting can be set on device.
      - `[MinDeviceOccurrence <Int32?>]`: Minimum times setting can be set on device.
A MinDeviceOccurrence of 0 means setting is optional
    - `[OffsetUri <String>]`: Offset CSP Path from Base
    - `[ReferredSettingInformationList <IMicrosoftGraphDeviceManagementConfigurationReferredSettingInformation- `[]`>]`: List of referred setting information.
      - `[SettingDefinitionId <String>]`: Setting definition id that is being referred to a setting.
Applicable for reusable setting
    - `[RiskLevel <DeviceManagementConfigurationSettingRiskLevel?>]`: Setting RiskLevel
    - `[RootDefinitionId <String>]`: Root setting definition id if the setting is a child setting.
    - `[SettingUsage <DeviceManagementConfigurationSettingUsage?>]`: Supported setting types
    - `[UxBehavior <DeviceManagementConfigurationControlType?>]`: Setting control type representation in the UX
    - `[Version <String>]`: Item Version
    - `[Visibility <DeviceManagementConfigurationSettingVisibility?>]`: Supported setting types
  - `[SettingInstance <IMicrosoftGraphDeviceManagementConfigurationSettingInstance>]`: Setting instance within policy
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[SettingDefinitionId <String>]`: Setting Definition Id
    - `[SettingInstanceTemplateReference <IMicrosoftGraphDeviceManagementConfigurationSettingInstanceTemplateReference>]`: Setting instance template reference information
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[SettingInstanceTemplateId <String>]`: Setting instance template id

INPUTOBJECT `<IDevicesCorporateManagementIdentity>`: Identity Parameter
  - `[AndroidManagedAppProtectionId <String>]`: The unique identifier of androidManagedAppProtection
  - `[AppLogCollectionRequestId <String>]`: The unique identifier of appLogCollectionRequest
  - `[AssignmentFilterEvaluationStatusDetailsId <String>]`: The unique identifier of assignmentFilterEvaluationStatusDetails
  - `[BundleId <String>]`: Usage: bundleId='{bundleId}'
  - `[DefaultManagedAppProtectionId <String>]`: The unique identifier of defaultManagedAppProtection
  - `[DetectedAppId <String>]`: The unique identifier of detectedApp
  - `[DeviceAppManagementTaskId <String>]`: The unique identifier of deviceAppManagementTask
  - `[DeviceCompliancePolicyStateId <String>]`: The unique identifier of deviceCompliancePolicyState
  - `[DeviceConfigurationStateId <String>]`: The unique identifier of deviceConfigurationState
  - `[DeviceEnrollmentConfigurationId <String>]`: The unique identifier of deviceEnrollmentConfiguration
  - `[DeviceId <String>]`: Property in multi-part unique identifier of deviceHealthScriptPolicyState
  - `[DeviceInstallStateId <String>]`: The unique identifier of deviceInstallState
  - `[DeviceLogCollectionResponseId <String>]`: The unique identifier of deviceLogCollectionResponse
  - `[DeviceManagementConfigurationSettingDefinitionId <String>]`: The unique identifier of deviceManagementConfigurationSettingDefinition
  - `[DeviceManagementConfigurationSettingId <String>]`: The unique identifier of deviceManagementConfigurationSetting
  - `[DeviceManagementTroubleshootingEventId <String>]`: The unique identifier of deviceManagementTroubleshootingEvent
  - `[EnrollmentConfigurationAssignmentId <String>]`: The unique identifier of enrollmentConfigurationAssignment
  - `[EnterpriseCodeSigningCertificateId <String>]`: The unique identifier of enterpriseCodeSigningCertificate
  - `[Id <String>]`: Property in multi-part unique identifier of deviceHealthScriptPolicyState
  - `[IosLobAppProvisioningConfigurationAssignmentId <String>]`: The unique identifier of iosLobAppProvisioningConfigurationAssignment
  - `[IosLobAppProvisioningConfigurationId <String>]`: The unique identifier of iosLobAppProvisioningConfiguration
  - `[IosManagedAppProtectionId <String>]`: The unique identifier of iosManagedAppProtection
  - `[IosVppAppAssignedLicenseId <String>]`: The unique identifier of iosVppAppAssignedLicense
  - `[ManagedAppLogCollectionRequestId <String>]`: The unique identifier of managedAppLogCollectionRequest
  - `[ManagedAppOperationId <String>]`: The unique identifier of managedAppOperation
  - `[ManagedAppPolicyId <String>]`: The unique identifier of managedAppPolicy
  - `[ManagedAppRegistrationId <String>]`: The unique identifier of managedAppRegistration
  - `[ManagedAppStatusId <String>]`: The unique identifier of managedAppStatus
  - `[ManagedDeviceId <String>]`: The unique identifier of managedDevice
  - `[ManagedDeviceMobileAppConfigurationAssignmentId <String>]`: The unique identifier of managedDeviceMobileAppConfigurationAssignment
  - `[ManagedDeviceMobileAppConfigurationDeviceStatusId <String>]`: The unique identifier of managedDeviceMobileAppConfigurationDeviceStatus
  - `[ManagedDeviceMobileAppConfigurationId <String>]`: The unique identifier of managedDeviceMobileAppConfiguration
  - `[ManagedDeviceMobileAppConfigurationStateId <String>]`: The unique identifier of managedDeviceMobileAppConfigurationState
  - `[ManagedDeviceMobileAppConfigurationUserStatusId <String>]`: The unique identifier of managedDeviceMobileAppConfigurationUserStatus
  - `[ManagedEBookAssignmentId <String>]`: The unique identifier of managedEBookAssignment
  - `[ManagedEBookCategoryId <String>]`: The unique identifier of managedEBookCategory
  - `[ManagedEBookId <String>]`: The unique identifier of managedEBook
  - `[ManagedMobileAppId <String>]`: The unique identifier of managedMobileApp
  - `[MdmWindowsInformationProtectionPolicyId <String>]`: The unique identifier of mdmWindowsInformationProtectionPolicy
  - `[MobileAppAssignmentId <String>]`: The unique identifier of mobileAppAssignment
  - `[MobileAppCatalogPackageId <String>]`: The unique identifier of mobileAppCatalogPackage
  - `[MobileAppCategoryId <String>]`: The unique identifier of mobileAppCategory
  - `[MobileAppContentFileId <String>]`: The unique identifier of mobileAppContentFile
  - `[MobileAppContentId <String>]`: The unique identifier of mobileAppContent
  - `[MobileAppId <String>]`: The unique identifier of mobileApp
  - `[MobileAppIntentAndStateId <String>]`: The unique identifier of mobileAppIntentAndState
  - `[MobileAppProvisioningConfigGroupAssignmentId <String>]`: The unique identifier of mobileAppProvisioningConfigGroupAssignment
  - `[MobileAppRelationshipId <String>]`: The unique identifier of mobileAppRelationship
  - `[MobileAppTroubleshootingEventId <String>]`: The unique identifier of mobileAppTroubleshootingEvent
  - `[MobileContainedAppId <String>]`: The unique identifier of mobileContainedApp
  - `[PolicyId <String>]`: Property in multi-part unique identifier of deviceHealthScriptPolicyState
  - `[PolicySetAssignmentId <String>]`: The unique identifier of policySetAssignment
  - `[PolicySetId <String>]`: The unique identifier of policySet
  - `[PolicySetItemId <String>]`: The unique identifier of policySetItem
  - `[SecurityBaselineSettingStateId <String>]`: The unique identifier of securityBaselineSettingState
  - `[SecurityBaselineStateId <String>]`: The unique identifier of securityBaselineState
  - `[TargetedManagedAppConfigurationId <String>]`: The unique identifier of targetedManagedAppConfiguration
  - `[TargetedManagedAppPolicyAssignmentId <String>]`: The unique identifier of targetedManagedAppPolicyAssignment
  - `[Upn <String>]`: Usage: upn='{upn}'
  - `[UserId <String>]`: The unique identifier of user
  - `[UserInstallStateSummaryId <String>]`: The unique identifier of userInstallStateSummary
  - `[UserPrincipalName <String>]`: Usage: userPrincipalName='{userPrincipalName}'
  - `[VppTokenId <String>]`: The unique identifier of vppToken
  - `[WindowsDefenderApplicationControlSupplementalPolicyAssignmentId <String>]`: The unique identifier of windowsDefenderApplicationControlSupplementalPolicyAssignment
  - `[WindowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId <String>]`: The unique identifier of windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus
  - `[WindowsDefenderApplicationControlSupplementalPolicyId <String>]`: The unique identifier of windowsDefenderApplicationControlSupplementalPolicy
  - `[WindowsDeviceMalwareStateId <String>]`: The unique identifier of windowsDeviceMalwareState
  - `[WindowsInformationProtectionAppLockerFileId <String>]`: The unique identifier of windowsInformationProtectionAppLockerFile
  - `[WindowsInformationProtectionDeviceRegistrationId <String>]`: The unique identifier of windowsInformationProtectionDeviceRegistration
  - `[WindowsInformationProtectionPolicyId <String>]`: The unique identifier of windowsInformationProtectionPolicy
  - `[WindowsInformationProtectionWipeActionId <String>]`: The unique identifier of windowsInformationProtectionWipeAction
  - `[WindowsManagedAppProtectionId <String>]`: The unique identifier of windowsManagedAppProtection

SETTINGDEFINITIONS `<IMicrosoftGraphDeviceManagementConfigurationSettingDefinition- `[]`>`: List of related Setting Definitions.
This property is read-only.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AccessTypes <String>]`: deviceManagementConfigurationSettingAccessTypes
  - `[Applicability <IMicrosoftGraphDeviceManagementConfigurationSettingApplicability>]`: deviceManagementConfigurationSettingApplicability
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Description <String>]`: description of the setting
    - `[DeviceMode <DeviceManagementConfigurationDeviceMode?>]`: Describes applicability for the mode the device is in
    - `[Platform <DeviceManagementConfigurationPlatforms?>]`: Supported platform types.
    - `[Technologies <DeviceManagementConfigurationTechnologies?>]`: Describes which technology this setting can be deployed with
  - `[BaseUri <String>]`: Base CSP Path
  - `[CategoryId <String>]`: Specify category in which the setting is under.
Support $filters.
  - `[Description <String>]`: Description of the setting.
  - `[DisplayName <String>]`: Name of the setting.
For example: Allow Toast.
  - `[HelpText <String>]`: Help text of the setting.
Give more details of the setting.
  - `[InfoUrls <String- `[]`>]`: List of links more info for the setting can be found at.
  - `[Keywords <String- `[]`>]`: Tokens which to search settings on
  - `[Name <String>]`: Name of the item
  - `[Occurrence <IMicrosoftGraphDeviceManagementConfigurationSettingOccurrence>]`: deviceManagementConfigurationSettingOccurrence
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[MaxDeviceOccurrence <Int32?>]`: Maximum times setting can be set on device.
    - `[MinDeviceOccurrence <Int32?>]`: Minimum times setting can be set on device.
A MinDeviceOccurrence of 0 means setting is optional
  - `[OffsetUri <String>]`: Offset CSP Path from Base
  - `[ReferredSettingInformationList <IMicrosoftGraphDeviceManagementConfigurationReferredSettingInformation- `[]`>]`: List of referred setting information.
    - `[SettingDefinitionId <String>]`: Setting definition id that is being referred to a setting.
Applicable for reusable setting
  - `[RiskLevel <DeviceManagementConfigurationSettingRiskLevel?>]`: Setting RiskLevel
  - `[RootDefinitionId <String>]`: Root setting definition id if the setting is a child setting.
  - `[SettingUsage <DeviceManagementConfigurationSettingUsage?>]`: Supported setting types
  - `[UxBehavior <DeviceManagementConfigurationControlType?>]`: Setting control type representation in the UX
  - `[Version <String>]`: Item Version
  - `[Visibility <DeviceManagementConfigurationSettingVisibility?>]`: Supported setting types

SETTINGINSTANCE `<IMicrosoftGraphDeviceManagementConfigurationSettingInstance>`: Setting instance within policy
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[SettingDefinitionId <String>]`: Setting Definition Id
  - `[SettingInstanceTemplateReference <IMicrosoftGraphDeviceManagementConfigurationSettingInstanceTemplateReference>]`: Setting instance template reference information
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[SettingInstanceTemplateId <String>]`: Setting instance template id

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.corporatemanagement/update-mgbetadeviceappmanagementtargetedmanagedappconfigurationsetting](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.corporatemanagement/update-mgbetadeviceappmanagementtargetedmanagedappconfigurationsetting)
























