---
external help file: Microsoft.Graph.Identity.DirectoryManagement-help.xml
Module Name: Microsoft.Graph.Identity.DirectoryManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.directorymanagement/update-mgdevicebydeviceid
schema: 2.0.0
ms.subservice: entra-directory-management
---

# Update-MgDeviceByDeviceId

## SYNOPSIS
Update the properties of a registered device.
Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaDeviceByDeviceId](/powershell/module/Microsoft.Graph.Beta.Identity.DirectoryManagement/Update-MgBetaDeviceByDeviceId?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgDeviceByDeviceId -DeviceId <String> [-ResponseHeadersVariable <String>] [-AccountEnabled]
 [-AdditionalProperties <Hashtable>] [-AlternativeSecurityIds <IMicrosoftGraphAlternativeSecurityId[]>]
 [-ApproximateLastSignInDateTime <DateTime>] [-ComplianceExpirationDateTime <DateTime>]
 [-DeletedDateTime <DateTime>] [-DeviceCategory <String>] [-DeviceId1 <String>] [-DeviceMetadata <String>]
 [-DeviceOwnership <String>] [-DeviceVersion <Int32>] [-DisplayName <String>] [-EnrollmentProfileName <String>]
 [-EnrollmentType <String>] [-Extensions <IMicrosoftGraphExtension[]>] [-Id <String>] [-IsCompliant]
 [-IsManaged] [-IsManagementRestricted] [-IsRooted] [-ManagementType <String>] [-Manufacturer <String>]
 [-MdmAppId <String>] [-MemberOf <IMicrosoftGraphDirectoryObject[]>] [-Model <String>]
 [-OnPremisesLastSyncDateTime <DateTime>] [-OnPremisesSecurityIdentifier <String>] [-OnPremisesSyncEnabled]
 [-OperatingSystem <String>] [-OperatingSystemVersion <String>] [-PhysicalIds <String[]>]
 [-ProfileType <String>] [-RegisteredOwners <IMicrosoftGraphDirectoryObject[]>]
 [-RegisteredUsers <IMicrosoftGraphDirectoryObject[]>] [-RegistrationDateTime <DateTime>]
 [-SystemLabels <String[]>] [-TransitiveMemberOf <IMicrosoftGraphDirectoryObject[]>] [-TrustType <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgDeviceByDeviceId [-DeviceId <String>] -InputObject <IIdentityDirectoryManagementIdentity>
 [-ResponseHeadersVariable <String>] [-AccountEnabled] [-AdditionalProperties <Hashtable>]
 [-AlternativeSecurityIds <IMicrosoftGraphAlternativeSecurityId[]>] [-ApproximateLastSignInDateTime <DateTime>]
 [-ComplianceExpirationDateTime <DateTime>] [-DeletedDateTime <DateTime>] [-DeviceCategory <String>]
 [-DeviceMetadata <String>] [-DeviceOwnership <String>] [-DeviceVersion <Int32>] [-DisplayName <String>]
 [-EnrollmentProfileName <String>] [-EnrollmentType <String>] [-Extensions <IMicrosoftGraphExtension[]>]
 [-Id <String>] [-IsCompliant] [-IsManaged] [-IsManagementRestricted] [-IsRooted] [-ManagementType <String>]
 [-Manufacturer <String>] [-MdmAppId <String>] [-MemberOf <IMicrosoftGraphDirectoryObject[]>] [-Model <String>]
 [-OnPremisesLastSyncDateTime <DateTime>] [-OnPremisesSecurityIdentifier <String>] [-OnPremisesSyncEnabled]
 [-OperatingSystem <String>] [-OperatingSystemVersion <String>] [-PhysicalIds <String[]>]
 [-ProfileType <String>] [-RegisteredOwners <IMicrosoftGraphDirectoryObject[]>]
 [-RegisteredUsers <IMicrosoftGraphDirectoryObject[]>] [-RegistrationDateTime <DateTime>]
 [-SystemLabels <String[]>] [-TransitiveMemberOf <IMicrosoftGraphDirectoryObject[]>] [-TrustType <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgDeviceByDeviceId -DeviceId <String> -BodyParameter <IMicrosoftGraphDevice>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgDeviceByDeviceId -InputObject <IIdentityDirectoryManagementIdentity>
 -BodyParameter <IMicrosoftGraphDevice> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the properties of a registered device.
Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.

## EXAMPLES

## PARAMETERS

### -AccountEnabled
true if the account is enabled; otherwise, false.
Required.
Default is true.
Supports $filter (eq, ne, not, in).
Only callers with at least the Cloud Device Administrator role can set this property.

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

### -AlternativeSecurityIds
For internal use only.
Not nullable.
Supports $filter (eq, not, ge, le).
To construct, see NOTES section for ALTERNATIVESECURITYIDS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAlternativeSecurityId[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ComplianceExpirationDateTime
The timestamp when the device is no longer deemed compliant.
The timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.

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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceId
Alternate key of device

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

```yaml
Type: String
Parameter Sets: UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceId1
Unique identifier set by Azure Device Registration Service at the time of registration.
This alternate key can be used to reference the device object.
Supports $filter (eq, ne, not, startsWith).

```yaml
Type: String
Parameter Sets: UpdateExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
This property is set by Intune.

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

### -EnrollmentType
Enrollment type of the device.
Intune sets this property.
Possible values are: unknown, userEnrollment, deviceEnrollmentManager, appleBulkWithUser, appleBulkWithoutUser, windowsAzureADJoin, windowsBulkUserless, windowsAutoEnrollment, windowsBulkAzureDomainJoin, windowsCoManagement, windowsAzureADJoinUsingDeviceAuth,appleUserEnrollment, appleUserEnrollmentWithServiceAccount.
NOTE: This property might return other values apart from those listed.

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

### -Extensions
The collection of open extensions defined for the device.
Read-only.
Nullable.
To construct, see NOTES section for EXTENSIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphExtension[]
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
Type: IIdentityDirectoryManagementIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsCompliant
true if the device complies with Mobile Device Management (MDM) policies; otherwise, false.
Read-only.
This can only be updated by Intune for any device OS type or by an approved MDM app for Windows OS devices.
Supports $filter (eq, ne, not).

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

### -IsManaged
true if the device is managed by a Mobile Device Management (MDM) app; otherwise, false.
This can only be updated by Intune for any device OS type or by an approved MDM app for Windows OS devices.
Supports $filter (eq, ne, not).

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

### -IsManagementRestricted


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

### -IsRooted
true if the device is rooted or jail-broken.
This property can only be updated by Intune.

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

### -ManagementType
The management channel of the device.
This property is set by Intune.
Possible values are: eas, mdm, easMdm, intuneClient, easIntuneClient, configurationManagerClient, configurationManagerClientMdm, configurationManagerClientMdmEas, unknown, jamf, googleCloudDevicePolicyController.

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

### -Manufacturer
Manufacturer of the device.
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

### -MdmAppId
Application identifier used to register device into MDM.
Read-only.
Supports $filter (eq, ne, not, startsWith).

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

### -MemberOf
Groups and administrative units that this device is a member of.
Read-only.
Nullable.
Supports $expand.
To construct, see NOTES section for MEMBEROF properties and create a hash table.

```yaml
Type: IMicrosoftGraphDirectoryObject[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OperatingSystemVersion
The version of the operating system on the device.
Required.
Supports $filter (eq, ne, not, ge, le, startsWith, and eq on null values).

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

### -PhysicalIds
For internal use only.
Not nullable.
Supports $filter (eq, not, ge, le, startsWith,/$count eq 0, /$count ne 0).

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

### -ProfileType
The profile type of the device.
Possible values: RegisteredDevice (default), SecureVM, Printer, Shared, IoT.

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

### -RegisteredOwners
The user that cloud joined the device or registered their personal device.
The registered owner is set at the time of registration.
Read-only.
Nullable.
Supports $expand.
To construct, see NOTES section for REGISTEREDOWNERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphDirectoryObject[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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

### -SystemLabels
List of labels applied to the device by the system.
Supports $filter (/$count eq 0, /$count ne 0).

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

### -TransitiveMemberOf
Groups and administrative units that the device is a member of.
This operation is transitive.
Supports $expand.
To construct, see NOTES section for TRANSITIVEMEMBEROF properties and create a hash table.

```yaml
Type: IMicrosoftGraphDirectoryObject[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Possible values: Workplace (indicates bring your own personal devices), AzureAd (Cloud-only joined devices), ServerAd (on-premises domain joined devices joined to Microsoft Entra ID).
For more information, see Introduction to device management in Microsoft Entra ID.
Supports $filter (eq, ne, not, in).

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

### Microsoft.Graph.PowerShell.Models.IIdentityDirectoryManagementIdentity
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphDevice
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphDevice
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
Required.
Default is true.
Supports $filter (eq, ne, not, in).
Only callers with at least the Cloud Device Administrator role can set this property.
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
  - `[ComplianceExpirationDateTime <DateTime?>]`: The timestamp when the device is no longer deemed compliant.
The timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
  - `[DeviceCategory <String>]`: User-defined property set by Intune to automatically add devices to groups and simplify managing devices.
  - `[DeviceId <String>]`: Unique identifier set by Azure Device Registration Service at the time of registration.
This alternate key can be used to reference the device object.
Supports $filter (eq, ne, not, startsWith).
  - `[DeviceMetadata <String>]`: For internal use only.
Set to null.
  - `[DeviceOwnership <String>]`: Ownership of the device.
Intune sets this property.
Possible values are: unknown, company, personal.
  - `[DeviceVersion <Int32?>]`: For internal use only.
  - `[DisplayName <String>]`: The display name for the device.
Maximum length is 256 characters.
Required.
Supports $filter (eq, ne, not, ge, le, in, startsWith, and eq on null values), $search, and $orderby.
  - `[EnrollmentProfileName <String>]`: Enrollment profile applied to the device.
For example, Apple Device Enrollment Profile, Device enrollment - Corporate device identifiers, or Windows Autopilot profile name.
This property is set by Intune.
  - `[EnrollmentType <String>]`: Enrollment type of the device.
Intune sets this property.
Possible values are: unknown, userEnrollment, deviceEnrollmentManager, appleBulkWithUser, appleBulkWithoutUser, windowsAzureADJoin, windowsBulkUserless, windowsAutoEnrollment, windowsBulkAzureDomainJoin, windowsCoManagement, windowsAzureADJoinUsingDeviceAuth,appleUserEnrollment, appleUserEnrollmentWithServiceAccount.
NOTE: This property might return other values apart from those listed.
  - `[Extensions <IMicrosoftGraphExtension- `[]`>]`: The collection of open extensions defined for the device.
Read-only.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[IsCompliant <Boolean?>]`: true if the device complies with Mobile Device Management (MDM) policies; otherwise, false.
Read-only.
This can only be updated by Intune for any device OS type or by an approved MDM app for Windows OS devices.
Supports $filter (eq, ne, not).
  - `[IsManaged <Boolean?>]`: true if the device is managed by a Mobile Device Management (MDM) app; otherwise, false.
This can only be updated by Intune for any device OS type or by an approved MDM app for Windows OS devices.
Supports $filter (eq, ne, not).
  - `[IsManagementRestricted <Boolean?>]`:
  - `[IsRooted <Boolean?>]`: true if the device is rooted or jail-broken.
This property can only be updated by Intune.
  - `[ManagementType <String>]`: The management channel of the device.
This property is set by Intune.
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
  - `[OperatingSystemVersion <String>]`: The version of the operating system on the device.
Required.
Supports $filter (eq, ne, not, ge, le, startsWith, and eq on null values).
  - `[PhysicalIds <String- `[]`>]`: For internal use only.
Not nullable.
Supports $filter (eq, not, ge, le, startsWith,/$count eq 0, /$count ne 0).
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
  - `[SystemLabels <String- `[]`>]`: List of labels applied to the device by the system.
Supports $filter (/$count eq 0, /$count ne 0).
  - `[TransitiveMemberOf <IMicrosoftGraphDirectoryObject- `[]`>]`: Groups and administrative units that the device is a member of.
This operation is transitive.
Supports $expand.
  - `[TrustType <String>]`: Type of trust for the joined device.
Read-only.
Possible values:  Workplace (indicates bring your own personal devices), AzureAd (Cloud-only joined devices), ServerAd (on-premises domain joined devices joined to Microsoft Entra ID).
For more information, see Introduction to device management in Microsoft Entra ID.
Supports $filter (eq, ne, not, in).

EXTENSIONS `<IMicrosoftGraphExtension- `[]`>`: The collection of open extensions defined for the device.
Read-only.
Nullable.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.

INPUTOBJECT `<IIdentityDirectoryManagementIdentity>`: Identity Parameter
  - `[AdministrativeUnitId <String>]`: The unique identifier of administrativeUnit
  - `[AllowedValueId <String>]`: The unique identifier of allowedValue
  - `[AttributeSetId <String>]`: The unique identifier of attributeSet
  - `[CommerceSubscriptionId <String>]`: Alternate key of companySubscription
  - `[CompanySubscriptionId <String>]`: The unique identifier of companySubscription
  - `[ContractId <String>]`: The unique identifier of contract
  - `[CustomSecurityAttributeDefinitionId <String>]`: The unique identifier of customSecurityAttributeDefinition
  - `[DeviceId <String>]`: The unique identifier of device
  - `[DeviceLocalCredentialInfoId <String>]`: The unique identifier of deviceLocalCredentialInfo
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[DirectoryRoleId <String>]`: The unique identifier of directoryRole
  - `[DirectoryRoleTemplateId <String>]`: The unique identifier of directoryRoleTemplate
  - `[DomainDnsRecordId <String>]`: The unique identifier of domainDnsRecord
  - `[DomainId <String>]`: The unique identifier of domain
  - `[DomainName <String>]`: Usage: domainName='{domainName}'
  - `[ExtensionId <String>]`: The unique identifier of extension
  - `[IdentityProviderBaseId <String>]`: The unique identifier of identityProviderBase
  - `[InternalDomainFederationId <String>]`: The unique identifier of internalDomainFederation
  - `[OnPremisesDirectorySynchronizationId <String>]`: The unique identifier of onPremisesDirectorySynchronization
  - `[OrgContactId <String>]`: The unique identifier of orgContact
  - `[OrganizationId <String>]`: The unique identifier of organization
  - `[OrganizationalBrandingLocalizationId <String>]`: The unique identifier of organizationalBrandingLocalization
  - `[ProfileCardPropertyId <String>]`: The unique identifier of profileCardProperty
  - `[RoleTemplateId <String>]`: Alternate key of directoryRole
  - `[ScopedRoleMembershipId <String>]`: The unique identifier of scopedRoleMembership
  - `[SubscribedSkuId <String>]`: The unique identifier of subscribedSku
  - `[TenantId <String>]`: Usage: tenantId='{tenantId}'
  - `[UserId <String>]`: The unique identifier of user

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

TRANSITIVEMEMBEROF `<IMicrosoftGraphDirectoryObject- `[]`>`: Groups and administrative units that the device is a member of.
This operation is transitive.
Supports $expand.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.directorymanagement/update-mgdevicebydeviceid](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.directorymanagement/update-mgdevicebydeviceid)

[https://learn.microsoft.com/graph/api/device-update?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/device-update?view=graph-rest-1.0)
























