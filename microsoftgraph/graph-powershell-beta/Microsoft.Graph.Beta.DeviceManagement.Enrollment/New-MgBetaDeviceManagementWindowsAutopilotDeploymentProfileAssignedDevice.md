---
external help file: Microsoft.Graph.Beta.DeviceManagement.Enrollment-help.xml
Module Name: Microsoft.Graph.Beta.DeviceManagement.Enrollment
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.enrollment/new-mgbetadevicemanagementwindowsautopilotdeploymentprofileassigneddevice
schema: 2.0.0
---

# New-MgBetaDeviceManagementWindowsAutopilotDeploymentProfileAssignedDevice

## SYNOPSIS
Create new navigation property to assignedDevices for deviceManagement

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaDeviceManagementWindowsAutopilotDeploymentProfileAssignedDevice
 -WindowsAutopilotDeploymentProfileId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-AddressableUserName <String>] [-AzureActiveDirectoryDeviceId <String>]
 [-AzureAdDeviceId <String>] [-DeploymentProfile <IMicrosoftGraphWindowsAutopilotDeploymentProfile>]
 [-DeploymentProfileAssignedDateTime <DateTime>]
 [-DeploymentProfileAssignmentDetailedStatus <WindowsAutopilotProfileAssignmentDetailedStatus>]
 [-DeploymentProfileAssignmentStatus <WindowsAutopilotProfileAssignmentStatus>]
 [-DeviceAccountPassword <String>] [-DeviceAccountUpn <String>] [-DeviceFriendlyName <String>]
 [-DisplayName <String>] [-EnrollmentState <EnrollmentState>] [-GroupTag <String>] [-Id <String>]
 [-IntendedDeploymentProfile <IMicrosoftGraphWindowsAutopilotDeploymentProfile>]
 [-LastContactedDateTime <DateTime>] [-ManagedDeviceId <String>] [-Manufacturer <String>] [-Model <String>]
 [-ProductKey <String>] [-PurchaseOrderIdentifier <String>]
 [-RemediationState <WindowsAutopilotDeviceRemediationState>]
 [-RemediationStateLastModifiedDateTime <DateTime>] [-ResourceName <String>] [-SerialNumber <String>]
 [-SkuNumber <String>] [-SystemFamily <String>] [-UserPrincipalName <String>]
 [-UserlessEnrollmentStatus <WindowsAutopilotUserlessEnrollmentStatus>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaDeviceManagementWindowsAutopilotDeploymentProfileAssignedDevice
 -WindowsAutopilotDeploymentProfileId <String> -BodyParameter <IMicrosoftGraphWindowsAutopilotDeviceIdentity>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgBetaDeviceManagementWindowsAutopilotDeploymentProfileAssignedDevice
 -InputObject <IDeviceManagementEnrollmentIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-AddressableUserName <String>] [-AzureActiveDirectoryDeviceId <String>]
 [-AzureAdDeviceId <String>] [-DeploymentProfile <IMicrosoftGraphWindowsAutopilotDeploymentProfile>]
 [-DeploymentProfileAssignedDateTime <DateTime>]
 [-DeploymentProfileAssignmentDetailedStatus <WindowsAutopilotProfileAssignmentDetailedStatus>]
 [-DeploymentProfileAssignmentStatus <WindowsAutopilotProfileAssignmentStatus>]
 [-DeviceAccountPassword <String>] [-DeviceAccountUpn <String>] [-DeviceFriendlyName <String>]
 [-DisplayName <String>] [-EnrollmentState <EnrollmentState>] [-GroupTag <String>] [-Id <String>]
 [-IntendedDeploymentProfile <IMicrosoftGraphWindowsAutopilotDeploymentProfile>]
 [-LastContactedDateTime <DateTime>] [-ManagedDeviceId <String>] [-Manufacturer <String>] [-Model <String>]
 [-ProductKey <String>] [-PurchaseOrderIdentifier <String>]
 [-RemediationState <WindowsAutopilotDeviceRemediationState>]
 [-RemediationStateLastModifiedDateTime <DateTime>] [-ResourceName <String>] [-SerialNumber <String>]
 [-SkuNumber <String>] [-SystemFamily <String>] [-UserPrincipalName <String>]
 [-UserlessEnrollmentStatus <WindowsAutopilotUserlessEnrollmentStatus>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgBetaDeviceManagementWindowsAutopilotDeploymentProfileAssignedDevice
 -InputObject <IDeviceManagementEnrollmentIdentity>
 -BodyParameter <IMicrosoftGraphWindowsAutopilotDeviceIdentity> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to assignedDevices for deviceManagement

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

### -AddressableUserName
Addressable user name.

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

### -AzureActiveDirectoryDeviceId
AAD Device ID - to be deprecated

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

### -AzureAdDeviceId
AAD Device ID

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
The windowsAutopilotDeviceIdentity resource represents a Windows Autopilot Device.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsAutopilotDeviceIdentity
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

### -DeploymentProfile
Windows Autopilot Deployment Profile
To construct, see NOTES section for DEPLOYMENTPROFILE properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsAutopilotDeploymentProfile
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeploymentProfileAssignedDateTime
Profile set time of the Windows autopilot device.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeploymentProfileAssignmentDetailedStatus
windowsAutopilotProfileAssignmentDetailedStatus

```yaml
Type: WindowsAutopilotProfileAssignmentDetailedStatus
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeploymentProfileAssignmentStatus
windowsAutopilotProfileAssignmentStatus

```yaml
Type: WindowsAutopilotProfileAssignmentStatus
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceAccountPassword
Surface Hub Device Account Password

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

### -DeviceAccountUpn
Surface Hub Device Account Upn

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

### -DeviceFriendlyName
Surface Hub Device Friendly Name

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
Display Name

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

### -EnrollmentState
enrollmentState

```yaml
Type: EnrollmentState
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GroupTag
Group Tag of the Windows autopilot device.

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

### -IntendedDeploymentProfile
Windows Autopilot Deployment Profile
To construct, see NOTES section for INTENDEDDEPLOYMENTPROFILE properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsAutopilotDeploymentProfile
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastContactedDateTime
Intune Last Contacted Date Time of the Windows autopilot device.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ManagedDeviceId
Managed Device ID

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

### -Manufacturer
Oem manufacturer of the Windows autopilot device.

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

### -Model
Model name of the Windows autopilot device.

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

### -ProductKey
Product Key of the Windows autopilot device.

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

### -PurchaseOrderIdentifier
Purchase Order Identifier of the Windows autopilot device.

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

### -RemediationState
Device remediation status, indicating whether or not hardware has been changed for an Autopilot-registered device.

```yaml
Type: WindowsAutopilotDeviceRemediationState
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemediationStateLastModifiedDateTime
RemediationState set time of Autopilot device.

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceName
Resource Name.

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

### -SerialNumber
Serial number of the Windows autopilot device.

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

### -SkuNumber
SKU Number

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

### -SystemFamily
System Family

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

### -UserlessEnrollmentStatus
Userless enrollment block status, indicating whether the next device enrollment will be blocked.

```yaml
Type: WindowsAutopilotUserlessEnrollmentStatus
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserPrincipalName
User Principal Name.

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

### -WindowsAutopilotDeploymentProfileId
The unique identifier of windowsAutopilotDeploymentProfile

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IDeviceManagementEnrollmentIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphWindowsAutopilotDeviceIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphWindowsAutopilotDeviceIdentity
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphWindowsAutopilotDeviceIdentity>`: The windowsAutopilotDeviceIdentity resource represents a Windows Autopilot Device.
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AddressableUserName <String>]`: Addressable user name.
  - `[AzureActiveDirectoryDeviceId <String>]`: AAD Device ID - to be deprecated
  - `[AzureAdDeviceId <String>]`: AAD Device ID
  - `[DeploymentProfile <IMicrosoftGraphWindowsAutopilotDeploymentProfile>]`: Windows Autopilot Deployment Profile
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AssignedDevices <IMicrosoftGraphWindowsAutopilotDeviceIdentity- `[]`>]`: The list of assigned devices for the profile.
    - `[Assignments <IMicrosoftGraphWindowsAutopilotDeploymentProfileAssignment- `[]`>]`: The list of group assignments for the profile.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Source <DeviceAndAppManagementAssignmentSource?>]`: Represents source of assignment.
      - `[SourceId <String>]`: Identifier for resource used for deployment to a group
      - `[Target <IMicrosoftGraphDeviceAndAppManagementAssignmentTarget>]`: Base type for assignment targets.
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DeviceAndAppManagementAssignmentFilterId <String>]`: The ID of the filter for the target assignment.
        - `[DeviceAndAppManagementAssignmentFilterType <DeviceAndAppManagementAssignmentFilterType?>]`: Represents type of the assignment filter.
    - `[CreatedDateTime <DateTime?>]`: The date and time of when the deployment profile was created.
