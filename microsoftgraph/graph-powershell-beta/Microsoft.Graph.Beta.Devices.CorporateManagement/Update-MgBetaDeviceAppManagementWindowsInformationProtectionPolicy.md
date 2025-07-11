---
external help file: Microsoft.Graph.Beta.Devices.CorporateManagement-help.xml
Module Name: Microsoft.Graph.Beta.Devices.CorporateManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.corporatemanagement/update-mgbetadeviceappmanagementwindowsinformationprotectionpolicy
schema: 2.0.0
---

# Update-MgBetaDeviceAppManagementWindowsInformationProtectionPolicy

## SYNOPSIS
Update the navigation property windowsInformationProtectionPolicies in deviceAppManagement

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgDeviceAppManagementWindowsInformationProtectionPolicy](/powershell/module/Microsoft.Graph.Devices.CorporateManagement/Update-MgDeviceAppManagementWindowsInformationProtectionPolicy?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaDeviceAppManagementWindowsInformationProtectionPolicy
 -WindowsInformationProtectionPolicyId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Assignments <IMicrosoftGraphTargetedManagedAppPolicyAssignment[]>]
 [-AzureRightsManagementServicesAllowed] [-CreatedDateTime <DateTime>]
 [-DataRecoveryCertificate <IMicrosoftGraphWindowsInformationProtectionDataRecoveryCertificate>]
 [-DaysWithoutContactBeforeUnenroll <Int32>] [-Description <String>] [-DisplayName <String>]
 [-EnforcementLevel <WindowsInformationProtectionEnforcementLevel>] [-EnterpriseDomain <String>]
 [-EnterpriseIPRanges <IMicrosoftGraphWindowsInformationProtectionIPRangeCollection[]>]
 [-EnterpriseIPRangesAreAuthoritative]
 [-EnterpriseInternalProxyServers <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-EnterpriseNetworkDomainNames <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-EnterpriseProtectedDomainNames <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-EnterpriseProxiedDomains <IMicrosoftGraphWindowsInformationProtectionProxiedDomainCollection[]>]
 [-EnterpriseProxyServers <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-EnterpriseProxyServersAreAuthoritative]
 [-ExemptAppLockerFiles <IMicrosoftGraphWindowsInformationProtectionAppLockerFile[]>]
 [-ExemptApps <IMicrosoftGraphWindowsInformationProtectionApp[]>] [-IconsVisible] [-Id <String>]
 [-IndexingEncryptedStoresOrItemsBlocked] [-IsAssigned] [-LastModifiedDateTime <DateTime>]
 [-MdmEnrollmentUrl <String>] [-MinutesOfInactivityBeforeDeviceLock <Int32>]
 [-NeutralDomainResources <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-NumberOfPastPinsRemembered <Int32>] [-PasswordMaximumAttemptCount <Int32>] [-PinExpirationDays <Int32>]
 [-PinLowercaseLetters <WindowsInformationProtectionPinCharacterRequirements>] [-PinMinimumLength <Int32>]
 [-PinSpecialCharacters <WindowsInformationProtectionPinCharacterRequirements>]
 [-PinUppercaseLetters <WindowsInformationProtectionPinCharacterRequirements>]
 [-ProtectedAppLockerFiles <IMicrosoftGraphWindowsInformationProtectionAppLockerFile[]>]
 [-ProtectedApps <IMicrosoftGraphWindowsInformationProtectionApp[]>] [-ProtectionUnderLockConfigRequired]
 [-RevokeOnMdmHandoffDisabled] [-RevokeOnUnenrollDisabled] [-RightsManagementServicesTemplateId <String>]
 [-RoleScopeTagIds <String[]>]
 [-SmbAutoEncryptedFileExtensions <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-Version <String>] [-WindowsHelloForBusinessBlocked] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaDeviceAppManagementWindowsInformationProtectionPolicy
 -WindowsInformationProtectionPolicyId <String>
 -BodyParameter <IMicrosoftGraphWindowsInformationProtectionPolicy> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaDeviceAppManagementWindowsInformationProtectionPolicy
 -InputObject <IDevicesCorporateManagementIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Assignments <IMicrosoftGraphTargetedManagedAppPolicyAssignment[]>]
 [-AzureRightsManagementServicesAllowed] [-CreatedDateTime <DateTime>]
 [-DataRecoveryCertificate <IMicrosoftGraphWindowsInformationProtectionDataRecoveryCertificate>]
 [-DaysWithoutContactBeforeUnenroll <Int32>] [-Description <String>] [-DisplayName <String>]
 [-EnforcementLevel <WindowsInformationProtectionEnforcementLevel>] [-EnterpriseDomain <String>]
 [-EnterpriseIPRanges <IMicrosoftGraphWindowsInformationProtectionIPRangeCollection[]>]
 [-EnterpriseIPRangesAreAuthoritative]
 [-EnterpriseInternalProxyServers <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-EnterpriseNetworkDomainNames <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-EnterpriseProtectedDomainNames <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-EnterpriseProxiedDomains <IMicrosoftGraphWindowsInformationProtectionProxiedDomainCollection[]>]
 [-EnterpriseProxyServers <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-EnterpriseProxyServersAreAuthoritative]
 [-ExemptAppLockerFiles <IMicrosoftGraphWindowsInformationProtectionAppLockerFile[]>]
 [-ExemptApps <IMicrosoftGraphWindowsInformationProtectionApp[]>] [-IconsVisible] [-Id <String>]
 [-IndexingEncryptedStoresOrItemsBlocked] [-IsAssigned] [-LastModifiedDateTime <DateTime>]
 [-MdmEnrollmentUrl <String>] [-MinutesOfInactivityBeforeDeviceLock <Int32>]
 [-NeutralDomainResources <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-NumberOfPastPinsRemembered <Int32>] [-PasswordMaximumAttemptCount <Int32>] [-PinExpirationDays <Int32>]
 [-PinLowercaseLetters <WindowsInformationProtectionPinCharacterRequirements>] [-PinMinimumLength <Int32>]
 [-PinSpecialCharacters <WindowsInformationProtectionPinCharacterRequirements>]
 [-PinUppercaseLetters <WindowsInformationProtectionPinCharacterRequirements>]
 [-ProtectedAppLockerFiles <IMicrosoftGraphWindowsInformationProtectionAppLockerFile[]>]
 [-ProtectedApps <IMicrosoftGraphWindowsInformationProtectionApp[]>] [-ProtectionUnderLockConfigRequired]
 [-RevokeOnMdmHandoffDisabled] [-RevokeOnUnenrollDisabled] [-RightsManagementServicesTemplateId <String>]
 [-RoleScopeTagIds <String[]>]
 [-SmbAutoEncryptedFileExtensions <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-Version <String>] [-WindowsHelloForBusinessBlocked] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaDeviceAppManagementWindowsInformationProtectionPolicy
 -InputObject <IDevicesCorporateManagementIdentity>
 -BodyParameter <IMicrosoftGraphWindowsInformationProtectionPolicy> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property windowsInformationProtectionPolicies in deviceAppManagement

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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Assignments
Navigation property to list of security groups targeted for policy.
To construct, see NOTES section for ASSIGNMENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphTargetedManagedAppPolicyAssignment[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AzureRightsManagementServicesAllowed
Specifies whether to allow Azure RMS encryption for WIP

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
Policy for Windows information protection without MDM
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionPolicy
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
The date and time the policy was created.

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

### -DataRecoveryCertificate
Windows Information Protection DataRecoveryCertificate
To construct, see NOTES section for DATARECOVERYCERTIFICATE properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionDataRecoveryCertificate
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DaysWithoutContactBeforeUnenroll
Offline interval before app data is wiped (days)

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
The policy's description.

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

### -DisplayName
Policy display name.

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

### -EnforcementLevel
Possible values for WIP Protection enforcement levels

```yaml
Type: WindowsInformationProtectionEnforcementLevel
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnterpriseDomain
Primary enterprise domain

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

### -EnterpriseInternalProxyServers
This is the comma-separated list of internal proxy servers.
For example, '157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59'.
These proxies have been configured by the admin to connect to specific resources on the Internet.
They are considered to be enterprise network locations.
The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies
To construct, see NOTES section for ENTERPRISEINTERNALPROXYSERVERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionResourceCollection[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnterpriseIPRanges
Sets the enterprise IP ranges that define the computers in the enterprise network.
Data that comes from those computers will be considered part of the enterprise and protected.
These locations will be considered a safe destination for enterprise data to be shared to
To construct, see NOTES section for ENTERPRISEIPRANGES properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionIPRangeCollection[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnterpriseIPRangesAreAuthoritative
Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.
Default is false

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnterpriseNetworkDomainNames
This is the list of domains that comprise the boundaries of the enterprise.
Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to
To construct, see NOTES section for ENTERPRISENETWORKDOMAINNAMES properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionResourceCollection[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnterpriseProtectedDomainNames
List of enterprise domains to be protected
To construct, see NOTES section for ENTERPRISEPROTECTEDDOMAINNAMES properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionResourceCollection[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnterpriseProxiedDomains
Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.
Connections to these resources are considered enterprise data.
If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).
A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy
To construct, see NOTES section for ENTERPRISEPROXIEDDOMAINS properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionProxiedDomainCollection[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnterpriseProxyServers
This is a list of proxy servers.
Any server not on this list is considered non-enterprise
To construct, see NOTES section for ENTERPRISEPROXYSERVERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionResourceCollection[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnterpriseProxyServersAreAuthoritative
Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.
Default is false

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExemptAppLockerFiles
Another way to input exempt apps through xml files
To construct, see NOTES section for EXEMPTAPPLOCKERFILES properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionAppLockerFile[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExemptApps
Exempt applications can also access enterprise data, but the data handled by those applications are not protected.
This is because some critical enterprise applications may have compatibility problems with encrypted data.
To construct, see NOTES section for EXEMPTAPPS properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionApp[]
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

### -IconsVisible
Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.
Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
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

### -IndexingEncryptedStoresOrItemsBlocked
This switch is for the Windows Search Indexer, to allow or disallow indexing of items

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
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

### -IsAssigned
Indicates if the policy is deployed to any inclusion groups or not.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedDateTime
Last time the policy was modified.

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

### -MdmEnrollmentUrl
Enrollment url for the MDM

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

### -MinutesOfInactivityBeforeDeviceLock
Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.
Range is an integer X where 0 `<= X `<= 999.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -NeutralDomainResources
List of domain names that can used for work or personal resource
To construct, see NOTES section for NEUTRALDOMAINRESOURCES properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionResourceCollection[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NumberOfPastPinsRemembered
Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.
The largest number you can configure for this policy setting is 50.
The lowest number you can configure for this policy setting is 0.
If this policy is set to 0, then storage of previous PINs is not required.
This node was added in Windows 10, version 1511.
Default is 0.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -PasswordMaximumAttemptCount
The number of authentication failures allowed before the device will be wiped.
A value of 0 disables device wipe functionality.
Range is an integer X where 4 `<= X `<= 16 for desktop and 0 `<= X `<= 999 for mobile devices.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -PinExpirationDays
Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.
The largest number you can configure for this policy setting is 730.
The lowest number you can configure for this policy setting is 0.
If this policy is set to 0, then the user's PIN will never expire.
This node was added in Windows 10, version 1511.
Default is 0.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -PinLowercaseLetters
Pin Character Requirements

```yaml
Type: WindowsInformationProtectionPinCharacterRequirements
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PinMinimumLength
Integer value that sets the minimum number of characters required for the PIN.
Default value is 4.
The lowest number you can configure for this policy setting is 4.
The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.

```yaml
Type: Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -PinSpecialCharacters
Pin Character Requirements

```yaml
Type: WindowsInformationProtectionPinCharacterRequirements
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PinUppercaseLetters
Pin Character Requirements

```yaml
Type: WindowsInformationProtectionPinCharacterRequirements
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProtectedAppLockerFiles
Another way to input protected apps through xml files
To construct, see NOTES section for PROTECTEDAPPLOCKERFILES properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionAppLockerFile[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProtectedApps
Protected applications can access enterprise data and the data handled by those applications are protected with encryption
To construct, see NOTES section for PROTECTEDAPPS properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionApp[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProtectionUnderLockConfigRequired
Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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

### -RevokeOnMdmHandoffDisabled
New property in RS2, pending documentation

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -RevokeOnUnenrollDisabled
This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.
If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.
If the keys are not revoked, there will be no revoked file cleanup subsequently.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -RightsManagementServicesTemplateId
TemplateID GUID to use for RMS encryption.
The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access

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

### -RoleScopeTagIds
List of Scope Tags for this Entity instance.

```yaml
Type: String[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SmbAutoEncryptedFileExtensions
Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary
To construct, see NOTES section for SMBAUTOENCRYPTEDFILEEXTENSIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsInformationProtectionResourceCollection[]
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

### -WindowsHelloForBusinessBlocked
Boolean value that sets Windows Hello for Business as a method for signing into Windows.

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WindowsInformationProtectionPolicyId
The unique identifier of windowsInformationProtectionPolicy

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IDevicesCorporateManagementIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphWindowsInformationProtectionPolicy
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphWindowsInformationProtectionPolicy
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ASSIGNMENTS `<IMicrosoftGraphTargetedManagedAppPolicyAssignment- `[]`>`: Navigation property to list of security groups targeted for policy.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Source <DeviceAndAppManagementAssignmentSource?>]`: Represents source of assignment.
  - `[SourceId <String>]`: Identifier for resource used for deployment to a group
  - `[Target <IMicrosoftGraphDeviceAndAppManagementAssignmentTarget>]`: Base type for assignment targets.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DeviceAndAppManagementAssignmentFilterId <String>]`: The ID of the filter for the target assignment.
    - `[DeviceAndAppManagementAssignmentFilterType <DeviceAndAppManagementAssignmentFilterType?>]`: Represents type of the assignment filter.

BODYPARAMETER `<IMicrosoftGraphWindowsInformationProtectionPolicy>`: Policy for Windows information protection without MDM
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Assignments <IMicrosoftGraphTargetedManagedAppPolicyAssignment- `[]`>]`: Navigation property to list of security groups targeted for policy.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Source <DeviceAndAppManagementAssignmentSource?>]`: Represents source of assignment.
    - `[SourceId <String>]`: Identifier for resource used for deployment to a group
    - `[Target <IMicrosoftGraphDeviceAndAppManagementAssignmentTarget>]`: Base type for assignment targets.
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DeviceAndAppManagementAssignmentFilterId <String>]`: The ID of the filter for the target assignment.
      - `[DeviceAndAppManagementAssignmentFilterType <DeviceAndAppManagementAssignmentFilterType?>]`: Represents type of the assignment filter.
  - `[AzureRightsManagementServicesAllowed <Boolean?>]`: Specifies whether to allow Azure RMS encryption for WIP
  - `[DataRecoveryCertificate <IMicrosoftGraphWindowsInformationProtectionDataRecoveryCertificate>]`: Windows Information Protection DataRecoveryCertificate
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Certificate <Byte- `[]`>]`: Data recovery Certificate
    - `[Description <String>]`: Data recovery Certificate description
    - `[ExpirationDateTime <DateTime?>]`: Data recovery Certificate expiration datetime
    - `[SubjectName <String>]`: Data recovery Certificate subject name
  - `[EnforcementLevel <WindowsInformationProtectionEnforcementLevel?>]`: Possible values for WIP Protection enforcement levels
  - `[EnterpriseDomain <String>]`: Primary enterprise domain
  - `[EnterpriseIPRanges <IMicrosoftGraphWindowsInformationProtectionIPRangeCollection- `[]`>]`: Sets the enterprise IP ranges that define the computers in the enterprise network.
