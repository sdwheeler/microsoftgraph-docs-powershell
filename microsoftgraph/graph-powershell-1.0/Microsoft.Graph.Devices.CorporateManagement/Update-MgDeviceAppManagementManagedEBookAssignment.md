---
external help file: Microsoft.Graph.Devices.CorporateManagement-help.xml
Module Name: Microsoft.Graph.Devices.CorporateManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.devices.corporatemanagement/update-mgdeviceappmanagementmanagedebookassignment
schema: 2.0.0
ms.subservice: intune
---

# Update-MgDeviceAppManagementManagedEBookAssignment

## SYNOPSIS
Update the properties of a iosVppEBookAssignment object.

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaDeviceAppManagementManagedEBookAssignment](/powershell/module/Microsoft.Graph.Beta.Devices.CorporateManagement/Update-MgBetaDeviceAppManagementManagedEBookAssignment?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgDeviceAppManagementManagedEBookAssignment -ManagedEBookAssignmentId <String> -ManagedEBookId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-Id <String>]
 [-InstallIntent <InstallIntent>] [-Target <Hashtable>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgDeviceAppManagementManagedEBookAssignment -ManagedEBookAssignmentId <String> -ManagedEBookId <String>
 -BodyParameter <IMicrosoftGraphManagedEBookAssignment> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgDeviceAppManagementManagedEBookAssignment -InputObject <IDevicesCorporateManagementIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-Id <String>]
 [-InstallIntent <InstallIntent>] [-Target <Hashtable>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgDeviceAppManagementManagedEBookAssignment -InputObject <IDevicesCorporateManagementIdentity>
 -BodyParameter <IMicrosoftGraphManagedEBookAssignment> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the properties of a iosVppEBookAssignment object.

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
	"@odata.type" = "#microsoft.graph.iosVppEBookAssignment"
	target = @{
		"@odata.type" = "microsoft.graph.deviceAndAppManagementAssignmentTarget"
	}
	installIntent = "required"
}

Update-MgDeviceAppManagementManagedEBookAssignment -ManagedEBookId $managedEBookId -ManagedEBookAssignmentId $managedEBookAssignmentId -BodyParameter $params

```
This example shows how to use the Update-MgDeviceAppManagementManagedEBookAssignment Cmdlet.


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
Contains properties used to assign a eBook to a group.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphManagedEBookAssignment
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

### -InstallIntent
Possible values for the install intent chosen by the admin.

```yaml
Type: InstallIntent
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ManagedEBookAssignmentId
The unique identifier of managedEBookAssignment

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

### -ManagedEBookId
The unique identifier of managedEBook

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

### -Target
Base type for assignment targets.

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
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphManagedEBookAssignment
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphManagedEBookAssignment
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphManagedEBookAssignment>`: Contains properties used to assign a eBook to a group.
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[InstallIntent <InstallIntent?>]`: Possible values for the install intent chosen by the admin.
  - `[Target <IMicrosoftGraphDeviceAndAppManagementAssignmentTarget>]`: Base type for assignment targets.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.

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

[https://learn.microsoft.com/powershell/module/microsoft.graph.devices.corporatemanagement/update-mgdeviceappmanagementmanagedebookassignment](https://learn.microsoft.com/powershell/module/microsoft.graph.devices.corporatemanagement/update-mgdeviceappmanagementmanagedebookassignment)

[https://learn.microsoft.com/graph/api/intune-books-iosvppebookassignment-update?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/intune-books-iosvppebookassignment-update?view=graph-rest-1.0)























