---
external help file: Microsoft.Graph.Beta.Identity.DirectoryManagement-help.xml
Module Name: Microsoft.Graph.Beta.Identity.DirectoryManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/new-mgbetadevice
schema: 2.0.0
ms.subservice: entra-directory-management
---

# New-MgBetaDevice

## SYNOPSIS
Create a new device.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgDevice](/powershell/module/Microsoft.Graph.Identity.DirectoryManagement/New-MgDevice?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaDevice [-ResponseHeadersVariable <String>] [-AccountEnabled] [-AdditionalProperties <Hashtable>]
 [-AlternativeNames <String[]>] [-AlternativeSecurityIds <IMicrosoftGraphAlternativeSecurityId[]>]
 [-ApproximateLastSignInDateTime <DateTime>] [-Commands <IMicrosoftGraphCommand[]>]
 [-ComplianceExpirationDateTime <DateTime>] [-DeletedDateTime <DateTime>] [-DeviceCategory <String>]
 [-DeviceId <String>] [-DeviceMetadata <String>] [-DeviceOwnership <String>]
 [-DeviceTemplate <IMicrosoftGraphDeviceTemplate[]>] [-DeviceVersion <Int32>] [-DisplayName <String>]
 [-DomainName <String>] [-EnrollmentProfileName <String>] [-EnrollmentType <String>]
 [-ExtensionAttributes <IMicrosoftGraphOnPremisesExtensionAttributes>]
 [-Extensions <IMicrosoftGraphExtension[]>] [-Hostnames <String[]>] [-Id <String>] [-IsCompliant] [-IsManaged]
 [-IsManagementRestricted] [-IsRooted] [-Kind <String>] [-ManagementType <String>] [-Manufacturer <String>]
 [-MdmAppId <String>] [-MemberOf <IMicrosoftGraphDirectoryObject[]>] [-Model <String>] [-Name <String>]
 [-OnPremisesLastSyncDateTime <DateTime>] [-OnPremisesSecurityIdentifier <String>] [-OnPremisesSyncEnabled]
 [-OperatingSystem <String>] [-OperatingSystemVersion <String>] [-PhysicalIds <String[]>] [-Platform <String>]
 [-ProfileType <String>] [-RegisteredOwners <IMicrosoftGraphDirectoryObject[]>]
 [-RegisteredUsers <IMicrosoftGraphDirectoryObject[]>] [-RegistrationDateTime <DateTime>] [-Status <String>]
 [-SystemLabels <String[]>] [-TransitiveMemberOf <IMicrosoftGraphDirectoryObject[]>] [-TrustType <String>]
 [-UsageRights <IMicrosoftGraphUsageRight[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaDevice -BodyParameter <IMicrosoftGraphDevice> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new device.

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	accountEnabled = $true
	alternativeSecurityIds = @(
		@{
			type = 99
			identityProvider = "identityProvider-value"
			key = [System.Text.Encoding]::ASCII.GetBytes("base64Y3YxN2E1MWFlYw==")
		}
	)
	approximateLastSignInDateTime = [System.DateTime]::Parse("2016-10-19T10:37:00Z")
	deviceId = "deviceId-value"
	deviceMetadata = "deviceMetadata-value"
	deviceVersion = 99
}

New-MgBetaDevice -BodyParameter $params

```
This example shows how to use the New-MgBetaDevice Cmdlet.


## PARAMETERS

### -AccountEnabled
true if the account is enabled; otherwise, false.
Default is true.
Supports $filter (eq, ne, not, in).
Only callers with at least the Cloud Device Administrator role can set this property.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

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

### -AlternativeNames
List of alternative names for the device.

```yaml
Type: String[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AlternativeSecurityIds
For internal use only.
Not nullable.
Supports $filter (eq, not, ge, le).
To construct, see NOTES section for ALTERNATIVESECURITYIDS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAlternativeSecurityId[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApproximateLastSignInDateTime
The timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
Supports $filter (eq, ne, not, ge, le, and eq on null values) and $orderby.

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

### -BodyParameter
device
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphDevice
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Commands
Set of commands sent to this device.
To construct, see NOTES section for COMMANDS properties and create a hash table.

```yaml
Type: IMicrosoftGraphCommand[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ComplianceExpirationDateTime
The timestamp when the device is no longer deemed compliant.
The timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.

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

### -DeletedDateTime
Date and time when this object was deleted.
Always null when the object hasn't been deleted.

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

### -DeviceCategory
User-defined property set by Intune to automatically add devices to groups and simplify managing devices.

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

### -DeviceId
Unique identifier set by Azure Device Registration Service at the time of registration.
This ID is an alternate key that can be used to reference the device object.
Also supports $filter (eq, ne, not, startsWith).

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

### -DeviceMetadata
For internal use only.
Set to null.

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

### -DeviceOwnership
Ownership of the device.
Intune sets this property.
Possible values are: unknown, company, personal.

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

### -DeviceTemplate
Device template used to instantiate this device.
Nullable.
Read-only.
To construct, see NOTES section for DEVICETEMPLATE properties and create a hash table.

```yaml
Type: IMicrosoftGraphDeviceTemplate[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceVersion
For internal use only.

```yaml
Type: Int32
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
The display name for the device.
Maximum length is 256 characters.
Required.
Supports $filter (eq, ne, not, ge, le, in, startsWith, and eq on null values), $search, and $orderby.

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

### -DomainName
The on-premises domain name of Microsoft Entra hybrid joined devices.
Intune sets this property.

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

### -EnrollmentProfileName
Enrollment profile applied to the device.
For example, Apple Device Enrollment Profile, Device enrollment - Corporate device identifiers, or Windows Autopilot profile name.
Intune sets this property.

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

### -EnrollmentType
Enrollment type of the device.
Intune sets this property.
Possible values are: unknown, userEnrollment, deviceEnrollmentManager, appleBulkWithUser, appleBulkWithoutUser, windowsAzureADJoin, windowsBulkUserless, windowsAutoEnrollment, windowsBulkAzureDomainJoin, windowsCoManagement, windowsAzureADJoinUsingDeviceAuth,appleUserEnrollment, appleUserEnrollmentWithServiceAccount.
NOTE: This property might return other values apart from those listed.

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

### -ExtensionAttributes
onPremisesExtensionAttributes
To construct, see NOTES section for EXTENSIONATTRIBUTES properties and create a hash table.

```yaml
Type: IMicrosoftGraphOnPremisesExtensionAttributes
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Extensions
The collection of open extensions defined for the device.
Read-only.
Nullable.
To construct, see NOTES section for EXTENSIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphExtension[]
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

### -Hostnames
List of host names for the device.

```yaml
Type: String[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
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

### -IsCompliant
true if the device complies with Mobile Device Management (MDM) policies; otherwise, false.
Read-only.
This can only be updated by Intune for any device OS type or by an approved MDM app for Windows OS devices.
Supports $filter (eq, ne, not).

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsManaged
true if the device is managed by a Mobile Device Management (MDM) app; otherwise, false.
This can only be updated by Intune for any device OS type or by an approved MDM app for Windows OS devices.
Supports $filter (eq, ne, not).

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsManagementRestricted
Indicates whether the device is a member of a restricted management administrative unit.
The default value is false.
Read-only.
To manage a device that's a member of a restricted management administrative unit, the administrator or calling app must be assigned a Microsoft Entra role at the scope of the restricted management administrative unit.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsRooted
true if the device is rooted or jail-broken.
This property can only be updated by Intune.

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Kind
Form factor of the device.
Only returned if the user signs in with a Microsoft account as part of Project Rome.

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

### -ManagementType
Management channel of the device.
Intune sets this property.
Possible values are: eas, mdm, easMdm, intuneClient, easIntuneClient, configurationManagerClient, configurationManagerClientMdm, configurationManagerClientMdmEas, unknown, jamf, googleCloudDevicePolicyController.

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

### -Manufacturer
Manufacturer of the device.
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

### -MdmAppId
Application identifier used to register device into MDM.
Read-only.
Supports $filter (eq, ne, not, startsWith).

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

### -MemberOf
Groups and administrative units that this device is a member of.
Read-only.
Nullable.
Supports $expand.
To construct, see NOTES section for MEMBEROF properties and create a hash table.

```yaml
Type: IMicrosoftGraphDirectoryObject[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Model
Model of the device.
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

### -Name
Friendly name of the device.
Only returned if user signs in with a Microsoft account as part of Project Rome.

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

### -OnPremisesLastSyncDateTime
The last time at which the object was synced with the on-premises directory.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z Read-only.
Supports $filter (eq, ne, not, ge, le, in).

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

### -OnPremisesSecurityIdentifier
The on-premises security identifier (SID) for the user who was synchronized from on-premises to the cloud.
Read-only.
Returned only on $select.
Supports $filter (eq).

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

### -OnPremisesSyncEnabled
true if this object is synced from an on-premises directory; false if this object was originally synced from an on-premises directory but is no longer synced; null if this object has never been synced from an on-premises directory (default).
Read-only.
Supports $filter (eq, ne, not, in, and eq on null values).

```yaml
Type: SwitchParameter
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -OperatingSystem
The type of operating system on the device.
Required.
Supports $filter (eq, ne, not, ge, le, startsWith, and eq on null values).

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

### -OperatingSystemVersion
Operating system version of the device.
Required.
Supports $filter (eq, ne, not, ge, le, startsWith, and eq on null values).

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

### -PhysicalIds
For internal use only.
Not nullable.
Supports $filter (eq, not, ge, le, startsWith, /$count eq 0, /$count ne 0.

```yaml
Type: String[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Platform
Platform of device.
Only returned if the user signs in with a Microsoft account as part of Project Rome.

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

### -ProfileType
The profile type of the device.
Possible values: RegisteredDevice (default), SecureVM, Printer, Shared, IoT.

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

### -RegisteredOwners
The user that cloud joined the device or registered their personal device.
The registered owner is set at the time of registration.
Read-only.
Nullable.
Supports $expand.
To construct, see NOTES section for REGISTEREDOWNERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphDirectoryObject[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RegisteredUsers
Collection of registered users of the device.
For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.
Read-only.
Nullable.
Supports $expand.
To construct, see NOTES section for REGISTEREDUSERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphDirectoryObject[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RegistrationDateTime
Date and time of when the device was registered.
The timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.

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

### -Status
Device is online or offline.
Only returned if user signs in with a Microsoft account as part of Project Rome.

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

### -SystemLabels
List of labels applied to the device by the system.
Supports $filter (/$count eq 0, /$count ne 0).

```yaml
Type: String[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TransitiveMemberOf
Groups and administrative units that this device is a member of.
This operation is transitive.
Supports $expand.
To construct, see NOTES section for TRANSITIVEMEMBEROF properties and create a hash table.

```yaml
Type: IMicrosoftGraphDirectoryObject[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TrustType
Type of trust for the joined device.
Read-only.
Possible values: Workplace (indicates bring your own personal devices), AzureAd (Cloud only joined devices), ServerAd (on-premises domain joined devices joined to Microsoft Entra ID).
For more information, see Introduction to device management in Microsoft Entra ID.
Supports $filter (eq, ne, not, in).

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

### -UsageRights
Represents the usage rights a device has been granted.
To construct, see NOTES section for USAGERIGHTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphUsageRight[]
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphDevice
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphDevice
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ALTERNATIVESECURITYIDS `<IMicrosoftGraphAlternativeSecurityId- `[]`>`: For internal use only.
Not nullable.
Supports $filter (eq, not, ge, le).
  - `[IdentityProvider <String>]`: For internal use only.
  - `[Key <Byte- `[]`>]`: For internal use only.
  - `[Type <Int32?>]`: For internal use only.

BODYPARAMETER `<IMicrosoftGraphDevice>`: device
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AccountEnabled <Boolean?>]`: true if the account is enabled; otherwise, false.
Default is true. 
Supports $filter (eq, ne, not, in).
Only callers with at least the Cloud Device Administrator role can set this property.
  - `[AlternativeNames <String- `[]`>]`: List of alternative names for the device.
  - `[AlternativeSecurityIds <IMicrosoftGraphAlternativeSecurityId- `[]`>]`: For internal use only.
Not nullable.
Supports $filter (eq, not, ge, le).
    - `[IdentityProvider <String>]`: For internal use only.
    - `[Key <Byte- `[]`>]`: For internal use only.
    - `[Type <Int32?>]`: For internal use only.
  - `[ApproximateLastSignInDateTime <DateTime?>]`: The timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
Supports $filter (eq, ne, not, ge, le, and eq on null values) and $orderby.
  - `[Commands <IMicrosoftGraphCommand- `[]`>]`: Set of commands sent to this device.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AppServiceName <String>]`: 
    - `[Error <String>]`: 
    - `[PackageFamilyName <String>]`: 
    - `[Payload <IMicrosoftGraphPayloadRequest>]`: payloadRequest
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[PermissionTicket <String>]`: 
    - `[PostBackUri <String>]`: 
    - `[Responsepayload <IMicrosoftGraphPayloadResponse>]`: payloadResponse
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Status <String>]`: 
    - `[Type <String>]`: 
  - `[ComplianceExpirationDateTime <DateTime?>]`: The timestamp when the device is no longer deemed compliant.
The timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
  - `[DeviceCategory <String>]`: User-defined property set by Intune to automatically add devices to groups and simplify managing devices.
  - `[DeviceId <String>]`: Unique identifier set by Azure Device Registration Service at the time of registration.
This ID is an alternate key that can be used to reference the device object.
Also supports $filter (eq, ne, not, startsWith).
  - `[DeviceMetadata <String>]`: For internal use only.
Set to null.
  - `[DeviceOwnership <String>]`: Ownership of the device.
Intune sets this property.
Possible values are: unknown, company, personal.
  - `[DeviceTemplate <IMicrosoftGraphDeviceTemplate- `[]`>]`: Device template used to instantiate this device.
Nullable.
Read-only.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DeviceAuthority <String>]`: A tenant-defined name for the party that's responsible for provisioning and managing devices on the Microsoft Entra tenant.
For example, Tailwind Traders (the manufacturer) makes security cameras that are installed in customer buildings and managed by Lakeshore Retail (the device authority).
This value is provided to the customer by the device authority (manufacturer or reseller).
    - `[DeviceInstances <IMicrosoftGraphDevice- `[]`>]`: Collection of device objects created based on this template.
    - `[Manufacturer <String>]`: Manufacturer name.
    - `[Model <String>]`: Model name.
    - `[MutualTlsOauthConfigurationId <String>]`: Object ID of the mutualTlsOauthConfiguration.
This value isn't required if self-signed certificates are used.
This value is provided to the customer by the device authority (manufacturer or reseller).
    - `[MutualTlsOauthConfigurationTenantId <String>]`: ID (tenant ID for device authority) of the tenant that contains the mutualTlsOauthConfiguration.
This value isn't required if self-signed certificates are used.
This value is provided to the customer by the device authority (manufacturer or reseller).
    - `[OperatingSystem <String>]`: Operating system type.
Supports $filter (eq, in).
    - `[Owners <IMicrosoftGraphDirectoryObject- `[]`>]`: Collection of directory objects that can manage the device template and the related deviceInstances.
Owners can be represented as service principals, users, or applications.
An owner has full privileges over the device template and doesn't require other administrator roles to create, update, or delete devices from this template, as well as to add or remove template owners.
There can be a maximum of 100 owners on a device template. 
Supports $expand.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  - `[DeviceVersion <Int32?>]`: For internal use only.
  - `[DisplayName <String>]`: The display name for the device.
Maximum length is 256 characters.
Required.
Supports $filter (eq, ne, not, ge, le, in, startsWith, and eq on null values), $search, and $orderby.
  - `[DomainName <String>]`: The on-premises domain name of Microsoft Entra hybrid joined devices.
Intune sets this property.
  - `[EnrollmentProfileName <String>]`: Enrollment profile applied to the device.
For example, Apple Device Enrollment Profile, Device enrollment - Corporate device identifiers, or Windows Autopilot profile name.
Intune sets this property.
  - `[EnrollmentType <String>]`: Enrollment type of the device.
Intune sets this property.
Possible values are: unknown, userEnrollment, deviceEnrollmentManager, appleBulkWithUser, appleBulkWithoutUser, windowsAzureADJoin, windowsBulkUserless, windowsAutoEnrollment, windowsBulkAzureDomainJoin, windowsCoManagement, windowsAzureADJoinUsingDeviceAuth,appleUserEnrollment, appleUserEnrollmentWithServiceAccount.
NOTE: This property might return other values apart from those listed.
  - `[ExtensionAttributes <IMicrosoftGraphOnPremisesExtensionAttributes>]`: onPremisesExtensionAttributes
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ExtensionAttribute1 <String>]`: First customizable extension attribute.
    - `[ExtensionAttribute10 <String>]`: Tenth customizable extension attribute.
    - `[ExtensionAttribute11 <String>]`: Eleventh customizable extension attribute.
    - `[ExtensionAttribute12 <String>]`: Twelfth customizable extension attribute.
    - `[ExtensionAttribute13 <String>]`: Thirteenth customizable extension attribute.
    - `[ExtensionAttribute14 <String>]`: Fourteenth customizable extension attribute.
    - `[ExtensionAttribute15 <String>]`: Fifteenth customizable extension attribute.
    - `[ExtensionAttribute2 <String>]`: Second customizable extension attribute.
    - `[ExtensionAttribute3 <String>]`: Third customizable extension attribute.
    - `[ExtensionAttribute4 <String>]`: Fourth customizable extension attribute.
    - `[ExtensionAttribute5 <String>]`: Fifth customizable extension attribute.
    - `[ExtensionAttribute6 <String>]`: Sixth customizable extension attribute.
    - `[ExtensionAttribute7 <String>]`: Seventh customizable extension attribute.
    - `[ExtensionAttribute8 <String>]`: Eighth customizable extension attribute.
    - `[ExtensionAttribute9 <String>]`: Ninth customizable extension attribute.
  - `[Extensions <IMicrosoftGraphExtension- `[]`>]`: The collection of open extensions defined for the device.
Read-only.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Hostnames <String- `[]`>]`: List of host names for the device.
  - `[IsCompliant <Boolean?>]`: true if the device complies with Mobile Device Management (MDM) policies; otherwise, false.
Read-only.
This can only be updated by Intune for any device OS type or by an approved MDM app for Windows OS devices.
Supports $filter (eq, ne, not).
  - `[IsManaged <Boolean?>]`: true if the device is managed by a Mobile Device Management (MDM) app; otherwise, false.
This can only be updated by Intune for any device OS type or by an approved MDM app for Windows OS devices.
Supports $filter (eq, ne, not).
  - `[IsManagementRestricted <Boolean?>]`: Indicates whether the device is a member of a restricted management administrative unit.
The default value is false.
Read-only. 
To manage a device that's a member of a restricted management administrative unit, the administrator or calling app must be assigned a Microsoft Entra role at the scope of the restricted management administrative unit.
  - `[IsRooted <Boolean?>]`: true if the device is rooted or jail-broken.
This property can only be updated by Intune.
  - `[Kind <String>]`: Form factor of the device.
Only returned if the user signs in with a Microsoft account as part of Project Rome.
  - `[ManagementType <String>]`: Management channel of the device.
Intune sets this property.
Possible values are: eas, mdm, easMdm, intuneClient, easIntuneClient, configurationManagerClient, configurationManagerClientMdm, configurationManagerClientMdmEas, unknown, jamf, googleCloudDevicePolicyController.
  - `[Manufacturer <String>]`: Manufacturer of the device.
Read-only.
  - `[MdmAppId <String>]`: Application identifier used to register device into MDM.
Read-only.
Supports $filter (eq, ne, not, startsWith).
  - `[MemberOf <IMicrosoftGraphDirectoryObject- `[]`>]`: Groups and administrative units that this device is a member of.
Read-only.
Nullable.
Supports $expand.
  - `[Model <String>]`: Model of the device.
Read-only.
  - `[Name <String>]`: Friendly name of the device.
Only returned if user signs in with a Microsoft account as part of Project Rome.
  - `[OnPremisesLastSyncDateTime <DateTime?>]`: The last time at which the object was synced with the on-premises directory.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z Read-only.
Supports $filter (eq, ne, not, ge, le, in).
  - `[OnPremisesSecurityIdentifier <String>]`: The on-premises security identifier (SID) for the user who was synchronized from on-premises to the cloud.
Read-only.
Returned only on $select.
Supports $filter (eq).
  - `[OnPremisesSyncEnabled <Boolean?>]`: true if this object is synced from an on-premises directory; false if this object was originally synced from an on-premises directory but is no longer synced; null if this object has never been synced from an on-premises directory (default).
Read-only.
Supports $filter (eq, ne, not, in, and eq on null values).
  - `[OperatingSystem <String>]`: The type of operating system on the device.
Required.
Supports $filter (eq, ne, not, ge, le, startsWith, and eq on null values).
  - `[OperatingSystemVersion <String>]`: Operating system version of the device.
Required.
Supports $filter (eq, ne, not, ge, le, startsWith, and eq on null values).
  - `[PhysicalIds <String- `[]`>]`: For internal use only.
Not nullable.
Supports $filter (eq, not, ge, le, startsWith, /$count eq 0, /$count ne 0.
  - `[Platform <String>]`: Platform of device.
Only returned if the user signs in with a Microsoft account as part of Project Rome.
  - `[ProfileType <String>]`: The profile type of the device.
Possible values: RegisteredDevice (default), SecureVM, Printer, Shared, IoT.
  - `[RegisteredOwners <IMicrosoftGraphDirectoryObject- `[]`>]`: The user that cloud joined the device or registered their personal device.
The registered owner is set at the time of registration.
Read-only.
Nullable.
Supports $expand.
  - `[RegisteredUsers <IMicrosoftGraphDirectoryObject- `[]`>]`: Collection of registered users of the device.
For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.
Read-only.
Nullable.
Supports $expand.
  - `[RegistrationDateTime <DateTime?>]`: Date and time of when the device was registered.
The timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
  - `[Status <String>]`: Device is online or offline.
Only returned if user signs in with a Microsoft account as part of Project Rome.
  - `[SystemLabels <String- `[]`>]`: List of labels applied to the device by the system.
Supports $filter (/$count eq 0, /$count ne 0).
  - `[TransitiveMemberOf <IMicrosoftGraphDirectoryObject- `[]`>]`: Groups and administrative units that this device is a member of.
This operation is transitive.
Supports $expand.
  - `[TrustType <String>]`: Type of trust for the joined device.
Read-only.
Possible values: Workplace (indicates bring your own personal devices), AzureAd (Cloud only joined devices), ServerAd (on-premises domain joined devices joined to Microsoft Entra ID).
For more information, see Introduction to device management in Microsoft Entra ID.
Supports $filter (eq, ne, not, in).
  - `[UsageRights <IMicrosoftGraphUsageRight- `[]`>]`: Represents the usage rights a device has been granted.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[CatalogId <String>]`: Product id corresponding to the usage right.
    - `[ServiceIdentifier <String>]`: Identifier of the service corresponding to the usage right.
    - `[State <String>]`: usageRightState

COMMANDS `<IMicrosoftGraphCommand- `[]`>`: Set of commands sent to this device.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AppServiceName <String>]`: 
  - `[Error <String>]`: 
  - `[PackageFamilyName <String>]`: 
  - `[Payload <IMicrosoftGraphPayloadRequest>]`: payloadRequest
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[PermissionTicket <String>]`: 
  - `[PostBackUri <String>]`: 
  - `[Responsepayload <IMicrosoftGraphPayloadResponse>]`: payloadResponse
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Status <String>]`: 
  - `[Type <String>]`: 

DEVICETEMPLATE `<IMicrosoftGraphDeviceTemplate- `[]`>`: Device template used to instantiate this device.
Nullable.
Read-only.
  - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DeviceAuthority <String>]`: A tenant-defined name for the party that's responsible for provisioning and managing devices on the Microsoft Entra tenant.
For example, Tailwind Traders (the manufacturer) makes security cameras that are installed in customer buildings and managed by Lakeshore Retail (the device authority).
This value is provided to the customer by the device authority (manufacturer or reseller).
  - `[DeviceInstances <IMicrosoftGraphDevice- `[]`>]`: Collection of device objects created based on this template.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AccountEnabled <Boolean?>]`: true if the account is enabled; otherwise, false.
Default is true. 
Supports $filter (eq, ne, not, in).
Only callers with at least the Cloud Device Administrator role can set this property.
    - `[AlternativeNames <String- `[]`>]`: List of alternative names for the device.
    - `[AlternativeSecurityIds <IMicrosoftGraphAlternativeSecurityId- `[]`>]`: For internal use only.
Not nullable.
Supports $filter (eq, not, ge, le).
      - `[IdentityProvider <String>]`: For internal use only.
      - `[Key <Byte- `[]`>]`: For internal use only.
      - `[Type <Int32?>]`: For internal use only.
    - `[ApproximateLastSignInDateTime <DateTime?>]`: The timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
Supports $filter (eq, ne, not, ge, le, and eq on null values) and $orderby.
    - `[Commands <IMicrosoftGraphCommand- `[]`>]`: Set of commands sent to this device.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AppServiceName <String>]`: 
      - `[Error <String>]`: 
      - `[PackageFamilyName <String>]`: 
      - `[Payload <IMicrosoftGraphPayloadRequest>]`: payloadRequest
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[PermissionTicket <String>]`: 
      - `[PostBackUri <String>]`: 
      - `[Responsepayload <IMicrosoftGraphPayloadResponse>]`: payloadResponse
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Status <String>]`: 
      - `[Type <String>]`: 
    - `[ComplianceExpirationDateTime <DateTime?>]`: The timestamp when the device is no longer deemed compliant.
The timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
    - `[DeviceCategory <String>]`: User-defined property set by Intune to automatically add devices to groups and simplify managing devices.
    - `[DeviceId <String>]`: Unique identifier set by Azure Device Registration Service at the time of registration.
This ID is an alternate key that can be used to reference the device object.
Also supports $filter (eq, ne, not, startsWith).
    - `[DeviceMetadata <String>]`: For internal use only.
Set to null.
    - `[DeviceOwnership <String>]`: Ownership of the device.
Intune sets this property.
Possible values are: unknown, company, personal.
    - `[DeviceTemplate <IMicrosoftGraphDeviceTemplate- `[]`>]`: Device template used to instantiate this device.
Nullable.
Read-only.
    - `[DeviceVersion <Int32?>]`: For internal use only.
    - `[DisplayName <String>]`: The display name for the device.
Maximum length is 256 characters.
Required.
Supports $filter (eq, ne, not, ge, le, in, startsWith, and eq on null values), $search, and $orderby.
    - `[DomainName <String>]`: The on-premises domain name of Microsoft Entra hybrid joined devices.
Intune sets this property.
    - `[EnrollmentProfileName <String>]`: Enrollment profile applied to the device.
For example, Apple Device Enrollment Profile, Device enrollment - Corporate device identifiers, or Windows Autopilot profile name.
Intune sets this property.
    - `[EnrollmentType <String>]`: Enrollment type of the device.
Intune sets this property.
Possible values are: unknown, userEnrollment, deviceEnrollmentManager, appleBulkWithUser, appleBulkWithoutUser, windowsAzureADJoin, windowsBulkUserless, windowsAutoEnrollment, windowsBulkAzureDomainJoin, windowsCoManagement, windowsAzureADJoinUsingDeviceAuth,appleUserEnrollment, appleUserEnrollmentWithServiceAccount.
NOTE: This property might return other values apart from those listed.
    - `[ExtensionAttributes <IMicrosoftGraphOnPremisesExtensionAttributes>]`: onPremisesExtensionAttributes
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ExtensionAttribute1 <String>]`: First customizable extension attribute.
      - `[ExtensionAttribute10 <String>]`: Tenth customizable extension attribute.
      - `[ExtensionAttribute11 <String>]`: Eleventh customizable extension attribute.
      - `[ExtensionAttribute12 <String>]`: Twelfth customizable extension attribute.
      - `[ExtensionAttribute13 <String>]`: Thirteenth customizable extension attribute.
      - `[ExtensionAttribute14 <String>]`: Fourteenth customizable extension attribute.
      - `[ExtensionAttribute15 <String>]`: Fifteenth customizable extension attribute.
      - `[ExtensionAttribute2 <String>]`: Second customizable extension attribute.
      - `[ExtensionAttribute3 <String>]`: Third customizable extension attribute.
      - `[ExtensionAttribute4 <String>]`: Fourth customizable extension attribute.
      - `[ExtensionAttribute5 <String>]`: Fifth customizable extension attribute.
      - `[ExtensionAttribute6 <String>]`: Sixth customizable extension attribute.
      - `[ExtensionAttribute7 <String>]`: Seventh customizable extension attribute.
      - `[ExtensionAttribute8 <String>]`: Eighth customizable extension attribute.
      - `[ExtensionAttribute9 <String>]`: Ninth customizable extension attribute.
    - `[Extensions <IMicrosoftGraphExtension- `[]`>]`: The collection of open extensions defined for the device.
Read-only.
Nullable.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Hostnames <String- `[]`>]`: List of host names for the device.
    - `[IsCompliant <Boolean?>]`: true if the device complies with Mobile Device Management (MDM) policies; otherwise, false.
Read-only.
This can only be updated by Intune for any device OS type or by an approved MDM app for Windows OS devices.
Supports $filter (eq, ne, not).
    - `[IsManaged <Boolean?>]`: true if the device is managed by a Mobile Device Management (MDM) app; otherwise, false.
This can only be updated by Intune for any device OS type or by an approved MDM app for Windows OS devices.
Supports $filter (eq, ne, not).
    - `[IsManagementRestricted <Boolean?>]`: Indicates whether the device is a member of a restricted management administrative unit.
The default value is false.
Read-only. 
To manage a device that's a member of a restricted management administrative unit, the administrator or calling app must be assigned a Microsoft Entra role at the scope of the restricted management administrative unit.
    - `[IsRooted <Boolean?>]`: true if the device is rooted or jail-broken.
This property can only be updated by Intune.
    - `[Kind <String>]`: Form factor of the device.
Only returned if the user signs in with a Microsoft account as part of Project Rome.
    - `[ManagementType <String>]`: Management channel of the device.
Intune sets this property.
Possible values are: eas, mdm, easMdm, intuneClient, easIntuneClient, configurationManagerClient, configurationManagerClientMdm, configurationManagerClientMdmEas, unknown, jamf, googleCloudDevicePolicyController.
    - `[Manufacturer <String>]`: Manufacturer of the device.
Read-only.
    - `[MdmAppId <String>]`: Application identifier used to register device into MDM.
Read-only.
Supports $filter (eq, ne, not, startsWith).
    - `[MemberOf <IMicrosoftGraphDirectoryObject- `[]`>]`: Groups and administrative units that this device is a member of.
Read-only.
Nullable.
Supports $expand.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[Model <String>]`: Model of the device.
Read-only.
    - `[Name <String>]`: Friendly name of the device.
Only returned if user signs in with a Microsoft account as part of Project Rome.
    - `[OnPremisesLastSyncDateTime <DateTime?>]`: The last time at which the object was synced with the on-premises directory.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z Read-only.
Supports $filter (eq, ne, not, ge, le, in).
    - `[OnPremisesSecurityIdentifier <String>]`: The on-premises security identifier (SID) for the user who was synchronized from on-premises to the cloud.
Read-only.
Returned only on $select.
Supports $filter (eq).
    - `[OnPremisesSyncEnabled <Boolean?>]`: true if this object is synced from an on-premises directory; false if this object was originally synced from an on-premises directory but is no longer synced; null if this object has never been synced from an on-premises directory (default).
Read-only.
Supports $filter (eq, ne, not, in, and eq on null values).
    - `[OperatingSystem <String>]`: The type of operating system on the device.
Required.
Supports $filter (eq, ne, not, ge, le, startsWith, and eq on null values).
    - `[OperatingSystemVersion <String>]`: Operating system version of the device.
Required.
Supports $filter (eq, ne, not, ge, le, startsWith, and eq on null values).
    - `[PhysicalIds <String- `[]`>]`: For internal use only.
Not nullable.
Supports $filter (eq, not, ge, le, startsWith, /$count eq 0, /$count ne 0.
    - `[Platform <String>]`: Platform of device.
Only returned if the user signs in with a Microsoft account as part of Project Rome.
    - `[ProfileType <String>]`: The profile type of the device.
Possible values: RegisteredDevice (default), SecureVM, Printer, Shared, IoT.
    - `[RegisteredOwners <IMicrosoftGraphDirectoryObject- `[]`>]`: The user that cloud joined the device or registered their personal device.
The registered owner is set at the time of registration.
Read-only.
Nullable.
Supports $expand.
    - `[RegisteredUsers <IMicrosoftGraphDirectoryObject- `[]`>]`: Collection of registered users of the device.
For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.
Read-only.
Nullable.
Supports $expand.
    - `[RegistrationDateTime <DateTime?>]`: Date and time of when the device was registered.
The timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
    - `[Status <String>]`: Device is online or offline.
Only returned if user signs in with a Microsoft account as part of Project Rome.
    - `[SystemLabels <String- `[]`>]`: List of labels applied to the device by the system.
Supports $filter (/$count eq 0, /$count ne 0).
    - `[TransitiveMemberOf <IMicrosoftGraphDirectoryObject- `[]`>]`: Groups and administrative units that this device is a member of.
This operation is transitive.
Supports $expand.
    - `[TrustType <String>]`: Type of trust for the joined device.
Read-only.
Possible values: Workplace (indicates bring your own personal devices), AzureAd (Cloud only joined devices), ServerAd (on-premises domain joined devices joined to Microsoft Entra ID).
For more information, see Introduction to device management in Microsoft Entra ID.
Supports $filter (eq, ne, not, in).
    - `[UsageRights <IMicrosoftGraphUsageRight- `[]`>]`: Represents the usage rights a device has been granted.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[CatalogId <String>]`: Product id corresponding to the usage right.
      - `[ServiceIdentifier <String>]`: Identifier of the service corresponding to the usage right.
      - `[State <String>]`: usageRightState
  - `[Manufacturer <String>]`: Manufacturer name.
  - `[Model <String>]`: Model name.
  - `[MutualTlsOauthConfigurationId <String>]`: Object ID of the mutualTlsOauthConfiguration.
This value isn't required if self-signed certificates are used.
This value is provided to the customer by the device authority (manufacturer or reseller).
  - `[MutualTlsOauthConfigurationTenantId <String>]`: ID (tenant ID for device authority) of the tenant that contains the mutualTlsOauthConfiguration.
This value isn't required if self-signed certificates are used.
This value is provided to the customer by the device authority (manufacturer or reseller).
  - `[OperatingSystem <String>]`: Operating system type.
Supports $filter (eq, in).
  - `[Owners <IMicrosoftGraphDirectoryObject- `[]`>]`: Collection of directory objects that can manage the device template and the related deviceInstances.
Owners can be represented as service principals, users, or applications.
An owner has full privileges over the device template and doesn't require other administrator roles to create, update, or delete devices from this template, as well as to add or remove template owners.
There can be a maximum of 100 owners on a device template. 
Supports $expand.

EXTENSIONATTRIBUTES `<IMicrosoftGraphOnPremisesExtensionAttributes>`: onPremisesExtensionAttributes
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ExtensionAttribute1 <String>]`: First customizable extension attribute.
  - `[ExtensionAttribute10 <String>]`: Tenth customizable extension attribute.
  - `[ExtensionAttribute11 <String>]`: Eleventh customizable extension attribute.
  - `[ExtensionAttribute12 <String>]`: Twelfth customizable extension attribute.
  - `[ExtensionAttribute13 <String>]`: Thirteenth customizable extension attribute.
  - `[ExtensionAttribute14 <String>]`: Fourteenth customizable extension attribute.
  - `[ExtensionAttribute15 <String>]`: Fifteenth customizable extension attribute.
  - `[ExtensionAttribute2 <String>]`: Second customizable extension attribute.
  - `[ExtensionAttribute3 <String>]`: Third customizable extension attribute.
  - `[ExtensionAttribute4 <String>]`: Fourth customizable extension attribute.
  - `[ExtensionAttribute5 <String>]`: Fifth customizable extension attribute.
  - `[ExtensionAttribute6 <String>]`: Sixth customizable extension attribute.
  - `[ExtensionAttribute7 <String>]`: Seventh customizable extension attribute.
  - `[ExtensionAttribute8 <String>]`: Eighth customizable extension attribute.
  - `[ExtensionAttribute9 <String>]`: Ninth customizable extension attribute.

EXTENSIONS `<IMicrosoftGraphExtension- `[]`>`: The collection of open extensions defined for the device.
Read-only.
Nullable.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.

MEMBEROF `<IMicrosoftGraphDirectoryObject- `[]`>`: Groups and administrative units that this device is a member of.
Read-only.
Nullable.
Supports $expand.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.

REGISTEREDOWNERS `<IMicrosoftGraphDirectoryObject- `[]`>`: The user that cloud joined the device or registered their personal device.
The registered owner is set at the time of registration.
Read-only.
Nullable.
Supports $expand.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.

REGISTEREDUSERS `<IMicrosoftGraphDirectoryObject- `[]`>`: Collection of registered users of the device.
For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.
Read-only.
Nullable.
Supports $expand.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.

TRANSITIVEMEMBEROF `<IMicrosoftGraphDirectoryObject- `[]`>`: Groups and administrative units that this device is a member of.
This operation is transitive.
Supports $expand.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.

USAGERIGHTS `<IMicrosoftGraphUsageRight- `[]`>`: Represents the usage rights a device has been granted.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[CatalogId <String>]`: Product id corresponding to the usage right.
  - `[ServiceIdentifier <String>]`: Identifier of the service corresponding to the usage right.
  - `[State <String>]`: usageRightState

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/new-mgbetadevice](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/new-mgbetadevice)

[https://learn.microsoft.com/graph/api/device-post-devices?view=graph-rest-beta](https://learn.microsoft.com/graph/api/device-post-devices?view=graph-rest-beta)