Data that comes from those computers will be considered part of the enterprise and protected.
These locations will be considered a safe destination for enterprise data to be shared to
    - `[DisplayName <String>]`: Display name
    - `[Ranges <IMicrosoftGraphIPRange- `[]`>]`: Collection of ip ranges
  - `[EnterpriseIPRangesAreAuthoritative <Boolean?>]`: Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.
Default is false
  - `[EnterpriseInternalProxyServers <IMicrosoftGraphWindowsInformationProtectionResourceCollection- `[]`>]`: This is the comma-separated list of internal proxy servers.
For example, '157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59'.
These proxies have been configured by the admin to connect to specific resources on the Internet.
They are considered to be enterprise network locations.
The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies
    - `[DisplayName <String>]`: Display name
    - `[Resources <String- `[]`>]`: Collection of resources
  - `[EnterpriseNetworkDomainNames <IMicrosoftGraphWindowsInformationProtectionResourceCollection- `[]`>]`: This is the list of domains that comprise the boundaries of the enterprise.
Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to
  - `[EnterpriseProtectedDomainNames <IMicrosoftGraphWindowsInformationProtectionResourceCollection- `[]`>]`: List of enterprise domains to be protected
  - `[EnterpriseProxiedDomains <IMicrosoftGraphWindowsInformationProtectionProxiedDomainCollection- `[]`>]`: Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.
