---
external help file: Microsoft.Graph.Beta.Devices.CorporateManagement-help.xml
Module Name: Microsoft.Graph.Beta.Devices.CorporateManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.corporatemanagement/invoke-mgbetacommitdeviceappmanagementmobileappmicrosoftgraphwin32lobappcontentversionfile
schema: 2.0.0
---

# Invoke-MgBetaCommitDeviceAppManagementMobileAppMicrosoftGraphWin32LobAppContentVersionFile

## SYNOPSIS
Commits a file of a given app.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Invoke-MgCommitDeviceAppManagementMobileAppMicrosoftGraphWin32LobAppContentVersionFile](/powershell/module/Microsoft.Graph.Devices.CorporateManagement/Invoke-MgCommitDeviceAppManagementMobileAppMicrosoftGraphWin32LobAppContentVersionFile?view=graph-powershell-1.0)

## SYNTAX

### CommitExpanded (Default)
```
Invoke-MgBetaCommitDeviceAppManagementMobileAppMicrosoftGraphWin32LobAppContentVersionFile
 -MobileAppContentFileId <String> -MobileAppContentId <String> -MobileAppId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-FileEncryptionInfo <IMicrosoftGraphFileEncryptionInfo>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Commit
```
Invoke-MgBetaCommitDeviceAppManagementMobileAppMicrosoftGraphWin32LobAppContentVersionFile
 -MobileAppContentFileId <String> -MobileAppContentId <String> -MobileAppId <String>
 -BodyParameter <IPaths1RksdjoDeviceappmanagementMobileappsMobileappIdMicrosoftGraphWin32LobappContentversionsMobileappcontentIdFilesMobileappcontentfileIdMicrosoftGraphCommitPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CommitViaIdentityExpanded
```
Invoke-MgBetaCommitDeviceAppManagementMobileAppMicrosoftGraphWin32LobAppContentVersionFile
 -InputObject <IDevicesCorporateManagementIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-FileEncryptionInfo <IMicrosoftGraphFileEncryptionInfo>]
 [-Headers <IDictionary>] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### CommitViaIdentity
```
Invoke-MgBetaCommitDeviceAppManagementMobileAppMicrosoftGraphWin32LobAppContentVersionFile
 -InputObject <IDevicesCorporateManagementIdentity>
 -BodyParameter <IPaths1RksdjoDeviceappmanagementMobileappsMobileappIdMicrosoftGraphWin32LobappContentversionsMobileappcontentIdFilesMobileappcontentfileIdMicrosoftGraphCommitPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Commits a file of a given app.

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CommitExpanded, CommitViaIdentityExpanded
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
Type: IPaths1RksdjoDeviceappmanagementMobileappsMobileappIdMicrosoftGraphWin32LobappContentversionsMobileappcontentIdFilesMobileappcontentfileIdMicrosoftGraphCommitPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Commit, CommitViaIdentity
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

### -FileEncryptionInfo
Contains properties for file encryption information for the content version of a line-of-business app.
To construct, see NOTES section for FILEENCRYPTIONINFO properties and create a hash table.

```yaml
Type: IMicrosoftGraphFileEncryptionInfo
Parameter Sets: CommitExpanded, CommitViaIdentityExpanded
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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IDevicesCorporateManagementIdentity
Parameter Sets: CommitViaIdentityExpanded, CommitViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -MobileAppContentFileId
The unique identifier of mobileAppContentFile

```yaml
Type: String
Parameter Sets: CommitExpanded, Commit
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MobileAppContentId
The unique identifier of mobileAppContent

```yaml
Type: String
Parameter Sets: CommitExpanded, Commit
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MobileAppId
The unique identifier of mobileApp

```yaml
Type: String
Parameter Sets: CommitExpanded, Commit
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

### Microsoft.Graph.Beta.PowerShell.Models.IDevicesCorporateManagementIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IPaths1RksdjoDeviceappmanagementMobileappsMobileappIdMicrosoftGraphWin32LobappContentversionsMobileappcontentIdFilesMobileappcontentfileIdMicrosoftGraphCommitPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPaths1RksdjoDeviceappmanagementMobileappsMobileappIdMicrosoftGraphWin32LobappContentversionsMobileappcontentIdFilesMobileappcontentfileIdMicrosoftGraphCommitPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[FileEncryptionInfo <IMicrosoftGraphFileEncryptionInfo>]`: Contains properties for file encryption information for the content version of a line-of-business app.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[EncryptionKey <Byte- `[]`>]`: The key used to encrypt the file content.
    - `[FileDigest <Byte- `[]`>]`: The file digest prior to encryption.
ProfileVersion1 requires a non-null FileDigest.
    - `[FileDigestAlgorithm <String>]`: The file digest algorithm.
ProfileVersion1 currently only supports SHA256 for the FileDigestAlgorithm.
    - `[InitializationVector <Byte- `[]`>]`: The initialization vector (IV) used for the encryption algorithm.
Must be 16 bytes.
    - `[Mac <Byte- `[]`>]`: The hash of the concatenation of the IV and encrypted file content.
Must be 32 bytes.
    - `[MacKey <Byte- `[]`>]`: The key used to compute the message authentication code of the concatenation of the IV and encrypted file content.
Must be 32 bytes.
    - `[ProfileIdentifier <String>]`: The profile identifier.
Maps to the strategy used to encrypt the file.
Currently, only ProfileVersion1 is supported.

FILEENCRYPTIONINFO `<IMicrosoftGraphFileEncryptionInfo>`: Contains properties for file encryption information for the content version of a line-of-business app.
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[EncryptionKey <Byte- `[]`>]`: The key used to encrypt the file content.
  - `[FileDigest <Byte- `[]`>]`: The file digest prior to encryption.
ProfileVersion1 requires a non-null FileDigest.
  - `[FileDigestAlgorithm <String>]`: The file digest algorithm.
ProfileVersion1 currently only supports SHA256 for the FileDigestAlgorithm.
  - `[InitializationVector <Byte- `[]`>]`: The initialization vector (IV) used for the encryption algorithm.
Must be 16 bytes.
  - `[Mac <Byte- `[]`>]`: The hash of the concatenation of the IV and encrypted file content.
Must be 32 bytes.
  - `[MacKey <Byte- `[]`>]`: The key used to compute the message authentication code of the concatenation of the IV and encrypted file content.
Must be 32 bytes.
  - `[ProfileIdentifier <String>]`: The profile identifier.
Maps to the strategy used to encrypt the file.
Currently, only ProfileVersion1 is supported.

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

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.corporatemanagement/invoke-mgbetacommitdeviceappmanagementmobileappmicrosoftgraphwin32lobappcontentversionfile](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.corporatemanagement/invoke-mgbetacommitdeviceappmanagementmobileappmicrosoftgraphwin32lobappcontentversionfile)
























