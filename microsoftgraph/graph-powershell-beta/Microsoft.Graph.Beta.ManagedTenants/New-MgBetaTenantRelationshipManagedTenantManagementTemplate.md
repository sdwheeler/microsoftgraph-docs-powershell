---
external help file: Microsoft.Graph.Beta.ManagedTenants-help.xml
Module Name: Microsoft.Graph.Beta.ManagedTenants
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.managedtenants/new-mgbetatenantrelationshipmanagedtenantmanagementtemplate
schema: 2.0.0
---

# New-MgBetaTenantRelationshipManagedTenantManagementTemplate

## SYNOPSIS
Create new navigation property to managementTemplates for tenantRelationships

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaTenantRelationshipManagedTenantManagementTemplate [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Category <String>] [-CreatedByUserId <String>]
 [-CreatedDateTime <DateTime>] [-Description <String>] [-DisplayName <String>] [-Id <String>]
 [-InformationLinks <IMicrosoftGraphActionUrl[]>] [-LastActionByUserId <String>]
 [-LastActionDateTime <DateTime>]
 [-ManagementTemplateCollections <IMicrosoftGraphManagedTenantsManagementTemplateCollection[]>]
 [-ManagementTemplateSteps <IMicrosoftGraphManagedTenantsManagementTemplateStep[]>]
 [-Parameters <IMicrosoftGraphManagedTenantsTemplateParameter[]>] [-Priority <Int32>] [-Provider <String>]
 [-UserImpact <String>] [-Version <Int32>] [-WorkloadActions <IMicrosoftGraphManagedTenantsWorkloadAction[]>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaTenantRelationshipManagedTenantManagementTemplate
 -BodyParameter <IMicrosoftGraphManagedTenantsManagementTemplate> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to managementTemplates for tenantRelationships

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

### -BodyParameter
managementTemplate
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphManagedTenantsManagementTemplate
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Category
managementCategory

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

### -CreatedByUserId


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

### -CreatedDateTime


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

### -Description
The description for the management template.
Optional.
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

### -DisplayName
The display name for the management template.
Required.
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

### -InformationLinks

To construct, see NOTES section for INFORMATIONLINKS properties and create a hash table.

```yaml
Type: IMicrosoftGraphActionUrl[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastActionByUserId


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

### -LastActionDateTime


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

### -ManagementTemplateCollections

To construct, see NOTES section for MANAGEMENTTEMPLATECOLLECTIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphManagedTenantsManagementTemplateCollection[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ManagementTemplateSteps

To construct, see NOTES section for MANAGEMENTTEMPLATESTEPS properties and create a hash table.

```yaml
Type: IMicrosoftGraphManagedTenantsManagementTemplateStep[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameters
The collection of parameters used by the management template.
Optional.
Read-only.
To construct, see NOTES section for PARAMETERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphManagedTenantsTemplateParameter[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Priority


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

### -Provider
managementProvider

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

### -UserImpact


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

### -Version


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

### -WorkloadActions
The collection of workload actions associated with the management template.
Optional.
Read-only.
To construct, see NOTES section for WORKLOADACTIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphManagedTenantsWorkloadAction[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphManagedTenantsManagementTemplate
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphManagedTenantsManagementTemplate
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphManagedTenantsManagementTemplate>`: managementTemplate
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Category <String>]`: managementCategory
  - `[CreatedByUserId <String>]`: 
  - `[CreatedDateTime <DateTime?>]`: 
  - `[Description <String>]`: The description for the management template.
Optional.
Read-only.
  - `[DisplayName <String>]`: The display name for the management template.
Required.
Read-only.
  - `[InformationLinks <IMicrosoftGraphActionUrl- `[]`>]`: 
    - `[DisplayName <String>]`: Brief title for the page that the links directs to.
    - `[Url <String>]`: The URL to the documentation or Microsoft Entra admin center page.
  - `[LastActionByUserId <String>]`: 
  - `[LastActionDateTime <DateTime?>]`: 
  - `[ManagementTemplateCollections <IMicrosoftGraphManagedTenantsManagementTemplateCollection- `[]`>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[CreatedByUserId <String>]`: 
    - `[CreatedDateTime <DateTime?>]`: 
    - `[Description <String>]`: 
    - `[DisplayName <String>]`: 
    - `[LastActionByUserId <String>]`: 
    - `[LastActionDateTime <DateTime?>]`: 
    - `[ManagementTemplates <IMicrosoftGraphManagedTenantsManagementTemplate- `[]`>]`: 
  - `[ManagementTemplateSteps <IMicrosoftGraphManagedTenantsManagementTemplateStep- `[]`>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AcceptedVersion <IMicrosoftGraphManagedTenantsManagementTemplateStepVersion>]`: managementTemplateStepVersion
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AcceptedFor <IMicrosoftGraphManagedTenantsManagementTemplateStep>]`: managementTemplateStep
      - `[ContentMarkdown <String>]`: 
      - `[CreatedByUserId <String>]`: 
      - `[CreatedDateTime <DateTime?>]`: 
      - `[Deployments <IMicrosoftGraphManagedTenantsManagementTemplateStepDeployment- `[]`>]`: 
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[CreatedByUserId <String>]`: 
        - `[CreatedDateTime <DateTime?>]`: 
        - `[Error <IMicrosoftGraphManagedTenantsGraphApiErrorDetails>]`: graphAPIErrorDetails
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Code <String>]`: 
          - `[Message <String>]`: 
        - `[LastActionByUserId <String>]`: 
        - `[LastActionDateTime <DateTime?>]`: 
        - `[Status <String>]`: managementTemplateDeploymentStatus
        - `[TemplateStepVersion <IMicrosoftGraphManagedTenantsManagementTemplateStepVersion>]`: managementTemplateStepVersion
        - `[TenantId <String>]`: 
      - `[LastActionByUserId <String>]`: 
      - `[LastActionDateTime <DateTime?>]`: 
      - `[Name <String>]`: 
      - `[TemplateStep <IMicrosoftGraphManagedTenantsManagementTemplateStep>]`: managementTemplateStep
      - `[Version <Int32?>]`: 
      - `[VersionInformation <String>]`: 
    - `[Category <String>]`: managementCategory
    - `[CreatedByUserId <String>]`: 
    - `[CreatedDateTime <DateTime?>]`: 
    - `[Description <String>]`: 
    - `[DisplayName <String>]`: 
    - `[InformationLinks <IMicrosoftGraphActionUrl- `[]`>]`: 
    - `[LastActionByUserId <String>]`: 
    - `[LastActionDateTime <DateTime?>]`: 
    - `[ManagementTemplate <IMicrosoftGraphManagedTenantsManagementTemplate>]`: managementTemplate
    - `[PortalLink <IMicrosoftGraphActionUrl>]`: actionUrl
    - `[Priority <Int32?>]`: 
    - `[UserImpact <String>]`: 
    - `[Versions <IMicrosoftGraphManagedTenantsManagementTemplateStepVersion- `[]`>]`: 
  - `[Parameters <IMicrosoftGraphManagedTenantsTemplateParameter- `[]`>]`: The collection of parameters used by the management template.
Optional.
Read-only.
    - `[Description <String>]`: The description for the template parameter.
Optional.
Read-only.
    - `[DisplayName <String>]`: The display name for the template parameter.
Required.
Read-only.
    - `[JsonAllowedValues <String>]`: The allowed values for the template parameter represented by a serialized string of JSON.
Optional.
Read-only.
    - `[JsonDefaultValue <String>]`: The default value for the template parameter represented by a serialized string of JSON.
Required.
Read-only.
    - `[ValueType <String>]`: managementParameterValueType
  - `[Priority <Int32?>]`: 
  - `[Provider <String>]`: managementProvider
  - `[UserImpact <String>]`: 
  - `[Version <Int32?>]`: 
  - `[WorkloadActions <IMicrosoftGraphManagedTenantsWorkloadAction- `[]`>]`: The collection of workload actions associated with the management template.
Optional.
Read-only.
    - `[ActionId <String>]`: The unique identifier for the workload action.
Required.
Read-only.
    - `[Category <String>]`: workloadActionCategory
    - `[Description <String>]`: The description for the workload action.
Optional.
Read-only.
    - `[DisplayName <String>]`: The display name for the workload action.
Optional.
Read-only.
    - `[Licenses <String- `[]`>]`: 
    - `[Service <String>]`: The service associated with workload action.
Optional.
Read-only.
    - `[Settings <IMicrosoftGraphManagedTenantsSetting- `[]`>]`: The collection of settings associated with the workload action.
Optional.
Read-only.
      - `[DisplayName <String>]`: The display name for the setting.
Required.
Read-only.
      - `[JsonValue <String>]`: The value for the setting serialized as string of JSON.
Required.
Read-only.
      - `[OverwriteAllowed <Boolean?>]`: A flag indicating whether the setting can be override existing configurations when applied.
Required.
Read-only.
      - `[SettingId <String>]`: 
      - `[ValueType <String>]`: managementParameterValueType

INFORMATIONLINKS `<IMicrosoftGraphActionUrl- `[]`>`: .
  - `[DisplayName <String>]`: Brief title for the page that the links directs to.
  - `[Url <String>]`: The URL to the documentation or Microsoft Entra admin center page.

MANAGEMENTTEMPLATECOLLECTIONS `<IMicrosoftGraphManagedTenantsManagementTemplateCollection- `[]`>`: .
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[CreatedByUserId <String>]`: 
  - `[CreatedDateTime <DateTime?>]`: 
  - `[Description <String>]`: 
  - `[DisplayName <String>]`: 
  - `[LastActionByUserId <String>]`: 
  - `[LastActionDateTime <DateTime?>]`: 
  - `[ManagementTemplates <IMicrosoftGraphManagedTenantsManagementTemplate- `[]`>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Category <String>]`: managementCategory
    - `[CreatedByUserId <String>]`: 
    - `[CreatedDateTime <DateTime?>]`: 
    - `[Description <String>]`: The description for the management template.
Optional.
Read-only.
    - `[DisplayName <String>]`: The display name for the management template.
Required.
Read-only.
    - `[InformationLinks <IMicrosoftGraphActionUrl- `[]`>]`: 
      - `[DisplayName <String>]`: Brief title for the page that the links directs to.
      - `[Url <String>]`: The URL to the documentation or Microsoft Entra admin center page.
    - `[LastActionByUserId <String>]`: 
    - `[LastActionDateTime <DateTime?>]`: 
    - `[ManagementTemplateCollections <IMicrosoftGraphManagedTenantsManagementTemplateCollection- `[]`>]`: 
    - `[ManagementTemplateSteps <IMicrosoftGraphManagedTenantsManagementTemplateStep- `[]`>]`: 
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AcceptedVersion <IMicrosoftGraphManagedTenantsManagementTemplateStepVersion>]`: managementTemplateStepVersion
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[AcceptedFor <IMicrosoftGraphManagedTenantsManagementTemplateStep>]`: managementTemplateStep
        - `[ContentMarkdown <String>]`: 
        - `[CreatedByUserId <String>]`: 
        - `[CreatedDateTime <DateTime?>]`: 
        - `[Deployments <IMicrosoftGraphManagedTenantsManagementTemplateStepDeployment- `[]`>]`: 
          - `[Id <String>]`: The unique identifier for an entity.
Read-only.
          - `[CreatedByUserId <String>]`: 
          - `[CreatedDateTime <DateTime?>]`: 
          - `[Error <IMicrosoftGraphManagedTenantsGraphApiErrorDetails>]`: graphAPIErrorDetails
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
            - `[Code <String>]`: 
            - `[Message <String>]`: 
          - `[LastActionByUserId <String>]`: 
          - `[LastActionDateTime <DateTime?>]`: 
          - `[Status <String>]`: managementTemplateDeploymentStatus
          - `[TemplateStepVersion <IMicrosoftGraphManagedTenantsManagementTemplateStepVersion>]`: managementTemplateStepVersion
          - `[TenantId <String>]`: 
        - `[LastActionByUserId <String>]`: 
        - `[LastActionDateTime <DateTime?>]`: 
        - `[Name <String>]`: 
        - `[TemplateStep <IMicrosoftGraphManagedTenantsManagementTemplateStep>]`: managementTemplateStep
        - `[Version <Int32?>]`: 
        - `[VersionInformation <String>]`: 
      - `[Category <String>]`: managementCategory
      - `[CreatedByUserId <String>]`: 
      - `[CreatedDateTime <DateTime?>]`: 
      - `[Description <String>]`: 
      - `[DisplayName <String>]`: 
      - `[InformationLinks <IMicrosoftGraphActionUrl- `[]`>]`: 
      - `[LastActionByUserId <String>]`: 
      - `[LastActionDateTime <DateTime?>]`: 
      - `[ManagementTemplate <IMicrosoftGraphManagedTenantsManagementTemplate>]`: managementTemplate
      - `[PortalLink <IMicrosoftGraphActionUrl>]`: actionUrl
      - `[Priority <Int32?>]`: 
      - `[UserImpact <String>]`: 
      - `[Versions <IMicrosoftGraphManagedTenantsManagementTemplateStepVersion- `[]`>]`: 
    - `[Parameters <IMicrosoftGraphManagedTenantsTemplateParameter- `[]`>]`: The collection of parameters used by the management template.
Optional.
Read-only.
      - `[Description <String>]`: The description for the template parameter.
Optional.
Read-only.
      - `[DisplayName <String>]`: The display name for the template parameter.
Required.
Read-only.
      - `[JsonAllowedValues <String>]`: The allowed values for the template parameter represented by a serialized string of JSON.
Optional.
Read-only.
      - `[JsonDefaultValue <String>]`: The default value for the template parameter represented by a serialized string of JSON.
Required.
Read-only.
      - `[ValueType <String>]`: managementParameterValueType
    - `[Priority <Int32?>]`: 
    - `[Provider <String>]`: managementProvider
    - `[UserImpact <String>]`: 
    - `[Version <Int32?>]`: 
    - `[WorkloadActions <IMicrosoftGraphManagedTenantsWorkloadAction- `[]`>]`: The collection of workload actions associated with the management template.
Optional.
Read-only.
      - `[ActionId <String>]`: The unique identifier for the workload action.
Required.
Read-only.
      - `[Category <String>]`: workloadActionCategory
      - `[Description <String>]`: The description for the workload action.
Optional.
Read-only.
      - `[DisplayName <String>]`: The display name for the workload action.
Optional.
Read-only.
      - `[Licenses <String- `[]`>]`: 
      - `[Service <String>]`: The service associated with workload action.
Optional.
Read-only.
      - `[Settings <IMicrosoftGraphManagedTenantsSetting- `[]`>]`: The collection of settings associated with the workload action.
Optional.
Read-only.
        - `[DisplayName <String>]`: The display name for the setting.
Required.
Read-only.
        - `[JsonValue <String>]`: The value for the setting serialized as string of JSON.
Required.
Read-only.
        - `[OverwriteAllowed <Boolean?>]`: A flag indicating whether the setting can be override existing configurations when applied.
Required.
Read-only.
        - `[SettingId <String>]`: 
        - `[ValueType <String>]`: managementParameterValueType

MANAGEMENTTEMPLATESTEPS `<IMicrosoftGraphManagedTenantsManagementTemplateStep- `[]`>`: .
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AcceptedVersion <IMicrosoftGraphManagedTenantsManagementTemplateStepVersion>]`: managementTemplateStepVersion
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AcceptedFor <IMicrosoftGraphManagedTenantsManagementTemplateStep>]`: managementTemplateStep
    - `[ContentMarkdown <String>]`: 
    - `[CreatedByUserId <String>]`: 
    - `[CreatedDateTime <DateTime?>]`: 
    - `[Deployments <IMicrosoftGraphManagedTenantsManagementTemplateStepDeployment- `[]`>]`: 
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[CreatedByUserId <String>]`: 
      - `[CreatedDateTime <DateTime?>]`: 
      - `[Error <IMicrosoftGraphManagedTenantsGraphApiErrorDetails>]`: graphAPIErrorDetails
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Code <String>]`: 
        - `[Message <String>]`: 
      - `[LastActionByUserId <String>]`: 
      - `[LastActionDateTime <DateTime?>]`: 
      - `[Status <String>]`: managementTemplateDeploymentStatus
      - `[TemplateStepVersion <IMicrosoftGraphManagedTenantsManagementTemplateStepVersion>]`: managementTemplateStepVersion
      - `[TenantId <String>]`: 
    - `[LastActionByUserId <String>]`: 
    - `[LastActionDateTime <DateTime?>]`: 
    - `[Name <String>]`: 
    - `[TemplateStep <IMicrosoftGraphManagedTenantsManagementTemplateStep>]`: managementTemplateStep
    - `[Version <Int32?>]`: 
    - `[VersionInformation <String>]`: 
  - `[Category <String>]`: managementCategory
  - `[CreatedByUserId <String>]`: 
  - `[CreatedDateTime <DateTime?>]`: 
  - `[Description <String>]`: 
  - `[DisplayName <String>]`: 
  - `[InformationLinks <IMicrosoftGraphActionUrl- `[]`>]`: 
    - `[DisplayName <String>]`: Brief title for the page that the links directs to.
    - `[Url <String>]`: The URL to the documentation or Microsoft Entra admin center page.
  - `[LastActionByUserId <String>]`: 
  - `[LastActionDateTime <DateTime?>]`: 
  - `[ManagementTemplate <IMicrosoftGraphManagedTenantsManagementTemplate>]`: managementTemplate
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Category <String>]`: managementCategory
    - `[CreatedByUserId <String>]`: 
    - `[CreatedDateTime <DateTime?>]`: 
    - `[Description <String>]`: The description for the management template.
Optional.
Read-only.
    - `[DisplayName <String>]`: The display name for the management template.
Required.
Read-only.
    - `[InformationLinks <IMicrosoftGraphActionUrl- `[]`>]`: 
    - `[LastActionByUserId <String>]`: 
    - `[LastActionDateTime <DateTime?>]`: 
    - `[ManagementTemplateCollections <IMicrosoftGraphManagedTenantsManagementTemplateCollection- `[]`>]`: 
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[CreatedByUserId <String>]`: 
      - `[CreatedDateTime <DateTime?>]`: 
      - `[Description <String>]`: 
      - `[DisplayName <String>]`: 
      - `[LastActionByUserId <String>]`: 
      - `[LastActionDateTime <DateTime?>]`: 
      - `[ManagementTemplates <IMicrosoftGraphManagedTenantsManagementTemplate- `[]`>]`: 
    - `[ManagementTemplateSteps <IMicrosoftGraphManagedTenantsManagementTemplateStep- `[]`>]`: 
    - `[Parameters <IMicrosoftGraphManagedTenantsTemplateParameter- `[]`>]`: The collection of parameters used by the management template.