The value cannot be modified and is automatically populated when the profile was created.
The timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
Read-Only.
    - `[Description <String>]`: A description of the deployment profile.
Max allowed length is 1500 chars.
Supports: $select, $top, $skip, $orderBy.
$Search and $filter are not supported.
    - `[DeviceNameTemplate <String>]`: The template used to name the Autopilot device.
This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.
The total length of the text generated by the template can be no more than 15 characters.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
    - `[DeviceType <WindowsAutopilotDeviceType?>]`: windowsAutopilotDeviceType
    - `[DisplayName <String>]`: The display name of the deployment profile.
Max allowed length is 200 chars.
Returned by default.
Supports: $select, $top, $skip, $orderby.
$Search and $filter are not supported.
    - `[EnableWhiteGlove <Boolean?>]`: Indicates whether the user is allowed to use Windows Autopilot for pre-provisioned deployment mode during Out of Box experience (OOBE).
When TRUE, indicates that Windows Autopilot for pre-provisioned deployment mode is allowed.
When false, Windows Autopilot for pre-provisioned deployment mode is not allowed.
The default is FALSE.
Read-Only.
Starting from May 2024 this property will no longer be supported and will be marked as deprecated.
Use preprovisioningAllowed instead.
    - `[EnrollmentStatusScreenSettings <IMicrosoftGraphWindowsEnrollmentStatusScreenSettings>]`: Enrollment status screen setting
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[AllowDeviceUseBeforeProfileAndAppInstallComplete <Boolean?>]`: Allow or block user to use device before profile and app installation complete
      - `[AllowDeviceUseOnInstallFailure <Boolean?>]`: Allow the user to continue using the device on installation failure
      - `[AllowLogCollectionOnInstallFailure <Boolean?>]`: Allow or block log collection on installation failure
      - `[BlockDeviceSetupRetryByUser <Boolean?>]`: Allow the user to retry the setup on installation failure
      - `[CustomErrorMessage <String>]`: Set custom error message to show upon installation failure
      - `[HideInstallationProgress <Boolean?>]`: Show or hide installation progress to user
      - `[InstallProgressTimeoutInMinutes <Int32?>]`: Set installation progress timeout in minutes
    - `[ExtractHardwareHash <Boolean?>]`: Indicates whether the profile supports the extraction of hardware hash values and registration of the device into Windows Autopilot.
When TRUE, indicates if hardware extraction and Windows Autopilot registration will happen on the next successful check-in.
When FALSE, hardware hash extraction and Windows Autopilot registration will not happen.
Default value is FALSE.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
Read-Only.
Starting from May 2024 this property will no longer be supported and will be marked as deprecated.
Use hardwareHashExtractionEnabled instead.
    - `[HardwareHashExtractionEnabled <Boolean?>]`: Indicates whether the profile supports the extraction of hardware hash values and registration of the device into Windows Autopilot.
When TRUE, indicates if hardware extraction and Windows Autopilot registration will happen on the next successful check-in.
When FALSE, hardware hash extraction and Windows Autopilot registration will not happen.
Default value is FALSE.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
    - `[Language <String>]`: The language code to be used when configuring the device.
E.g.
en-US.
The default value is os-default.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
Read-Only.
Starting from May 2024 this property will no longer be supported and will be marked as deprecated.
Use locale instead.
    - `[LastModifiedDateTime <DateTime?>]`: The date and time of when the deployment profile was last modified.
The value cannot be updated manually and is automatically populated when any changes are made to the profile.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported Read-Only.
    - `[Locale <String>]`: The locale (language) to be used when configuring the device.
E.g.
en-US.
The default value is os-default.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
    - `[ManagementServiceAppId <String>]`: The Entra management service App ID which gets used during client device-based enrollment discovery.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
    - `[OutOfBoxExperienceSetting <IMicrosoftGraphOutOfBoxExperienceSetting>]`: The Windows Autopilot Deployment Profile settings used by the device for the out-of-box experience.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DeviceUsageType <WindowsDeviceUsageType?>]`: windowsDeviceUsageType
      - `[EscapeLinkHidden <Boolean?>]`: When TRUE, the link that allows user to start over with a different account on company sign-in is hidden.