Connections to these resources are considered enterprise data.
If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).
A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy
    - `[DisplayName <String>]`: Display name
    - `[ProxiedDomains <IMicrosoftGraphProxiedDomain- `[]`>]`: Collection of proxied domains
      - `[IPAddressOrFqdn <String>]`: The IP address or FQDN
      - `[Proxy <String>]`: Proxy IP or FQDN
  - `[EnterpriseProxyServers <IMicrosoftGraphWindowsInformationProtectionResourceCollection- `[]`>]`: This is a list of proxy servers.
Any server not on this list is considered non-enterprise
  - `[EnterpriseProxyServersAreAuthoritative <Boolean?>]`: Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.
Default is false
  - `[ExemptAppLockerFiles <IMicrosoftGraphWindowsInformationProtectionAppLockerFile- `[]`>]`: Another way to input exempt apps through xml files
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: The friendly name
    - `[File <Byte- `[]`>]`: File as a byte array
    - `[FileHash <String>]`: SHA256 hash of the file
    - `[Version <String>]`: Version of the entity.
  - `[ExemptApps <IMicrosoftGraphWindowsInformationProtectionApp- `[]`>]`: Exempt applications can also access enterprise data, but the data handled by those applications are not protected.
This is because some critical enterprise applications may have compatibility problems with encrypted data.
    - `[Denied <Boolean?>]`: If true, app is denied protection or exemption.
    - `[Description <String>]`: The app's description.
    - `[DisplayName <String>]`: App display name.
    - `[ProductName <String>]`: The product name.
    - `[PublisherName <String>]`: The publisher name
  - `[IconsVisible <Boolean?>]`: Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu.
Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app
  - `[IndexingEncryptedStoresOrItemsBlocked <Boolean?>]`: This switch is for the Windows Search Indexer, to allow or disallow indexing of items
  - `[IsAssigned <Boolean?>]`: Indicates if the policy is deployed to any inclusion groups or not.
  - `[NeutralDomainResources <IMicrosoftGraphWindowsInformationProtectionResourceCollection- `[]`>]`: List of domain names that can used for work or personal resource
  - `[ProtectedAppLockerFiles <IMicrosoftGraphWindowsInformationProtectionAppLockerFile- `[]`>]`: Another way to input protected apps through xml files
  - `[ProtectedApps <IMicrosoftGraphWindowsInformationProtectionApp- `[]`>]`: Protected applications can access enterprise data and the data handled by those applications are protected with encryption
  - `[ProtectionUnderLockConfigRequired <Boolean?>]`: Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured
  - `[RevokeOnUnenrollDisabled <Boolean?>]`: This policy controls whether to revoke the WIP keys when a device unenrolls from the management service.