Optional.
Read-only.
      - `[Description <String>]`: The description for the template parameter.
Optional.
Read-only.
      - `[DisplayName <String>]`: The display name for the template parameter.
Required.
Read-only.
      - `[JsonAllowedValues <String>]`: The allowed values for the template parameter represented by a serialized string of JSON.
Optional.
Read-only.
      - `[JsonDefaultValue <String>]`: The default value for the template parameter represented by a serialized string of JSON.
Required.
Read-only.
      - `[ValueType <String>]`: managementParameterValueType
    - `[Priority <Int32?>]`: 
    - `[Provider <String>]`: managementProvider
    - `[UserImpact <String>]`: 
    - `[Version <Int32?>]`: 
    - `[WorkloadActions <IMicrosoftGraphManagedTenantsWorkloadAction- `[]`>]`: The collection of workload actions associated with the management template.
Optional.
Read-only.
      - `[ActionId <String>]`: The unique identifier for the workload action.
Required.
Read-only.
      - `[Category <String>]`: workloadActionCategory
      - `[Description <String>]`: The description for the workload action.
Optional.
Read-only.
      - `[DisplayName <String>]`: The display name for the workload action.
Optional.
Read-only.
      - `[Licenses <String- `[]`>]`: 
      - `[Service <String>]`: The service associated with workload action.