When false, the link that allows user to start over with a different account on company sign-in is available.
Default value is FALSE.
      - `[EulaHidden <Boolean?>]`: When TRUE, EULA is hidden to the end user during OOBE.
When FALSE, EULA is shown to the end user during OOBE.
Default value is FALSE.
      - `[KeyboardSelectionPageSkipped <Boolean?>]`: When TRUE, the keyboard selection page is hidden to the end user during OOBE if Language and Region are set.
When FALSE, the keyboard selection page is skipped during OOBE.
      - `[PrivacySettingsHidden <Boolean?>]`: When TRUE, privacy settings is hidden to the end user during OOBE.
When FALSE, privacy settings is shown to the end user during OOBE.
Default value is FALSE.
      - `[UserType <WindowsUserType?>]`: windowsUserType
    - `[OutOfBoxExperienceSettings <IMicrosoftGraphOutOfBoxExperienceSettings>]`: The Windows Autopilot Deployment Profile settings used by the Autopilot device for out-of-box experience.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
Read-Only.
Starting from May 2024 this property will no longer be supported and will be marked as deprecated.
Use outOfBoxExperienceSetting instead.
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DeviceUsageType <WindowsDeviceUsageType?>]`: windowsDeviceUsageType
      - `[HideEscapeLink <Boolean?>]`: If set to true, then the user can't start over with different account, on company sign-in
      - `[HideEula <Boolean?>]`: Show or hide EULA to user
      - `[HidePrivacySettings <Boolean?>]`: Show or hide privacy settings to user
      - `[SkipKeyboardSelectionPage <Boolean?>]`: If set, then skip the keyboard selection page if Language and Region are set
      - `[UserType <WindowsUserType?>]`: windowsUserType
    - `[PreprovisioningAllowed <Boolean?>]`: Indicates whether the user is allowed to use Windows Autopilot for pre-provisioned deployment mode during Out of Box experience (OOBE).
When TRUE, indicates that Windows Autopilot for pre-provisioned deployment mode for OOBE is allowed to be used.
When false, Windows Autopilot for pre-provisioned deployment mode for OOBE is not allowed.
The default is FALSE.
    - `[RoleScopeTagIds <String- `[]`>]`: List of role scope tags for the deployment profile.
  - `[DeploymentProfileAssignedDateTime <DateTime?>]`: Profile set time of the Windows autopilot device.
  - `[DeploymentProfileAssignmentDetailedStatus <WindowsAutopilotProfileAssignmentDetailedStatus?>]`: windowsAutopilotProfileAssignmentDetailedStatus
  - `[DeploymentProfileAssignmentStatus <WindowsAutopilotProfileAssignmentStatus?>]`: windowsAutopilotProfileAssignmentStatus
  - `[DeviceAccountPassword <String>]`: Surface Hub Device Account Password
  - `[DeviceAccountUpn <String>]`: Surface Hub Device Account Upn
  - `[DeviceFriendlyName <String>]`: Surface Hub Device Friendly Name
  - `[DisplayName <String>]`: Display Name
  - `[EnrollmentState <EnrollmentState?>]`: enrollmentState
  - `[GroupTag <String>]`: Group Tag of the Windows autopilot device.
  - `[IntendedDeploymentProfile <IMicrosoftGraphWindowsAutopilotDeploymentProfile>]`: Windows Autopilot Deployment Profile
  - `[LastContactedDateTime <DateTime?>]`: Intune Last Contacted Date Time of the Windows autopilot device.
  - `[ManagedDeviceId <String>]`: Managed Device ID
  - `[Manufacturer <String>]`: Oem manufacturer of the Windows autopilot device.
  - `[Model <String>]`: Model name of the Windows autopilot device.
  - `[ProductKey <String>]`: Product Key of the Windows autopilot device.
  - `[PurchaseOrderIdentifier <String>]`: Purchase Order Identifier of the Windows autopilot device.
  - `[RemediationState <WindowsAutopilotDeviceRemediationState?>]`: Device remediation status, indicating whether or not hardware has been changed for an Autopilot-registered device.
  - `[RemediationStateLastModifiedDateTime <DateTime?>]`: RemediationState set time of Autopilot device.
  - `[ResourceName <String>]`: Resource Name.
  - `[SerialNumber <String>]`: Serial number of the Windows autopilot device.
  - `[SkuNumber <String>]`: SKU Number
  - `[SystemFamily <String>]`: System Family
  - `[UserPrincipalName <String>]`: User Principal Name.
  - `[UserlessEnrollmentStatus <WindowsAutopilotUserlessEnrollmentStatus?>]`: Userless enrollment block status, indicating whether the next device enrollment will be blocked.

DEPLOYMENTPROFILE `<IMicrosoftGraphWindowsAutopilotDeploymentProfile>`: Windows Autopilot Deployment Profile
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AssignedDevices <IMicrosoftGraphWindowsAutopilotDeviceIdentity- `[]`>]`: The list of assigned devices for the profile.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AddressableUserName <String>]`: Addressable user name.
    - `[AzureActiveDirectoryDeviceId <String>]`: AAD Device ID - to be deprecated
    - `[AzureAdDeviceId <String>]`: AAD Device ID
    - `[DeploymentProfile <IMicrosoftGraphWindowsAutopilotDeploymentProfile>]`: Windows Autopilot Deployment Profile
    - `[DeploymentProfileAssignedDateTime <DateTime?>]`: Profile set time of the Windows autopilot device.
    - `[DeploymentProfileAssignmentDetailedStatus <WindowsAutopilotProfileAssignmentDetailedStatus?>]`: windowsAutopilotProfileAssignmentDetailedStatus
    - `[DeploymentProfileAssignmentStatus <WindowsAutopilotProfileAssignmentStatus?>]`: windowsAutopilotProfileAssignmentStatus
    - `[DeviceAccountPassword <String>]`: Surface Hub Device Account Password
    - `[DeviceAccountUpn <String>]`: Surface Hub Device Account Upn
    - `[DeviceFriendlyName <String>]`: Surface Hub Device Friendly Name
    - `[DisplayName <String>]`: Display Name
    - `[EnrollmentState <EnrollmentState?>]`: enrollmentState
    - `[GroupTag <String>]`: Group Tag of the Windows autopilot device.
    - `[IntendedDeploymentProfile <IMicrosoftGraphWindowsAutopilotDeploymentProfile>]`: Windows Autopilot Deployment Profile
    - `[LastContactedDateTime <DateTime?>]`: Intune Last Contacted Date Time of the Windows autopilot device.
    - `[ManagedDeviceId <String>]`: Managed Device ID
    - `[Manufacturer <String>]`: Oem manufacturer of the Windows autopilot device.
    - `[Model <String>]`: Model name of the Windows autopilot device.
    - `[ProductKey <String>]`: Product Key of the Windows autopilot device.
    - `[PurchaseOrderIdentifier <String>]`: Purchase Order Identifier of the Windows autopilot device.
    - `[RemediationState <WindowsAutopilotDeviceRemediationState?>]`: Device remediation status, indicating whether or not hardware has been changed for an Autopilot-registered device.
    - `[RemediationStateLastModifiedDateTime <DateTime?>]`: RemediationState set time of Autopilot device.
    - `[ResourceName <String>]`: Resource Name.
    - `[SerialNumber <String>]`: Serial number of the Windows autopilot device.
    - `[SkuNumber <String>]`: SKU Number
    - `[SystemFamily <String>]`: System Family
    - `[UserPrincipalName <String>]`: User Principal Name.
    - `[UserlessEnrollmentStatus <WindowsAutopilotUserlessEnrollmentStatus?>]`: Userless enrollment block status, indicating whether the next device enrollment will be blocked.
  - `[Assignments <IMicrosoftGraphWindowsAutopilotDeploymentProfileAssignment- `[]`>]`: The list of group assignments for the profile.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Source <DeviceAndAppManagementAssignmentSource?>]`: Represents source of assignment.
    - `[SourceId <String>]`: Identifier for resource used for deployment to a group
    - `[Target <IMicrosoftGraphDeviceAndAppManagementAssignmentTarget>]`: Base type for assignment targets.
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DeviceAndAppManagementAssignmentFilterId <String>]`: The ID of the filter for the target assignment.
      - `[DeviceAndAppManagementAssignmentFilterType <DeviceAndAppManagementAssignmentFilterType?>]`: Represents type of the assignment filter.
  - `[CreatedDateTime <DateTime?>]`: The date and time of when the deployment profile was created.
The value cannot be modified and is automatically populated when the profile was created.
The timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
Read-Only.
  - `[Description <String>]`: A description of the deployment profile.
Max allowed length is 1500 chars.
Supports: $select, $top, $skip, $orderBy.
$Search and $filter are not supported.
  - `[DeviceNameTemplate <String>]`: The template used to name the Autopilot device.
This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.
The total length of the text generated by the template can be no more than 15 characters.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
  - `[DeviceType <WindowsAutopilotDeviceType?>]`: windowsAutopilotDeviceType
  - `[DisplayName <String>]`: The display name of the deployment profile.
Max allowed length is 200 chars.
Returned by default.
Supports: $select, $top, $skip, $orderby.
$Search and $filter are not supported.
  - `[EnableWhiteGlove <Boolean?>]`: Indicates whether the user is allowed to use Windows Autopilot for pre-provisioned deployment mode during Out of Box experience (OOBE).
When TRUE, indicates that Windows Autopilot for pre-provisioned deployment mode is allowed.
When false, Windows Autopilot for pre-provisioned deployment mode is not allowed.
The default is FALSE.
Read-Only.
Starting from May 2024 this property will no longer be supported and will be marked as deprecated.
Use preprovisioningAllowed instead.
  - `[EnrollmentStatusScreenSettings <IMicrosoftGraphWindowsEnrollmentStatusScreenSettings>]`: Enrollment status screen setting
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AllowDeviceUseBeforeProfileAndAppInstallComplete <Boolean?>]`: Allow or block user to use device before profile and app installation complete
    - `[AllowDeviceUseOnInstallFailure <Boolean?>]`: Allow the user to continue using the device on installation failure
    - `[AllowLogCollectionOnInstallFailure <Boolean?>]`: Allow or block log collection on installation failure
    - `[BlockDeviceSetupRetryByUser <Boolean?>]`: Allow the user to retry the setup on installation failure
    - `[CustomErrorMessage <String>]`: Set custom error message to show upon installation failure
    - `[HideInstallationProgress <Boolean?>]`: Show or hide installation progress to user
    - `[InstallProgressTimeoutInMinutes <Int32?>]`: Set installation progress timeout in minutes
  - `[ExtractHardwareHash <Boolean?>]`: Indicates whether the profile supports the extraction of hardware hash values and registration of the device into Windows Autopilot.