If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment.
If the keys are not revoked, there will be no revoked file cleanup subsequently.
  - `[RightsManagementServicesTemplateId <String>]`: TemplateID GUID to use for RMS encryption.
The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access
  - `[SmbAutoEncryptedFileExtensions <IMicrosoftGraphWindowsInformationProtectionResourceCollection- `[]`>]`: Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary
  - `[CreatedDateTime <DateTime?>]`: The date and time the policy was created.
  - `[Description <String>]`: The policy's description.
  - `[DisplayName <String>]`: Policy display name.
  - `[LastModifiedDateTime <DateTime?>]`: Last time the policy was modified.
  - `[RoleScopeTagIds <String- `[]`>]`: List of Scope Tags for this Entity instance.
  - `[Version <String>]`: Version of the entity.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DaysWithoutContactBeforeUnenroll <Int32?>]`: Offline interval before app data is wiped (days)
  - `[MdmEnrollmentUrl <String>]`: Enrollment url for the MDM
  - `[MinutesOfInactivityBeforeDeviceLock <Int32?>]`: Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked. 
Range is an integer X where 0 <= X <= 999.
  - `[NumberOfPastPinsRemembered <Int32?>]`: Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused.
The largest number you can configure for this policy setting is 50.
The lowest number you can configure for this policy setting is 0.
If this policy is set to 0, then storage of previous PINs is not required.
This node was added in Windows 10, version 1511.
Default is 0.
  - `[PasswordMaximumAttemptCount <Int32?>]`: The number of authentication failures allowed before the device will be wiped.
A value of 0 disables device wipe functionality.
Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.
  - `[PinExpirationDays <Int32?>]`: Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it.
The largest number you can configure for this policy setting is 730.
The lowest number you can configure for this policy setting is 0.
If this policy is set to 0, then the user's PIN will never expire.
This node was added in Windows 10, version 1511.
Default is 0.
  - `[PinLowercaseLetters <WindowsInformationProtectionPinCharacterRequirements?>]`: Pin Character Requirements
  - `[PinMinimumLength <Int32?>]`: Integer value that sets the minimum number of characters required for the PIN.
Default value is 4.
The lowest number you can configure for this policy setting is 4.
The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.
  - `[PinSpecialCharacters <WindowsInformationProtectionPinCharacterRequirements?>]`: Pin Character Requirements
  - `[PinUppercaseLetters <WindowsInformationProtectionPinCharacterRequirements?>]`: Pin Character Requirements
  - `[RevokeOnMdmHandoffDisabled <Boolean?>]`: New property in RS2, pending documentation
  - `[WindowsHelloForBusinessBlocked <Boolean?>]`: Boolean value that sets Windows Hello for Business as a method for signing into Windows.

DATARECOVERYCERTIFICATE `<IMicrosoftGraphWindowsInformationProtectionDataRecoveryCertificate>`: Windows Information Protection DataRecoveryCertificate
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Certificate <Byte- `[]`>]`: Data recovery Certificate
  - `[Description <String>]`: Data recovery Certificate description
  - `[ExpirationDateTime <DateTime?>]`: Data recovery Certificate expiration datetime
  - `[SubjectName <String>]`: Data recovery Certificate subject name