Optional.
Read-only.
      - `[Settings <IMicrosoftGraphManagedTenantsSetting- `[]`>]`: The collection of settings associated with the workload action.
Optional.
Read-only.
        - `[DisplayName <String>]`: The display name for the setting.
Required.
Read-only.
        - `[JsonValue <String>]`: The value for the setting serialized as string of JSON.
Required.
Read-only.
        - `[OverwriteAllowed <Boolean?>]`: A flag indicating whether the setting can be override existing configurations when applied.
Required.
Read-only.
        - `[SettingId <String>]`: 
        - `[ValueType <String>]`: managementParameterValueType
  - `[PortalLink <IMicrosoftGraphActionUrl>]`: actionUrl
  - `[Priority <Int32?>]`: 
  - `[UserImpact <String>]`: 
  - `[Versions <IMicrosoftGraphManagedTenantsManagementTemplateStepVersion- `[]`>]`: 

PARAMETERS `<IMicrosoftGraphManagedTenantsTemplateParameter- `[]`>`: The collection of parameters used by the management template.
Optional.
Read-only.
  - `[Description <String>]`: The description for the template parameter.
Optional.
Read-only.
  - `[DisplayName <String>]`: The display name for the template parameter.
Required.
Read-only.
  - `[JsonAllowedValues <String>]`: The allowed values for the template parameter represented by a serialized string of JSON.