When TRUE, indicates if hardware extraction and Windows Autopilot registration will happen on the next successful check-in.
When FALSE, hardware hash extraction and Windows Autopilot registration will not happen.
Default value is FALSE.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
Read-Only.
Starting from May 2024 this property will no longer be supported and will be marked as deprecated.
Use hardwareHashExtractionEnabled instead.
  - `[HardwareHashExtractionEnabled <Boolean?>]`: Indicates whether the profile supports the extraction of hardware hash values and registration of the device into Windows Autopilot.
When TRUE, indicates if hardware extraction and Windows Autopilot registration will happen on the next successful check-in.
When FALSE, hardware hash extraction and Windows Autopilot registration will not happen.
Default value is FALSE.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
  - `[Language <String>]`: The language code to be used when configuring the device.
E.g.
en-US.
The default value is os-default.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
Read-Only.
Starting from May 2024 this property will no longer be supported and will be marked as deprecated.
Use locale instead.
  - `[LastModifiedDateTime <DateTime?>]`: The date and time of when the deployment profile was last modified.
The value cannot be updated manually and is automatically populated when any changes are made to the profile.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported Read-Only.
  - `[Locale <String>]`: The locale (language) to be used when configuring the device.
E.g.
en-US.
The default value is os-default.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
  - `[ManagementServiceAppId <String>]`: The Entra management service App ID which gets used during client device-based enrollment discovery.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
  - `[OutOfBoxExperienceSetting <IMicrosoftGraphOutOfBoxExperienceSetting>]`: The Windows Autopilot Deployment Profile settings used by the device for the out-of-box experience.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DeviceUsageType <WindowsDeviceUsageType?>]`: windowsDeviceUsageType
    - `[EscapeLinkHidden <Boolean?>]`: When TRUE, the link that allows user to start over with a different account on company sign-in is hidden.
When false, the link that allows user to start over with a different account on company sign-in is available.
Default value is FALSE.
    - `[EulaHidden <Boolean?>]`: When TRUE, EULA is hidden to the end user during OOBE.
When FALSE, EULA is shown to the end user during OOBE.
Default value is FALSE.
    - `[KeyboardSelectionPageSkipped <Boolean?>]`: When TRUE, the keyboard selection page is hidden to the end user during OOBE if Language and Region are set.
When FALSE, the keyboard selection page is skipped during OOBE.
    - `[PrivacySettingsHidden <Boolean?>]`: When TRUE, privacy settings is hidden to the end user during OOBE.
When FALSE, privacy settings is shown to the end user during OOBE.
Default value is FALSE.
    - `[UserType <WindowsUserType?>]`: windowsUserType
  - `[OutOfBoxExperienceSettings <IMicrosoftGraphOutOfBoxExperienceSettings>]`: The Windows Autopilot Deployment Profile settings used by the Autopilot device for out-of-box experience.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
Read-Only.
Starting from May 2024 this property will no longer be supported and will be marked as deprecated.
Use outOfBoxExperienceSetting instead.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DeviceUsageType <WindowsDeviceUsageType?>]`: windowsDeviceUsageType
    - `[HideEscapeLink <Boolean?>]`: If set to true, then the user can't start over with different account, on company sign-in
    - `[HideEula <Boolean?>]`: Show or hide EULA to user
    - `[HidePrivacySettings <Boolean?>]`: Show or hide privacy settings to user
    - `[SkipKeyboardSelectionPage <Boolean?>]`: If set, then skip the keyboard selection page if Language and Region are set
    - `[UserType <WindowsUserType?>]`: windowsUserType
  - `[PreprovisioningAllowed <Boolean?>]`: Indicates whether the user is allowed to use Windows Autopilot for pre-provisioned deployment mode during Out of Box experience (OOBE).
