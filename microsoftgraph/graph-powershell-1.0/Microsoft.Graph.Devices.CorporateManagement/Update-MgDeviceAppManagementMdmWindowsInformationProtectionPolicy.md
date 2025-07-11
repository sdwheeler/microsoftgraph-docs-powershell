---
external help file: Microsoft.Graph.Devices.CorporateManagement-help.xml
Module Name: Microsoft.Graph.Devices.CorporateManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.devices.corporatemanagement/update-mgdeviceappmanagementmdmwindowsinformationprotectionpolicy
schema: 2.0.0
---

# Update-MgDeviceAppManagementMdmWindowsInformationProtectionPolicy

## SYNOPSIS
Update the properties of a mdmWindowsInformationProtectionPolicy object.

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaDeviceAppManagementMdmWindowsInformationProtectionPolicy](/powershell/module/Microsoft.Graph.Beta.Devices.CorporateManagement/Update-MgBetaDeviceAppManagementMdmWindowsInformationProtectionPolicy?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgDeviceAppManagementMdmWindowsInformationProtectionPolicy
 -MdmWindowsInformationProtectionPolicyId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Assignments <IMicrosoftGraphTargetedManagedAppPolicyAssignment[]>]
 [-AzureRightsManagementServicesAllowed] [-CreatedDateTime <DateTime>]
 [-DataRecoveryCertificate <IMicrosoftGraphWindowsInformationProtectionDataRecoveryCertificate>]
 [-Description <String>] [-DisplayName <String>]
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
 [-NeutralDomainResources <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-ProtectedAppLockerFiles <IMicrosoftGraphWindowsInformationProtectionAppLockerFile[]>]
 [-ProtectedApps <IMicrosoftGraphWindowsInformationProtectionApp[]>] [-ProtectionUnderLockConfigRequired]
 [-RevokeOnUnenrollDisabled] [-RightsManagementServicesTemplateId <String>]
 [-SmbAutoEncryptedFileExtensions <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-Version <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Update
```
Update-MgDeviceAppManagementMdmWindowsInformationProtectionPolicy
 -MdmWindowsInformationProtectionPolicyId <String> -BodyParameter <Hashtable>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgDeviceAppManagementMdmWindowsInformationProtectionPolicy
 -InputObject <IDevicesCorporateManagementIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Assignments <IMicrosoftGraphTargetedManagedAppPolicyAssignment[]>]
 [-AzureRightsManagementServicesAllowed] [-CreatedDateTime <DateTime>]
 [-DataRecoveryCertificate <IMicrosoftGraphWindowsInformationProtectionDataRecoveryCertificate>]
 [-Description <String>] [-DisplayName <String>]
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
 [-NeutralDomainResources <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-ProtectedAppLockerFiles <IMicrosoftGraphWindowsInformationProtectionAppLockerFile[]>]
 [-ProtectedApps <IMicrosoftGraphWindowsInformationProtectionApp[]>] [-ProtectionUnderLockConfigRequired]
 [-RevokeOnUnenrollDisabled] [-RightsManagementServicesTemplateId <String>]
 [-SmbAutoEncryptedFileExtensions <IMicrosoftGraphWindowsInformationProtectionResourceCollection[]>]
 [-Version <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgDeviceAppManagementMdmWindowsInformationProtectionPolicy
 -InputObject <IDevicesCorporateManagementIdentity> -BodyParameter <Hashtable>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the properties of a mdmWindowsInformationProtectionPolicy object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | DeviceManagementApps.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | DeviceManagementApps.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Devices.CorporateManagement

$params = @{
	"@odata.type" = "#microsoft.graph.mdmWindowsInformationProtectionPolicy"
	displayName = "Display Name value"
	description = "Description value"
	version = "Version value"
	enforcementLevel = "encryptAndAuditOnly"
	enterpriseDomain = "Enterprise Domain value"
	enterpriseProtectedDomainNames = @(
		@{
			"@odata.type" = "microsoft.graph.windowsInformationProtectionResourceCollection"
			displayName = "Display Name value"
			resources = @(
			"Resources value"
		)
	}
)
protectionUnderLockConfigRequired = $true
dataRecoveryCertificate = @{
	"@odata.type" = "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
	subjectName = "Subject Name value"
	description = "Description value"
	expirationDateTime = [System.DateTime]::Parse("2016-12-31T23:57:57.2481234-08:00")
	certificate = [System.Text.Encoding]::ASCII.GetBytes("Y2VydGlmaWNhdGU=")
}
revokeOnUnenrollDisabled = $true
rightsManagementServicesTemplateId = "abf7b16f-b16f-abf7-6fb1-f7ab6fb1f7ab"
azureRightsManagementServicesAllowed = $true
iconsVisible = $true
protectedApps = @(
	@{
		"@odata.type" = "microsoft.graph.windowsInformationProtectionStoreApp"
		displayName = "Display Name value"
		description = "Description value"
		publisherName = "Publisher Name value"
		productName = "Product Name value"
		denied = $true
	}
)
exemptApps = @(
	@{
		"@odata.type" = "microsoft.graph.windowsInformationProtectionStoreApp"
		displayName = "Display Name value"
		description = "Description value"
		publisherName = "Publisher Name value"
		productName = "Product Name value"
		denied = $true
	}
)
enterpriseNetworkDomainNames = @(
	@{
		"@odata.type" = "microsoft.graph.windowsInformationProtectionResourceCollection"
		displayName = "Display Name value"
		resources = @(
		"Resources value"
	)
}
)
enterpriseProxiedDomains = @(
@{
	"@odata.type" = "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
	displayName = "Display Name value"
	proxiedDomains = @(
		@{
			"@odata.type" = "microsoft.graph.proxiedDomain"
			ipAddressOrFQDN = "Ip Address Or FQDN value"
			proxy = "Proxy value"
		}
	)
}
)
enterpriseIPRanges = @(
@{
	"@odata.type" = "microsoft.graph.windowsInformationProtectionIPRangeCollection"
	displayName = "Display Name value"
	ranges = @(
		@{
			"@odata.type" = "microsoft.graph.iPv6Range"
			lowerAddress = "Lower Address value"
			upperAddress = "Upper Address value"
		}
	)
}
)
enterpriseIPRangesAreAuthoritative = $true
enterpriseProxyServers = @(
@{
	"@odata.type" = "microsoft.graph.windowsInformationProtectionResourceCollection"
	displayName = "Display Name value"
	resources = @(
	"Resources value"
)
}
)
enterpriseInternalProxyServers = @(
@{
"@odata.type" = "microsoft.graph.windowsInformationProtectionResourceCollection"
displayName = "Display Name value"
resources = @(
"Resources value"
)
}
)
enterpriseProxyServersAreAuthoritative = $true
neutralDomainResources = @(
@{
"@odata.type" = "microsoft.graph.windowsInformationProtectionResourceCollection"
displayName = "Display Name value"
resources = @(
"Resources value"
)
}
)
indexingEncryptedStoresOrItemsBlocked = $true
smbAutoEncryptedFileExtensions = @(
@{
"@odata.type" = "microsoft.graph.windowsInformationProtectionResourceCollection"
displayName = "Display Name value"
resources = @(
"Resources value"
)
}
)
isAssigned = $true
}

Update-MgDeviceAppManagementMdmWindowsInformationProtectionPolicy -MdmWindowsInformationProtectionPolicyId $mdmWindowsInformationProtectionPolicyId -BodyParameter $params

```
This example shows how to use the Update-MgDeviceAppManagementMdmWindowsInformationProtectionPolicy Cmdlet.


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
Policy for Windows information protection with MDM

```yaml
Type: Hashtable
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

### -MdmWindowsInformationProtectionPolicyId
The unique identifier of mdmWindowsInformationProtectionPolicy

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IDevicesCorporateManagementIdentity
### System.Collections.Hashtable
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphMdmWindowsInformationProtectionPolicy
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ASSIGNMENTS `<IMicrosoftGraphTargetedManagedAppPolicyAssignment- `[]`>`: Navigation property to list of security groups targeted for policy.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Target <IMicrosoftGraphDeviceAndAppManagementAssignmentTarget>]`: Base type for assignment targets.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.

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

[https://learn.microsoft.com/powershell/module/microsoft.graph.devices.corporatemanagement/update-mgdeviceappmanagementmdmwindowsinformationprotectionpolicy](https://learn.microsoft.com/powershell/module/microsoft.graph.devices.corporatemanagement/update-mgdeviceappmanagementmdmwindowsinformationprotectionpolicy)

[https://learn.microsoft.com/graph/api/intune-mam-mdmwindowsinformationprotectionpolicy-update?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/intune-mam-mdmwindowsinformationprotectionpolicy-update?view=graph-rest-1.0)