ENTERPRISEINTERNALPROXYSERVERS `<IMicrosoftGraphWindowsInformationProtectionResourceCollection- `[]`>`: This is the comma-separated list of internal proxy servers.
For example, '157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59'.
These proxies have been configured by the admin to connect to specific resources on the Internet.
They are considered to be enterprise network locations.
The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies
  - `[DisplayName <String>]`: Display name
  - `[Resources <String- `[]`>]`: Collection of resources

ENTERPRISEIPRANGES `<IMicrosoftGraphWindowsInformationProtectionIPRangeCollection- `[]`>`: Sets the enterprise IP ranges that define the computers in the enterprise network.
Data that comes from those computers will be considered part of the enterprise and protected.
These locations will be considered a safe destination for enterprise data to be shared to
  - `[DisplayName <String>]`: Display name
  - `[Ranges <IMicrosoftGraphIPRange- `[]`>]`: Collection of ip ranges

ENTERPRISENETWORKDOMAINNAMES `<IMicrosoftGraphWindowsInformationProtectionResourceCollection- `[]`>`: This is the list of domains that comprise the boundaries of the enterprise.
Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to
  - `[DisplayName <String>]`: Display name
  - `[Resources <String- `[]`>]`: Collection of resources

ENTERPRISEPROTECTEDDOMAINNAMES `<IMicrosoftGraphWindowsInformationProtectionResourceCollection- `[]`>`: List of enterprise domains to be protected
  - `[DisplayName <String>]`: Display name
  - `[Resources <String- `[]`>]`: Collection of resources

