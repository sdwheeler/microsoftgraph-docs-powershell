---
external help file: Microsoft.Graph.DeviceManagement-help.xml
Module Name: Microsoft.Graph.DeviceManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement/update-mgdevicemanagementmanageddevicewindowsprotectionstate
schema: 2.0.0
---

# Update-MgDeviceManagementManagedDeviceWindowsProtectionState

## SYNOPSIS
Update the navigation property windowsProtectionState in deviceManagement

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaDeviceManagementManagedDeviceWindowsProtectionState](/powershell/module/Microsoft.Graph.Beta.DeviceManagement/Update-MgBetaDeviceManagementManagedDeviceWindowsProtectionState?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgDeviceManagementManagedDeviceWindowsProtectionState -ManagedDeviceId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-AntiMalwareVersion <String>]
 [-DetectedMalwareState <IMicrosoftGraphWindowsDeviceMalwareState[]>] [-DeviceState <WindowsDeviceHealthState>]
 [-EngineVersion <String>] [-FullScanOverdue] [-FullScanRequired] [-Id <String>] [-IsVirtualMachine]
 [-LastFullScanDateTime <DateTime>] [-LastFullScanSignatureVersion <String>]
 [-LastQuickScanDateTime <DateTime>] [-LastQuickScanSignatureVersion <String>]
 [-LastReportedDateTime <DateTime>] [-MalwareProtectionEnabled] [-NetworkInspectionSystemEnabled]
 [-ProductStatus <WindowsDefenderProductStatus>] [-QuickScanOverdue] [-RealTimeProtectionEnabled]
 [-RebootRequired] [-SignatureUpdateOverdue] [-SignatureVersion <String>] [-TamperProtectionEnabled]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgDeviceManagementManagedDeviceWindowsProtectionState -ManagedDeviceId <String>
 -BodyParameter <IMicrosoftGraphWindowsProtectionState> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgDeviceManagementManagedDeviceWindowsProtectionState -InputObject <IDeviceManagementIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-AntiMalwareVersion <String>]
 [-DetectedMalwareState <IMicrosoftGraphWindowsDeviceMalwareState[]>] [-DeviceState <WindowsDeviceHealthState>]
 [-EngineVersion <String>] [-FullScanOverdue] [-FullScanRequired] [-Id <String>] [-IsVirtualMachine]
 [-LastFullScanDateTime <DateTime>] [-LastFullScanSignatureVersion <String>]
 [-LastQuickScanDateTime <DateTime>] [-LastQuickScanSignatureVersion <String>]
 [-LastReportedDateTime <DateTime>] [-MalwareProtectionEnabled] [-NetworkInspectionSystemEnabled]
 [-ProductStatus <WindowsDefenderProductStatus>] [-QuickScanOverdue] [-RealTimeProtectionEnabled]
 [-RebootRequired] [-SignatureUpdateOverdue] [-SignatureVersion <String>] [-TamperProtectionEnabled]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgDeviceManagementManagedDeviceWindowsProtectionState -InputObject <IDeviceManagementIdentity>
 -BodyParameter <IMicrosoftGraphWindowsProtectionState> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property windowsProtectionState in deviceManagement

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

### -AntiMalwareVersion
Current anti malware version

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
Device protection status entity.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsProtectionState
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

### -DetectedMalwareState
Device malware list
To construct, see NOTES section for DETECTEDMALWARESTATE properties and create a hash table.

```yaml
Type: IMicrosoftGraphWindowsDeviceMalwareState[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceState
Computer endpoint protection state

```yaml
Type: WindowsDeviceHealthState
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EngineVersion
Current endpoint protection engine's version

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

### -FullScanOverdue
When TRUE indicates full scan is overdue, when FALSE indicates full scan is not overdue.
Defaults to setting on client device.

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

### -FullScanRequired
When TRUE indicates full scan is required, when FALSE indicates full scan is not required.
Defaults to setting on client device.

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
Type: IDeviceManagementIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsVirtualMachine
When TRUE indicates the device is a virtual machine, when FALSE indicates the device is not a virtual machine.
Defaults to setting on client device.

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

### -LastFullScanDateTime
Last quick scan datetime

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

### -LastFullScanSignatureVersion
Last full scan signature version

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

### -LastQuickScanDateTime
Last quick scan datetime

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

### -LastQuickScanSignatureVersion
Last quick scan signature version

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

### -LastReportedDateTime
Last device health status reported time

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

### -MalwareProtectionEnabled
When TRUE indicates anti malware is enabled when FALSE indicates anti malware is not enabled.

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

### -ManagedDeviceId
The unique identifier of managedDevice

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

### -NetworkInspectionSystemEnabled
When TRUE indicates network inspection system enabled, when FALSE indicates network inspection system is not enabled.
Defaults to setting on client device.

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