When TRUE, indicates that Windows Autopilot for pre-provisioned deployment mode for OOBE is allowed to be used.
When false, Windows Autopilot for pre-provisioned deployment mode for OOBE is not allowed.
The default is FALSE.
  - `[RoleScopeTagIds <String- `[]`>]`: List of role scope tags for the deployment profile.

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

INTENDEDDEPLOYMENTPROFILE `<IMicrosoftGraphWindowsAutopilotDeploymentProfile>`: Windows Autopilot Deployment Profile
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AssignedDevices <IMicrosoftGraphWindowsAutopilotDeviceIdentity- `[]`>]`: The list of assigned devices for the profile.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AddressableUserName <String>]`: Addressable user name.
    - `[AzureActiveDirectoryDeviceId <String>]`: AAD Device ID - to be deprecated
    - `[AzureAdDeviceId <String>]`: AAD Device ID
    - `[DeploymentProfile <IMicrosoftGraphWindowsAutopilotDeploymentProfile>]`: Windows Autopilot Deployment Profile
    - `[DeploymentProfileAssignedDateTime <DateTime?>]`: Profile set time of the Windows autopilot device.
    - `[DeploymentProfileAssignmentDetailedStatus <WindowsAutopilotProfileAssignmentDetailedStatus?>]`: windowsAutopilotProfileAssignmentDetailedStatus
    - `[DeploymentProfileAssignmentStatus <WindowsAutopilotProfileAssignmentStatus?>]`: windowsAutopilotProfileAssignmentStatus
    - `[DeviceAccountPassword <String>]`: Surface Hub Device Account Password
    - `[DeviceAccountUpn <String>]`: Surface Hub Device Account Upn
    - `[DeviceFriendlyName <String>]`: Surface Hub Device Friendly Name
    - `[DisplayName <String>]`: Display Name
    - `[EnrollmentState <EnrollmentState?>]`: enrollmentState
    - `[GroupTag <String>]`: Group Tag of the Windows autopilot device.
    - `[IntendedDeploymentProfile <IMicrosoftGraphWindowsAutopilotDeploymentProfile>]`: Windows Autopilot Deployment Profile
    - `[LastContactedDateTime <DateTime?>]`: Intune Last Contacted Date Time of the Windows autopilot device.
    - `[ManagedDeviceId <String>]`: Managed Device ID
    - `[Manufacturer <String>]`: Oem manufacturer of the Windows autopilot device.
    - `[Model <String>]`: Model name of the Windows autopilot device.
    - `[ProductKey <String>]`: Product Key of the Windows autopilot device.
    - `[PurchaseOrderIdentifier <String>]`: Purchase Order Identifier of the Windows autopilot device.
    - `[RemediationState <WindowsAutopilotDeviceRemediationState?>]`: Device remediation status, indicating whether or not hardware has been changed for an Autopilot-registered device.
    - `[RemediationStateLastModifiedDateTime <DateTime?>]`: RemediationState set time of Autopilot device.
    - `[ResourceName <String>]`: Resource Name.
    - `[SerialNumber <String>]`: Serial number of the Windows autopilot device.
    - `[SkuNumber <String>]`: SKU Number
    - `[SystemFamily <String>]`: System Family
    - `[UserPrincipalName <String>]`: User Principal Name.
    - `[UserlessEnrollmentStatus <WindowsAutopilotUserlessEnrollmentStatus?>]`: Userless enrollment block status, indicating whether the next device enrollment will be blocked.
  - `[Assignments <IMicrosoftGraphWindowsAutopilotDeploymentProfileAssignment- `[]`>]`: The list of group assignments for the profile.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Source <DeviceAndAppManagementAssignmentSource?>]`: Represents source of assignment.
    - `[SourceId <String>]`: Identifier for resource used for deployment to a group
    - `[Target <IMicrosoftGraphDeviceAndAppManagementAssignmentTarget>]`: Base type for assignment targets.
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DeviceAndAppManagementAssignmentFilterId <String>]`: The ID of the filter for the target assignment.
      - `[DeviceAndAppManagementAssignmentFilterType <DeviceAndAppManagementAssignmentFilterType?>]`: Represents type of the assignment filter.
  - `[CreatedDateTime <DateTime?>]`: The date and time of when the deployment profile was created.
