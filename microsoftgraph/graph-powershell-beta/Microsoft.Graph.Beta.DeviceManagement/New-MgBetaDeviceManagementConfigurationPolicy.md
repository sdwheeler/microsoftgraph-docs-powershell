---
external help file: Microsoft.Graph.Beta.DeviceManagement-help.xml
Module Name: Microsoft.Graph.Beta.DeviceManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement/new-mgbetadevicemanagementconfigurationpolicy
schema: 2.0.0
---

# New-MgBetaDeviceManagementConfigurationPolicy

## SYNOPSIS
Create new navigation property to configurationPolicies for deviceManagement

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaDeviceManagementConfigurationPolicy [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>]
 [-Assignments <IMicrosoftGraphDeviceManagementConfigurationPolicyAssignment[]>] [-CreatedDateTime <DateTime>]
 [-CreationSource <String>] [-Description <String>] [-Id <String>] [-LastModifiedDateTime <DateTime>]
 [-Name <String>] [-Platforms <DeviceManagementConfigurationPlatforms>]
 [-PriorityMetaData <IMicrosoftGraphDeviceManagementPriorityMetaData>] [-RoleScopeTagIds <String[]>]
 [-SettingCount <Int32>] [-Settings <IMicrosoftGraphDeviceManagementConfigurationSetting[]>]
 [-Technologies <DeviceManagementConfigurationTechnologies>]
 [-TemplateReference <IMicrosoftGraphDeviceManagementConfigurationPolicyTemplateReference>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaDeviceManagementConfigurationPolicy
 -BodyParameter <IMicrosoftGraphDeviceManagementConfigurationPolicy> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to configurationPolicies for deviceManagement

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | DeviceManagementConfiguration.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | DeviceManagementConfiguration.ReadWrite.All,  |

## EXAMPLES

## PARAMETERS

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

### -Assignments
Policy assignments
To construct, see NOTES section for ASSIGNMENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphDeviceManagementConfigurationPolicyAssignment[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
Device Management Configuration Policy
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphDeviceManagementConfigurationPolicy
Parameter Sets: Create
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
Policy creation date and time

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

### -CreationSource
Policy creation source

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

### -Description
Policy description

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
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedDateTime
Policy last modification date and time

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

### -Name
Policy name

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

### -Platforms
Supported platform types.

```yaml
Type: DeviceManagementConfigurationPlatforms
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PriorityMetaData
Priority metadata of the policy.
To construct, see NOTES section for PRIORITYMETADATA properties and create a hash table.

```yaml
Type: IMicrosoftGraphDeviceManagementPriorityMetaData
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

### -RoleScopeTagIds
List of Scope Tags for this Entity instance.

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

### -SettingCount
Number of settings

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

### -Settings
Policy settings
To construct, see NOTES section for SETTINGS properties and create a hash table.

```yaml
Type: IMicrosoftGraphDeviceManagementConfigurationSetting[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Technologies
Describes which technology this setting can be deployed with

```yaml
Type: DeviceManagementConfigurationTechnologies
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TemplateReference
Policy template reference information
To construct, see NOTES section for TEMPLATEREFERENCE properties and create a hash table.

```yaml
Type: IMicrosoftGraphDeviceManagementConfigurationPolicyTemplateReference
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphDeviceManagementConfigurationPolicy
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphDeviceManagementConfigurationPolicy
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ASSIGNMENTS `<IMicrosoftGraphDeviceManagementConfigurationPolicyAssignment- `[]`>`: Policy assignments
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Source <DeviceAndAppManagementAssignmentSource?>]`: Represents source of assignment.
  - `[SourceId <String>]`: The identifier of the source of the assignment.
  - `[Target <IMicrosoftGraphDeviceAndAppManagementAssignmentTarget>]`: Base type for assignment targets.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DeviceAndAppManagementAssignmentFilterId <String>]`: The ID of the filter for the target assignment.
    - `[DeviceAndAppManagementAssignmentFilterType <DeviceAndAppManagementAssignmentFilterType?>]`: Represents type of the assignment filter.

BODYPARAMETER `<IMicrosoftGraphDeviceManagementConfigurationPolicy>`: Device Management Configuration Policy
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Assignments <IMicrosoftGraphDeviceManagementConfigurationPolicyAssignment- `[]`>]`: Policy assignments
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Source <DeviceAndAppManagementAssignmentSource?>]`: Represents source of assignment.
    - `[SourceId <String>]`: The identifier of the source of the assignment.
    - `[Target <IMicrosoftGraphDeviceAndAppManagementAssignmentTarget>]`: Base type for assignment targets.
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DeviceAndAppManagementAssignmentFilterId <String>]`: The ID of the filter for the target assignment.
      - `[DeviceAndAppManagementAssignmentFilterType <DeviceAndAppManagementAssignmentFilterType?>]`: Represents type of the assignment filter.
  - `[CreatedDateTime <DateTime?>]`: Policy creation date and time
  - `[CreationSource <String>]`: Policy creation source
  - `[Description <String>]`: Policy description
  - `[LastModifiedDateTime <DateTime?>]`: Policy last modification date and time
  - `[Name <String>]`: Policy name
  - `[Platforms <DeviceManagementConfigurationPlatforms?>]`: Supported platform types.
  - `[PriorityMetaData <IMicrosoftGraphDeviceManagementPriorityMetaData>]`: Priority metadata of the policy.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Priority <Int32?>]`: Priority of the policy.
Valid values 1 to 500
  - `[RoleScopeTagIds <String- `[]`>]`: List of Scope Tags for this Entity instance.
  - `[SettingCount <Int32?>]`: Number of settings
  - `[Settings <IMicrosoftGraphDeviceManagementConfigurationSetting- `[]`>]`: Policy settings
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
  - `[Technologies <DeviceManagementConfigurationTechnologies?>]`: Describes which technology this setting can be deployed with
  - `[TemplateReference <IMicrosoftGraphDeviceManagementConfigurationPolicyTemplateReference>]`: Policy template reference information
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[TemplateFamily <DeviceManagementConfigurationTemplateFamily?>]`: Describes the TemplateFamily for the Template entity
    - `[TemplateId <String>]`: Template id

PRIORITYMETADATA `<IMicrosoftGraphDeviceManagementPriorityMetaData>`: Priority metadata of the policy.
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Priority <Int32?>]`: Priority of the policy.
Valid values 1 to 500

SETTINGS `<IMicrosoftGraphDeviceManagementConfigurationSetting- `[]`>`: Policy settings
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

TEMPLATEREFERENCE `<IMicrosoftGraphDeviceManagementConfigurationPolicyTemplateReference>`: Policy template reference information
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[TemplateFamily <DeviceManagementConfigurationTemplateFamily?>]`: Describes the TemplateFamily for the Template entity
  - `[TemplateId <String>]`: Template id

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement/new-mgbetadevicemanagementconfigurationpolicy](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement/new-mgbetadevicemanagementconfigurationpolicy)
