Optional.
Read-only.
  - `[JsonDefaultValue <String>]`: The default value for the template parameter represented by a serialized string of JSON.
Required.
Read-only.
  - `[ValueType <String>]`: managementParameterValueType

WORKLOADACTIONS `<IMicrosoftGraphManagedTenantsWorkloadAction- `[]`>`: The collection of workload actions associated with the management template.
Optional.
Read-only.
  - `[ActionId <String>]`: The unique identifier for the workload action.
Required.
Read-only.
  - `[Category <String>]`: workloadActionCategory
  - `[Description <String>]`: The description for the workload action.
Optional.
Read-only.
  - `[DisplayName <String>]`: The display name for the workload action.
Optional.
Read-only.
  - `[Licenses <String- `[]`>]`: 
  - `[Service <String>]`: The service associated with workload action.
Optional.
Read-only.
  - `[Settings <IMicrosoftGraphManagedTenantsSetting- `[]`>]`: The collection of settings associated with the workload action.
Optional.
Read-only.
    - `[DisplayName <String>]`: The display name for the setting.
Required.
Read-only.
    - `[JsonValue <String>]`: The value for the setting serialized as string of JSON.
Required.
Read-only.
    - `[OverwriteAllowed <Boolean?>]`: A flag indicating whether the setting can be override existing configurations when applied.
Required.
Read-only.
    - `[SettingId <String>]`: 
    - `[ValueType <String>]`: managementParameterValueType

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.managedtenants/new-mgbetatenantrelationshipmanagedtenantmanagementtemplate](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.managedtenants/new-mgbetatenantrelationshipmanagedtenantmanagementtemplate)
