The value cannot be modified and is automatically populated when the profile was created.
The timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
Read-Only.
  - `[Description <String>]`: A description of the deployment profile.
Max allowed length is 1500 chars.
Supports: $select, $top, $skip, $orderBy.
$Search and $filter are not supported.
  - `[DeviceNameTemplate <String>]`: The template used to name the Autopilot device.
This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.
The total length of the text generated by the template can be no more than 15 characters.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
  - `[DeviceType <WindowsAutopilotDeviceType?>]`: windowsAutopilotDeviceType
  - `[DisplayName <String>]`: The display name of the deployment profile.
Max allowed length is 200 chars.
Returned by default.
Supports: $select, $top, $skip, $orderby.
$Search and $filter are not supported.
  - `[EnableWhiteGlove <Boolean?>]`: Indicates whether the user is allowed to use Windows Autopilot for pre-provisioned deployment mode during Out of Box experience (OOBE).
When TRUE, indicates that Windows Autopilot for pre-provisioned deployment mode is allowed.
When false, Windows Autopilot for pre-provisioned deployment mode is not allowed.
The default is FALSE.
Read-Only.
Starting from May 2024 this property will no longer be supported and will be marked as deprecated.
Use preprovisioningAllowed instead.
  - `[EnrollmentStatusScreenSettings <IMicrosoftGraphWindowsEnrollmentStatusScreenSettings>]`: Enrollment status screen setting
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AllowDeviceUseBeforeProfileAndAppInstallComplete <Boolean?>]`: Allow or block user to use device before profile and app installation complete
    - `[AllowDeviceUseOnInstallFailure <Boolean?>]`: Allow the user to continue using the device on installation failure
    - `[AllowLogCollectionOnInstallFailure <Boolean?>]`: Allow or block log collection on installation failure
    - `[BlockDeviceSetupRetryByUser <Boolean?>]`: Allow the user to retry the setup on installation failure
    - `[CustomErrorMessage <String>]`: Set custom error message to show upon installation failure
    - `[HideInstallationProgress <Boolean?>]`: Show or hide installation progress to user
    - `[InstallProgressTimeoutInMinutes <Int32?>]`: Set installation progress timeout in minutes
  - `[ExtractHardwareHash <Boolean?>]`: Indicates whether the profile supports the extraction of hardware hash values and registration of the device into Windows Autopilot.
When TRUE, indicates if hardware extraction and Windows Autopilot registration will happen on the next successful check-in.
When FALSE, hardware hash extraction and Windows Autopilot registration will not happen.
Default value is FALSE.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
Read-Only.
Starting from May 2024 this property will no longer be supported and will be marked as deprecated.
Use hardwareHashExtractionEnabled instead.
  - `[HardwareHashExtractionEnabled <Boolean?>]`: Indicates whether the profile supports the extraction of hardware hash values and registration of the device into Windows Autopilot.
When TRUE, indicates if hardware extraction and Windows Autopilot registration will happen on the next successful check-in.
When FALSE, hardware hash extraction and Windows Autopilot registration will not happen.
Default value is FALSE.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
  - `[Language <String>]`: The language code to be used when configuring the device.
E.g.
en-US.
The default value is os-default.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
Read-Only.
Starting from May 2024 this property will no longer be supported and will be marked as deprecated.
Use locale instead.
  - `[LastModifiedDateTime <DateTime?>]`: The date and time of when the deployment profile was last modified.
The value cannot be updated manually and is automatically populated when any changes are made to the profile.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported Read-Only.
  - `[Locale <String>]`: The locale (language) to be used when configuring the device.
E.g.
en-US.
The default value is os-default.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
  - `[ManagementServiceAppId <String>]`: The Entra management service App ID which gets used during client device-based enrollment discovery.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
  - `[OutOfBoxExperienceSetting <IMicrosoftGraphOutOfBoxExperienceSetting>]`: The Windows Autopilot Deployment Profile settings used by the device for the out-of-box experience.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DeviceUsageType <WindowsDeviceUsageType?>]`: windowsDeviceUsageType
    - `[EscapeLinkHidden <Boolean?>]`: When TRUE, the link that allows user to start over with a different account on company sign-in is hidden.