### -ProductStatus
Product Status of Windows Defender

```yaml
Type: WindowsDefenderProductStatus
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -QuickScanOverdue
When TRUE indicates quick scan is overdue, when FALSE indicates quick scan is not overdue.
Defaults to setting on client device.

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

### -RealTimeProtectionEnabled
When TRUE indicates real time protection is enabled, when FALSE indicates real time protection is not enabled.
Defaults to setting on client device.

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

### -RebootRequired
When TRUE indicates reboot is required, when FALSE indicates when TRUE indicates reboot is not required.
Defaults to setting on client device.

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

### -SignatureUpdateOverdue
When TRUE indicates signature is out of date, when FALSE indicates signature is not out of date.
Defaults to setting on client device.

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

### -SignatureVersion
Current malware definitions version

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

### -TamperProtectionEnabled
When TRUE indicates the Windows Defender tamper protection feature is enabled, when FALSE indicates the Windows Defender tamper protection feature is not enabled.
Defaults to setting on client device.

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

### Microsoft.Graph.PowerShell.Models.IDeviceManagementIdentity
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphWindowsProtectionState
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphWindowsProtectionState
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphWindowsProtectionState>`: Device protection status entity.
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AntiMalwareVersion <String>]`: Current anti malware version
  - `[DetectedMalwareState <IMicrosoftGraphWindowsDeviceMalwareState- `[]`>]`: Device malware list
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AdditionalInformationUrl <String>]`: Information URL to learn more about the malware
    - `[Category <WindowsMalwareCategory?>]`: Malware category id
    - `[DetectionCount <Int32?>]`: Number of times the malware is detected
    - `[DisplayName <String>]`: Malware name
    - `[ExecutionState <WindowsMalwareExecutionState?>]`: Malware execution status
    - `[InitialDetectionDateTime <DateTime?>]`: Initial detection datetime of the malware
    - `[LastStateChangeDateTime <DateTime?>]`: The last time this particular threat was changed
    - `[Severity <WindowsMalwareSeverity?>]`: Malware severity
    - `[State <WindowsMalwareState?>]`: Malware current status
    - `[ThreatState <WindowsMalwareThreatState?>]`: Malware threat status
  - `[DeviceState <WindowsDeviceHealthState?>]`: Computer endpoint protection state
  - `[EngineVersion <String>]`: Current endpoint protection engine's version
  - `[FullScanOverdue <Boolean?>]`: When TRUE indicates full scan is overdue, when FALSE indicates full scan is not overdue.
Defaults to setting on client device.
  - `[FullScanRequired <Boolean?>]`: When TRUE indicates full scan is required, when FALSE indicates full scan is not required.
Defaults to setting on client device.
  - `[IsVirtualMachine <Boolean?>]`: When TRUE indicates the device is a virtual machine, when FALSE indicates the device is not a virtual machine.
Defaults to setting on client device.
  - `[LastFullScanDateTime <DateTime?>]`: Last quick scan datetime
  - `[LastFullScanSignatureVersion <String>]`: Last full scan signature version
  - `[LastQuickScanDateTime <DateTime?>]`: Last quick scan datetime
  - `[LastQuickScanSignatureVersion <String>]`: Last quick scan signature version
  - `[LastReportedDateTime <DateTime?>]`: Last device health status reported time
  - `[MalwareProtectionEnabled <Boolean?>]`: When TRUE indicates anti malware is enabled when FALSE indicates anti malware is not enabled.
  - `[NetworkInspectionSystemEnabled <Boolean?>]`: When TRUE indicates network inspection system enabled, when FALSE indicates network inspection system is not enabled.
Defaults to setting on client device.
  - `[ProductStatus <WindowsDefenderProductStatus?>]`: Product Status of Windows Defender
  - `[QuickScanOverdue <Boolean?>]`: When TRUE indicates quick scan is overdue, when FALSE indicates quick scan is not overdue.
Defaults to setting on client device.
  - `[RealTimeProtectionEnabled <Boolean?>]`: When TRUE indicates real time protection is enabled, when FALSE indicates real time protection is not enabled.
Defaults to setting on client device.
  - `[RebootRequired <Boolean?>]`: When TRUE indicates reboot is required, when FALSE indicates when TRUE indicates reboot is not required.
Defaults to setting on client device.
  - `[SignatureUpdateOverdue <Boolean?>]`: When TRUE indicates signature is out of date, when FALSE indicates signature is not out of date.
Defaults to setting on client device.
  - `[SignatureVersion <String>]`: Current malware definitions version
  - `[TamperProtectionEnabled <Boolean?>]`: When TRUE indicates the Windows Defender tamper protection feature is enabled, when FALSE indicates the Windows Defender tamper protection feature is not enabled.
Defaults to setting on client device.