ENTERPRISEPROXIEDDOMAINS `<IMicrosoftGraphWindowsInformationProtectionProxiedDomainCollection- `[]`>`: Contains a list of Enterprise resource domains hosted in the cloud that need to be protected.
Connections to these resources are considered enterprise data.
If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).
A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy
  - `[DisplayName <String>]`: Display name
  - `[ProxiedDomains <IMicrosoftGraphProxiedDomain- `[]`>]`: Collection of proxied domains
    - `[IPAddressOrFqdn <String>]`: The IP address or FQDN
    - `[Proxy <String>]`: Proxy IP or FQDN

ENTERPRISEPROXYSERVERS `<IMicrosoftGraphWindowsInformationProtectionResourceCollection- `[]`>`: This is a list of proxy servers.
Any server not on this list is considered non-enterprise
  - `[DisplayName <String>]`: Display name
  - `[Resources <String- `[]`>]`: Collection of resources

EXEMPTAPPLOCKERFILES `<IMicrosoftGraphWindowsInformationProtectionAppLockerFile- `[]`>`: Another way to input exempt apps through xml files
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DisplayName <String>]`: The friendly name
  - `[File <Byte- `[]`>]`: File as a byte array
  - `[FileHash <String>]`: SHA256 hash of the file
  - `[Version <String>]`: Version of the entity.

EXEMPTAPPS `<IMicrosoftGraphWindowsInformationProtectionApp- `[]`>`: Exempt applications can also access enterprise data, but the data handled by those applications are not protected.
This is because some critical enterprise applications may have compatibility problems with encrypted data.
  - `[Denied <Boolean?>]`: If true, app is denied protection or exemption.
  - `[Description <String>]`: The app's description.
  - `[DisplayName <String>]`: App display name.
  - `[ProductName <String>]`: The product name.
  - `[PublisherName <String>]`: The publisher name

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

NEUTRALDOMAINRESOURCES `<IMicrosoftGraphWindowsInformationProtectionResourceCollection- `[]`>`: List of domain names that can used for work or personal resource
  - `[DisplayName <String>]`: Display name
  - `[Resources <String- `[]`>]`: Collection of resources

PROTECTEDAPPLOCKERFILES `<IMicrosoftGraphWindowsInformationProtectionAppLockerFile- `[]`>`: Another way to input protected apps through xml files
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DisplayName <String>]`: The friendly name
  - `[File <Byte- `[]`>]`: File as a byte array
  - `[FileHash <String>]`: SHA256 hash of the file
  - `[Version <String>]`: Version of the entity.

PROTECTEDAPPS `<IMicrosoftGraphWindowsInformationProtectionApp- `[]`>`: Protected applications can access enterprise data and the data handled by those applications are protected with encryption
  - `[Denied <Boolean?>]`: If true, app is denied protection or exemption.
  - `[Description <String>]`: The app's description.
  - `[DisplayName <String>]`: App display name.
  - `[ProductName <String>]`: The product name.
  - `[PublisherName <String>]`: The publisher name

SMBAUTOENCRYPTEDFILEEXTENSIONS `<IMicrosoftGraphWindowsInformationProtectionResourceCollection- `[]`>`: Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary
  - `[DisplayName <String>]`: Display name
  - `[Resources <String- `[]`>]`: Collection of resources

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.corporatemanagement/update-mgbetadeviceappmanagementwindowsinformationprotectionpolicy](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.corporatemanagement/update-mgbetadeviceappmanagementwindowsinformationprotectionpolicy)
