When false, the link that allows user to start over with a different account on company sign-in is available.
Default value is FALSE.
    - `[EulaHidden <Boolean?>]`: When TRUE, EULA is hidden to the end user during OOBE.
When FALSE, EULA is shown to the end user during OOBE.
Default value is FALSE.
    - `[KeyboardSelectionPageSkipped <Boolean?>]`: When TRUE, the keyboard selection page is hidden to the end user during OOBE if Language and Region are set.
When FALSE, the keyboard selection page is skipped during OOBE.
    - `[PrivacySettingsHidden <Boolean?>]`: When TRUE, privacy settings is hidden to the end user during OOBE.
When FALSE, privacy settings is shown to the end user during OOBE.
Default value is FALSE.
    - `[UserType <WindowsUserType?>]`: windowsUserType
  - `[OutOfBoxExperienceSettings <IMicrosoftGraphOutOfBoxExperienceSettings>]`: The Windows Autopilot Deployment Profile settings used by the Autopilot device for out-of-box experience.
Supports: $select, $top, $skip.
$Search, $orderBy and $filter are not supported.
Read-Only.
Starting from May 2024 this property will no longer be supported and will be marked as deprecated.
Use outOfBoxExperienceSetting instead.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DeviceUsageType <WindowsDeviceUsageType?>]`: windowsDeviceUsageType
    - `[HideEscapeLink <Boolean?>]`: If set to true, then the user can't start over with different account, on company sign-in
    - `[HideEula <Boolean?>]`: Show or hide EULA to user
    - `[HidePrivacySettings <Boolean?>]`: Show or hide privacy settings to user
    - `[SkipKeyboardSelectionPage <Boolean?>]`: If set, then skip the keyboard selection page if Language and Region are set
    - `[UserType <WindowsUserType?>]`: windowsUserType
  - `[PreprovisioningAllowed <Boolean?>]`: Indicates whether the user is allowed to use Windows Autopilot for pre-provisioned deployment mode during Out of Box experience (OOBE).
When TRUE, indicates that Windows Autopilot for pre-provisioned deployment mode for OOBE is allowed to be used.
When false, Windows Autopilot for pre-provisioned deployment mode for OOBE is not allowed.
The default is FALSE.
  - `[RoleScopeTagIds <String- `[]`>]`: List of role scope tags for the deployment profile.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.enrollment/new-mgbetadevicemanagementwindowsautopilotdeploymentprofileassigneddevice](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement.enrollment/new-mgbetadevicemanagementwindowsautopilotdeploymentprofileassigneddevice)
