DETECTEDMALWARESTATE `<IMicrosoftGraphWindowsDeviceMalwareState- `[]`>`: Device malware list
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AdditionalInformationUrl <String>]`: Information URL to learn more about the malware
  - `[Category <WindowsMalwareCategory?>]`: Malware category id
  - `[DetectionCount <Int32?>]`: Number of times the malware is detected
  - `[DisplayName <String>]`: Malware name
  - `[ExecutionState <WindowsMalwareExecutionState?>]`: Malware execution status
  - `[InitialDetectionDateTime <DateTime?>]`: Initial detection datetime of the malware
  - `[LastStateChangeDateTime <DateTime?>]`: The last time this particular threat was changed
  - `[Severity <WindowsMalwareSeverity?>]`: Malware severity
  - `[State <WindowsMalwareState?>]`: Malware current status
  - `[ThreatState <WindowsMalwareThreatState?>]`: Malware threat status

INPUTOBJECT `<IDeviceManagementIdentity>`: Identity Parameter
  - `[AppLogCollectionRequestId <String>]`: The unique identifier of appLogCollectionRequest
  - `[BrowserSharedCookieId <String>]`: The unique identifier of browserSharedCookie
  - `[BrowserSiteId <String>]`: The unique identifier of browserSite
  - `[BrowserSiteListId <String>]`: The unique identifier of browserSiteList
  - `[DetectedAppId <String>]`: The unique identifier of detectedApp
  - `[DeviceCategoryId <String>]`: The unique identifier of deviceCategory
  - `[DeviceComplianceActionItemId <String>]`: The unique identifier of deviceComplianceActionItem
  - `[DeviceComplianceDeviceStatusId <String>]`: The unique identifier of deviceComplianceDeviceStatus
  - `[DeviceCompliancePolicyAssignmentId <String>]`: The unique identifier of deviceCompliancePolicyAssignment
  - `[DeviceCompliancePolicyId <String>]`: The unique identifier of deviceCompliancePolicy
  - `[DeviceCompliancePolicySettingStateSummaryId <String>]`: The unique identifier of deviceCompliancePolicySettingStateSummary
  - `[DeviceCompliancePolicyStateId <String>]`: The unique identifier of deviceCompliancePolicyState
  - `[DeviceComplianceScheduledActionForRuleId <String>]`: The unique identifier of deviceComplianceScheduledActionForRule
  - `[DeviceComplianceSettingStateId <String>]`: The unique identifier of deviceComplianceSettingState
  - `[DeviceComplianceUserStatusId <String>]`: The unique identifier of deviceComplianceUserStatus
  - `[DeviceConfigurationAssignmentId <String>]`: The unique identifier of deviceConfigurationAssignment
  - `[DeviceConfigurationDeviceStatusId <String>]`: The unique identifier of deviceConfigurationDeviceStatus
  - `[DeviceConfigurationId <String>]`: The unique identifier of deviceConfiguration
  - `[DeviceConfigurationStateId <String>]`: The unique identifier of deviceConfigurationState
  - `[DeviceConfigurationUserStatusId <String>]`: The unique identifier of deviceConfigurationUserStatus
  - `[DeviceLogCollectionResponseId <String>]`: The unique identifier of deviceLogCollectionResponse
  - `[DeviceManagementTroubleshootingEventId <String>]`: The unique identifier of deviceManagementTroubleshootingEvent
  - `[LocalizedNotificationMessageId <String>]`: The unique identifier of localizedNotificationMessage
  - `[MalwareStateForWindowsDeviceId <String>]`: The unique identifier of malwareStateForWindowsDevice
  - `[ManagedDeviceId <String>]`: The unique identifier of managedDevice
  - `[MobileAppTroubleshootingEventId <String>]`: The unique identifier of mobileAppTroubleshootingEvent
  - `[NotificationMessageTemplateId <String>]`: The unique identifier of notificationMessageTemplate
  - `[SecretReferenceValueId <String>]`: Usage: secretReferenceValueId='{secretReferenceValueId}'
  - `[SettingStateDeviceSummaryId <String>]`: The unique identifier of settingStateDeviceSummary
  - `[WindowsDeviceMalwareStateId <String>]`: The unique identifier of windowsDeviceMalwareState
  - `[WindowsInformationProtectionAppLearningSummaryId <String>]`: The unique identifier of windowsInformationProtectionAppLearningSummary
  - `[WindowsInformationProtectionNetworkLearningSummaryId <String>]`: The unique identifier of windowsInformationProtectionNetworkLearningSummary
  - `[WindowsMalwareInformationId <String>]`: The unique identifier of windowsMalwareInformation

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement/update-mgdevicemanagementmanageddevicewindowsprotectionstate](https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement/update-mgdevicemanagementmanageddevicewindowsprotectionstate)
























