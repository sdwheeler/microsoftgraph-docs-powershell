---
external help file: Microsoft.Graph.Beta.Devices.CorporateManagement-help.xml
Module Name: Microsoft.Graph.Beta.Devices.CorporateManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.corporatemanagement/update-mgbetadeviceappmanagementmanagedappregistration
schema: 2.0.0
---

# Update-MgBetaDeviceAppManagementManagedAppRegistration

## SYNOPSIS
Update the navigation property managedAppRegistrations in deviceAppManagement

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgDeviceAppManagementManagedAppRegistration](/powershell/module/Microsoft.Graph.Devices.CorporateManagement/Update-MgDeviceAppManagementManagedAppRegistration?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaDeviceAppManagementManagedAppRegistration -ManagedAppRegistrationId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-AppIdentifier <Hashtable>]
 [-ApplicationVersion <String>] [-AppliedPolicies <IMicrosoftGraphManagedAppPolicy[]>]
 [-AzureAdDeviceId <String>] [-CreatedDateTime <DateTime>] [-DeviceManufacturer <String>]
 [-DeviceModel <String>] [-DeviceName <String>] [-DeviceTag <String>] [-DeviceType <String>]
 [-FlaggedReasons <ManagedAppFlaggedReason[]>] [-Id <String>]
 [-IntendedPolicies <IMicrosoftGraphManagedAppPolicy[]>] [-LastSyncDateTime <DateTime>]
 [-ManagedAppLogCollectionRequests <IMicrosoftGraphManagedAppLogCollectionRequest[]>]
 [-ManagedDeviceId <String>] [-ManagementSdkVersion <String>]
 [-Operations <IMicrosoftGraphManagedAppOperation[]>] [-PlatformVersion <String>] [-UserId <String>]
 [-Version <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Update
```
Update-MgBetaDeviceAppManagementManagedAppRegistration -ManagedAppRegistrationId <String>
 -BodyParameter <IMicrosoftGraphManagedAppRegistration> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaDeviceAppManagementManagedAppRegistration -InputObject <IDevicesCorporateManagementIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-AppIdentifier <Hashtable>]
 [-ApplicationVersion <String>] [-AppliedPolicies <IMicrosoftGraphManagedAppPolicy[]>]
 [-AzureAdDeviceId <String>] [-CreatedDateTime <DateTime>] [-DeviceManufacturer <String>]
 [-DeviceModel <String>] [-DeviceName <String>] [-DeviceTag <String>] [-DeviceType <String>]
 [-FlaggedReasons <ManagedAppFlaggedReason[]>] [-Id <String>]
 [-IntendedPolicies <IMicrosoftGraphManagedAppPolicy[]>] [-LastSyncDateTime <DateTime>]
 [-ManagedAppLogCollectionRequests <IMicrosoftGraphManagedAppLogCollectionRequest[]>]
 [-ManagedDeviceId <String>] [-ManagementSdkVersion <String>]
 [-Operations <IMicrosoftGraphManagedAppOperation[]>] [-PlatformVersion <String>] [-UserId <String>]
 [-Version <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaDeviceAppManagementManagedAppRegistration -InputObject <IDevicesCorporateManagementIdentity>
 -BodyParameter <IMicrosoftGraphManagedAppRegistration> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property managedAppRegistrations in deviceAppManagement

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

### -AppIdentifier
The identifier for a mobile app.

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

### -ApplicationVersion
App version

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

### -AppliedPolicies
Zero or more policys already applied on the registered app when it last synchronized with managment service.
To construct, see NOTES section for APPLIEDPOLICIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphManagedAppPolicy[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AzureAdDeviceId
The Azure Active Directory Device identifier of the host device.
Value could be empty even when the host device is Azure Active Directory registered.

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

### -BodyParameter
The ManagedAppEntity is the base entity type for all other entity types under app management workflow.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphManagedAppRegistration
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
Date and time of creation

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

### -DeviceManufacturer
The device manufacturer for the current app registration

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

### -DeviceModel
The device model for the current app registration

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

### -DeviceName
Host device name

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

### -DeviceTag
App management SDK generated tag, which helps relate apps hosted on the same device.
Not guaranteed to relate apps in all conditions.

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

### -DeviceType
Host device type

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

### -FlaggedReasons
Zero or more reasons an app registration is flagged.
E.g.
app running on rooted device

```yaml
Type: ManagedAppFlaggedReason[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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

### -IntendedPolicies
Zero or more policies admin intended for the app as of now.
To construct, see NOTES section for INTENDEDPOLICIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphManagedAppPolicy[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastSyncDateTime
Date and time of last the app synced with management service.

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

### -ManagedAppLogCollectionRequests
Zero or more log collection requests triggered for the app.
To construct, see NOTES section for MANAGEDAPPLOGCOLLECTIONREQUESTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphManagedAppLogCollectionRequest[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ManagedAppRegistrationId
The unique identifier of managedAppRegistration

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

### -ManagedDeviceId
The Managed Device identifier of the host device.
Value could be empty even when the host device is managed.

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

### -ManagementSdkVersion
App management SDK version

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

### -Operations
Zero or more long running operations triggered on the app registration.
To construct, see NOTES section for OPERATIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphManagedAppOperation[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PlatformVersion
Operating System version

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

### -UserId
The user Id to who this app registration belongs.

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

### -Version
Version of the entity.

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

### Microsoft.Graph.Beta.PowerShell.Models.IDevicesCorporateManagementIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphManagedAppRegistration
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphManagedAppRegistration
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

APPLIEDPOLICIES `<IMicrosoftGraphManagedAppPolicy- `[]`>`: Zero or more policys already applied on the registered app when it last synchronized with managment service.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[CreatedDateTime <DateTime?>]`: The date and time the policy was created.
  - `[Description <String>]`: The policy's description.
  - `[DisplayName <String>]`: Policy display name.
  - `[LastModifiedDateTime <DateTime?>]`: Last time the policy was modified.
  - `[RoleScopeTagIds <String- `[]`>]`: List of Scope Tags for this Entity instance.
  - `[Version <String>]`: Version of the entity.

BODYPARAMETER `<IMicrosoftGraphManagedAppRegistration>`: The ManagedAppEntity is the base entity type for all other entity types under app management workflow.
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AppIdentifier <IMicrosoftGraphMobileAppIdentifier>]`: The identifier for a mobile app.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ApplicationVersion <String>]`: App version
  - `[AppliedPolicies <IMicrosoftGraphManagedAppPolicy- `[]`>]`: Zero or more policys already applied on the registered app when it last synchronized with managment service.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[CreatedDateTime <DateTime?>]`: The date and time the policy was created.
    - `[Description <String>]`: The policy's description.
    - `[DisplayName <String>]`: Policy display name.
    - `[LastModifiedDateTime <DateTime?>]`: Last time the policy was modified.
    - `[RoleScopeTagIds <String- `[]`>]`: List of Scope Tags for this Entity instance.
    - `[Version <String>]`: Version of the entity.
  - `[AzureAdDeviceId <String>]`: The Azure Active Directory Device identifier of the host device.
Value could be empty even when the host device is Azure Active Directory registered.
  - `[CreatedDateTime <DateTime?>]`: Date and time of creation
  - `[DeviceManufacturer <String>]`: The device manufacturer for the current app registration
  - `[DeviceModel <String>]`: The device model for the current app registration
  - `[DeviceName <String>]`: Host device name
  - `[DeviceTag <String>]`: App management SDK generated tag, which helps relate apps hosted on the same device.
Not guaranteed to relate apps in all conditions.
  - `[DeviceType <String>]`: Host device type
  - `[FlaggedReasons <ManagedAppFlaggedReason- `[]`>]`: Zero or more reasons an app registration is flagged.
E.g.
app running on rooted device
  - `[IntendedPolicies <IMicrosoftGraphManagedAppPolicy- `[]`>]`: Zero or more policies admin intended for the app as of now.
  - `[LastSyncDateTime <DateTime?>]`: Date and time of last the app synced with management service.
  - `[ManagedAppLogCollectionRequests <IMicrosoftGraphManagedAppLogCollectionRequest- `[]`>]`: Zero or more log collection requests triggered for the app.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[CompletedDateTime <DateTime?>]`: DateTime of when the log upload request was completed.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.
Returned by default.
Read-only.
    - `[ManagedAppRegistrationId <String>]`: The unique identifier of the app instance for which diagnostic logs were collected.
Read-only.
    - `[RequestedBy <String>]`: The user principal name associated with the request for the managed application log collection.
Read-only.
    - `[RequestedByUserPrincipalName <String>]`: The user principal name associated with the request for the managed application log collection.
Read-only.
    - `[RequestedDateTime <DateTime?>]`: DateTime of when the log upload request was received.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.
Returned by default.
Read-only.
    - `[Status <String>]`: Indicates the status for the app log collection request - pending, completed or failed.
Default is pending.
    - `[UploadedLogs <IMicrosoftGraphManagedAppLogUpload- `[]`>]`: The collection of log upload results as reported by each component on the device.
Such components can be the application itself, the Mobile Application Management (MAM) SDK, and other on-device components that are requested to upload diagnostic logs.
Read-only.
      - `[ManagedAppComponent <String>]`: The Mobile Application Management (MAM) Logs Uploading Component.
Such components can be the application itself, the MAM SDK, and other on-device components that are capable of uploading diagnostic logs.
Read-only.
      - `[ManagedAppComponentDescription <String>]`: The Mobile Application Management (MAM) Logs Uploading Component.
Such components can be the application itself, the MAM SDK, and other on-device components that are capable of uploading diagnostic logs.
Read-only.
      - `[ReferenceId <String>]`: A provider-specific reference id for the uploaded logs.
Read-only.
      - `[Status <ManagedAppLogUploadState?>]`: Represents the current status of the associated \`managedAppLogCollectionRequest\`.
    - `[UserLogUploadConsent <ManagedAppLogUploadConsent?>]`: Represents the current consent status of the associated \`managedAppLogCollectionRequest\`.
    - `[Version <String>]`: Version of the entity.
  - `[ManagedDeviceId <String>]`: The Managed Device identifier of the host device.
Value could be empty even when the host device is managed.
  - `[ManagementSdkVersion <String>]`: App management SDK version
  - `[Operations <IMicrosoftGraphManagedAppOperation- `[]`>]`: Zero or more long running operations triggered on the app registration.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: The operation name.
    - `[LastModifiedDateTime <DateTime?>]`: The last time the app operation was modified.
    - `[State <String>]`: The current state of the operation
    - `[Version <String>]`: Version of the entity.
  - `[PlatformVersion <String>]`: Operating System version
  - `[UserId <String>]`: The user Id to who this app registration belongs.
  - `[Version <String>]`: Version of the entity.

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

INTENDEDPOLICIES `<IMicrosoftGraphManagedAppPolicy- `[]`>`: Zero or more policies admin intended for the app as of now.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[CreatedDateTime <DateTime?>]`: The date and time the policy was created.
  - `[Description <String>]`: The policy's description.
  - `[DisplayName <String>]`: Policy display name.
  - `[LastModifiedDateTime <DateTime?>]`: Last time the policy was modified.
  - `[RoleScopeTagIds <String- `[]`>]`: List of Scope Tags for this Entity instance.
  - `[Version <String>]`: Version of the entity.

MANAGEDAPPLOGCOLLECTIONREQUESTS `<IMicrosoftGraphManagedAppLogCollectionRequest- `[]`>`: Zero or more log collection requests triggered for the app.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[CompletedDateTime <DateTime?>]`: DateTime of when the log upload request was completed.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.
Returned by default.
Read-only.
  - `[ManagedAppRegistrationId <String>]`: The unique identifier of the app instance for which diagnostic logs were collected.
Read-only.
  - `[RequestedBy <String>]`: The user principal name associated with the request for the managed application log collection.
Read-only.
  - `[RequestedByUserPrincipalName <String>]`: The user principal name associated with the request for the managed application log collection.
Read-only.
  - `[RequestedDateTime <DateTime?>]`: DateTime of when the log upload request was received.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.
Returned by default.
Read-only.
  - `[Status <String>]`: Indicates the status for the app log collection request - pending, completed or failed.
Default is pending.
  - `[UploadedLogs <IMicrosoftGraphManagedAppLogUpload- `[]`>]`: The collection of log upload results as reported by each component on the device.
Such components can be the application itself, the Mobile Application Management (MAM) SDK, and other on-device components that are requested to upload diagnostic logs.
Read-only.
    - `[ManagedAppComponent <String>]`: The Mobile Application Management (MAM) Logs Uploading Component.
Such components can be the application itself, the MAM SDK, and other on-device components that are capable of uploading diagnostic logs.
Read-only.
    - `[ManagedAppComponentDescription <String>]`: The Mobile Application Management (MAM) Logs Uploading Component.
Such components can be the application itself, the MAM SDK, and other on-device components that are capable of uploading diagnostic logs.
Read-only.
    - `[ReferenceId <String>]`: A provider-specific reference id for the uploaded logs.
Read-only.
    - `[Status <ManagedAppLogUploadState?>]`: Represents the current status of the associated \`managedAppLogCollectionRequest\`.
  - `[UserLogUploadConsent <ManagedAppLogUploadConsent?>]`: Represents the current consent status of the associated \`managedAppLogCollectionRequest\`.
  - `[Version <String>]`: Version of the entity.

OPERATIONS `<IMicrosoftGraphManagedAppOperation- `[]`>`: Zero or more long running operations triggered on the app registration.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DisplayName <String>]`: The operation name.
  - `[LastModifiedDateTime <DateTime?>]`: The last time the app operation was modified.
  - `[State <String>]`: The current state of the operation
  - `[Version <String>]`: Version of the entity.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.corporatemanagement/update-mgbetadeviceappmanagementmanagedappregistration](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.corporatemanagement/update-mgbetadeviceappmanagementmanagedappregistration)
























