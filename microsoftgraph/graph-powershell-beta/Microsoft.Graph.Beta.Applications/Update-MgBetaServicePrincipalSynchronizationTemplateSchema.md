---
external help file: Microsoft.Graph.Beta.Applications-help.xml
Module Name: Microsoft.Graph.Beta.Applications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/update-mgbetaserviceprincipalsynchronizationtemplateschema
schema: 2.0.0
---

# Update-MgBetaServicePrincipalSynchronizationTemplateSchema

## SYNOPSIS
Update the navigation property schema in servicePrincipals

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgServicePrincipalSynchronizationTemplateSchema](/powershell/module/Microsoft.Graph.Applications/Update-MgServicePrincipalSynchronizationTemplateSchema?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaServicePrincipalSynchronizationTemplateSchema -ServicePrincipalId <String>
 -SynchronizationTemplateId <String> [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Directories <IMicrosoftGraphDirectoryDefinition[]>] [-Id <String>]
 [-SynchronizationRules <IMicrosoftGraphSynchronizationRule[]>] [-Version <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaServicePrincipalSynchronizationTemplateSchema -ServicePrincipalId <String>
 -SynchronizationTemplateId <String> -BodyParameter <IMicrosoftGraphSynchronizationSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaServicePrincipalSynchronizationTemplateSchema -InputObject <IApplicationsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Directories <IMicrosoftGraphDirectoryDefinition[]>] [-Id <String>]
 [-SynchronizationRules <IMicrosoftGraphSynchronizationRule[]>] [-Version <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaServicePrincipalSynchronizationTemplateSchema -InputObject <IApplicationsIdentity>
 -BodyParameter <IMicrosoftGraphSynchronizationSchema> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property schema in servicePrincipals

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

### -BodyParameter
synchronizationSchema
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphSynchronizationSchema
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

### -Directories
Contains the collection of directories and all of their objects.
To construct, see NOTES section for DIRECTORIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphDirectoryDefinition[]
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
Type: IApplicationsIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

### -ServicePrincipalId
The unique identifier of servicePrincipal

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

### -SynchronizationRules
A collection of synchronization rules configured for the synchronizationJob or synchronizationTemplate.
To construct, see NOTES section for SYNCHRONIZATIONRULES properties and create a hash table.

```yaml
Type: IMicrosoftGraphSynchronizationRule[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SynchronizationTemplateId
The unique identifier of synchronizationTemplate

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

### -Version
The version of the schema, updated automatically with every schema change.

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

### Microsoft.Graph.Beta.PowerShell.Models.IApplicationsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSynchronizationSchema
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSynchronizationSchema
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphSynchronizationSchema>`: synchronizationSchema
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Directories <IMicrosoftGraphDirectoryDefinition- `[]`>]`: Contains the collection of directories and all of their objects.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Discoverabilities <String>]`: directoryDefinitionDiscoverabilities
    - `[DiscoveryDateTime <DateTime?>]`: Represents the discovery date and time using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[Name <String>]`: Name of the directory.
Must be unique within the synchronization schema.
Not nullable.
    - `[Objects <IMicrosoftGraphObjectDefinition- `[]`>]`: Collection of objects supported by the directory.
      - `[Attributes <IMicrosoftGraphAttributeDefinition- `[]`>]`: Defines attributes of the object.
        - `[Anchor <Boolean?>]`: true if the attribute should be used as the anchor for the object.
Anchor attributes must have a unique value identifying an object, and must be immutable.
Default is false.
One, and only one, of the object's attributes must be designated as the anchor to support synchronization.
        - `[ApiExpressions <IMicrosoftGraphStringKeyStringValuePair- `[]`>]`: 
          - `[Key <String>]`: Key.
          - `[Value <String>]`: Value.
        - `[CaseExact <Boolean?>]`: true if value of this attribute should be treated as case-sensitive.
This setting affects how the synchronization engine detects changes for the attribute.
        - `[DefaultValue <String>]`: The default value of the attribute.
        - `[FlowNullValues <Boolean?>]`: 'true' to allow null values for attributes.
        - `[Metadata <IMicrosoftGraphAttributeDefinitionMetadataEntry- `[]`>]`: Metadata for the given object.
          - `[Key <String>]`: attributeDefinitionMetadata
          - `[Value <String>]`: Value of the metadata property.
        - `[Multivalued <Boolean?>]`: true if an attribute can have multiple values.
Default is false.
        - `[Mutability <String>]`: mutability
        - `[Name <String>]`: Name of the attribute.
Must be unique within the object definition.
Not nullable.
        - `[ReferencedObjects <IMicrosoftGraphReferencedObject- `[]`>]`: For attributes with reference type, lists referenced objects (for example, the manager attribute would list User as the referenced object).
          - `[ReferencedObjectName <String>]`: Name of the referenced object.
Must match one of the objects in the directory definition.
          - `[ReferencedProperty <String>]`: Currently not supported.
Name of the property in the referenced object, the value for which is used as the reference.
        - `[Required <Boolean?>]`: true if attribute is required.
Object can not be created if any of the required attributes are missing.
If during synchronization, the required attribute has no value, the default value will be used.
If default the value was not set, synchronization will record an error.
        - `[Type <String>]`: attributeType
      - `[Metadata <IMicrosoftGraphObjectDefinitionMetadataEntry- `[]`>]`: Metadata for the given object.
        - `[Key <String>]`: objectDefinitionMetadata
        - `[Value <String>]`: Value of the metadata property.
      - `[Name <String>]`: Name of the object.
Must be unique within a directory definition.
Not nullable.
      - `[SupportedApis <String- `[]`>]`: The API that the provisioning service queries to retrieve data for synchronization.
    - `[ReadOnly <Boolean?>]`: Whether this object is read-only.
    - `[Version <String>]`: Read only value that indicates version discovered.
null if discovery hasn't yet occurred.
  - `[SynchronizationRules <IMicrosoftGraphSynchronizationRule- `[]`>]`: A collection of synchronization rules configured for the synchronizationJob or synchronizationTemplate.
    - `[ContainerFilter <IMicrosoftGraphContainerFilter>]`: containerFilter
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IncludedContainers <String- `[]`>]`: The identifiers of containers, such as organizational units, that are in scope for a synchronization rule.
For Active Directory organizational units, use the distinguished names.
An empty list means no container filtering is configured.
    - `[Editable <Boolean?>]`: true if the synchronization rule can be customized; false if this rule is read-only and shouldn't be changed.
    - `[GroupFilter <IMicrosoftGraphGroupFilter>]`: groupFilter
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IncludedGroups <String- `[]`>]`: Identifiers of groups that are in scope for a synchronization rule.
For Active Directory groups, use the distinguished names.
An empty list means no group filtering is configured.
    - `[Id <String>]`: Synchronization rule identifier.
Must be one of the identifiers recognized by the synchronization engine.
Supported rule identifiers can be found in the synchronization template returned by the API.
    - `[Metadata <IMicrosoftGraphStringKeyStringValuePair- `[]`>]`: Additional extension properties.
Unless instructed explicitly by the support team, metadata values shouldn't be changed.
    - `[Name <String>]`: Human-readable name of the synchronization rule.
Not nullable.
    - `[ObjectMappings <IMicrosoftGraphObjectMapping- `[]`>]`: Collection of object mappings supported by the rule.
Tells the synchronization engine which objects should be synchronized.
      - `[AttributeMappings <IMicrosoftGraphAttributeMapping- `[]`>]`: Attribute mappings define which attributes to map from the source object into the target object and how they should flow.
A number of functions are available to support the transformation of the original source values.
        - `[DefaultValue <String>]`: Default value to be used in case the source property was evaluated to null.
Optional.
        - `[ExportMissingReferences <Boolean?>]`: For internal use only.
        - `[FlowBehavior <String>]`: attributeFlowBehavior
        - `[FlowType <String>]`: attributeFlowType
        - `[MatchingPriority <Int32?>]`: If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.
The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.
If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.
Only attributes that are expected to have unique values, such as email, should be used as matching attributes.
        - `[Source <IMicrosoftGraphAttributeMappingSource>]`: attributeMappingSource
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Expression <String>]`: Equivalent expression representation of this attributeMappingSource object.
          - `[Name <String>]`: Name parameter of the mapping source.
Depending on the type property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.
          - `[Parameters <IMicrosoftGraphStringKeyAttributeMappingSourceValuePair- `[]`>]`: If this object represents a function, lists function parameters.
Parameters consist of attributeMappingSource objects themselves, allowing for complex expressions.
If type isn't Function, this property is null/empty array.
            - `[Key <String>]`: The name of the parameter.
            - `[Value <IMicrosoftGraphAttributeMappingSource>]`: attributeMappingSource
          - `[Type <String>]`: attributeMappingSourceType
        - `[TargetAttributeName <String>]`: Name of the attribute on the target object.
      - `[Enabled <Boolean?>]`: When true, this object mapping will be processed during synchronization.
When false, this object mapping will be skipped.
      - `[FlowTypes <String>]`: objectFlowTypes
      - `[Metadata <IMicrosoftGraphObjectMappingMetadataEntry- `[]`>]`: Additional extension properties.
Unless mentioned explicitly, metadata values should not be changed.
        - `[Key <String>]`: objectMappingMetadata
        - `[Value <String>]`: Value of the metadata property.
      - `[Name <String>]`: Human-friendly name of the object mapping.
      - `[Scope <IMicrosoftGraphFilter>]`: filter
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[CategoryFilterGroups <IMicrosoftGraphFilterGroup- `[]`>]`: *Experimental* Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.
An object is considered in scope if ANY of the groups in the collection is evaluated to true.
          - `[Clauses <IMicrosoftGraphFilterClause- `[]`>]`: Filter clauses (conditions) of this group.
All clauses in a group must be satisfied in order for the filter group to evaluate to true.
            - `[OperatorName <String>]`: Name of the operator to be applied to the source and target operands.
Must be one of the supported operators.
Supported operators can be discovered.
            - `[SourceOperandName <String>]`: Name of source operand (the operand being tested).
The source operand name must match one of the attribute names on the source object.
            - `[TargetOperand <IMicrosoftGraphFilterOperand>]`: filterOperand
              - `[(Any) <Object>]`: This indicates any property can be added to this object.
              - `[Values <String- `[]`>]`: Collection of values.
          - `[Name <String>]`: Human-readable name of the filter group.
        - `[Groups <IMicrosoftGraphFilterGroup- `[]`>]`: Filter group set used to decide whether given object is in scope for provisioning.
This is the filter which should be used in most cases.
If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter isn't satisfied any longer, such object will get de-provisioned'.
An object is considered in scope if ANY of the groups in the collection is evaluated to true.
        - `[InputFilterGroups <IMicrosoftGraphFilterGroup- `[]`>]`: *Experimental* Filter group set used to filter out objects at the early stage of reading them from the directory.
If an object doesn't satisfy this filter, it will not be processed further.
Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object will NOT get de-provisioned.
An object is considered in scope if ANY of the groups in the collection is evaluated to true.
      - `[SourceObjectName <String>]`: Name of the object in the source directory.
Must match the object name from the source directory definition.
      - `[TargetObjectName <String>]`: Name of the object in target directory.
Must match the object name from the target directory definition.
    - `[Priority <Int32?>]`: Priority relative to other rules in the synchronizationSchema.
Rules with the lowest priority number will be processed first.
    - `[SourceDirectoryName <String>]`: Name of the source directory.
Must match one of the directory definitions in synchronizationSchema.
    - `[TargetDirectoryName <String>]`: Name of the target directory.
Must match one of the directory definitions in synchronizationSchema.
  - `[Version <String>]`: The version of the schema, updated automatically with every schema change.

DIRECTORIES `<IMicrosoftGraphDirectoryDefinition- `[]`>`: Contains the collection of directories and all of their objects.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Discoverabilities <String>]`: directoryDefinitionDiscoverabilities
  - `[DiscoveryDateTime <DateTime?>]`: Represents the discovery date and time using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[Name <String>]`: Name of the directory.
Must be unique within the synchronization schema.
Not nullable.
  - `[Objects <IMicrosoftGraphObjectDefinition- `[]`>]`: Collection of objects supported by the directory.
    - `[Attributes <IMicrosoftGraphAttributeDefinition- `[]`>]`: Defines attributes of the object.
      - `[Anchor <Boolean?>]`: true if the attribute should be used as the anchor for the object.
Anchor attributes must have a unique value identifying an object, and must be immutable.
Default is false.
One, and only one, of the object's attributes must be designated as the anchor to support synchronization.
      - `[ApiExpressions <IMicrosoftGraphStringKeyStringValuePair- `[]`>]`: 
        - `[Key <String>]`: Key.
        - `[Value <String>]`: Value.
      - `[CaseExact <Boolean?>]`: true if value of this attribute should be treated as case-sensitive.
This setting affects how the synchronization engine detects changes for the attribute.
      - `[DefaultValue <String>]`: The default value of the attribute.
      - `[FlowNullValues <Boolean?>]`: 'true' to allow null values for attributes.
      - `[Metadata <IMicrosoftGraphAttributeDefinitionMetadataEntry- `[]`>]`: Metadata for the given object.
        - `[Key <String>]`: attributeDefinitionMetadata
        - `[Value <String>]`: Value of the metadata property.
      - `[Multivalued <Boolean?>]`: true if an attribute can have multiple values.
Default is false.
      - `[Mutability <String>]`: mutability
      - `[Name <String>]`: Name of the attribute.
Must be unique within the object definition.
Not nullable.
      - `[ReferencedObjects <IMicrosoftGraphReferencedObject- `[]`>]`: For attributes with reference type, lists referenced objects (for example, the manager attribute would list User as the referenced object).
        - `[ReferencedObjectName <String>]`: Name of the referenced object.
Must match one of the objects in the directory definition.
        - `[ReferencedProperty <String>]`: Currently not supported.
Name of the property in the referenced object, the value for which is used as the reference.
      - `[Required <Boolean?>]`: true if attribute is required.
Object can not be created if any of the required attributes are missing.
If during synchronization, the required attribute has no value, the default value will be used.
If default the value was not set, synchronization will record an error.
      - `[Type <String>]`: attributeType
    - `[Metadata <IMicrosoftGraphObjectDefinitionMetadataEntry- `[]`>]`: Metadata for the given object.
      - `[Key <String>]`: objectDefinitionMetadata
      - `[Value <String>]`: Value of the metadata property.
    - `[Name <String>]`: Name of the object.
Must be unique within a directory definition.
Not nullable.
    - `[SupportedApis <String- `[]`>]`: The API that the provisioning service queries to retrieve data for synchronization.
  - `[ReadOnly <Boolean?>]`: Whether this object is read-only.
  - `[Version <String>]`: Read only value that indicates version discovered.
null if discovery hasn't yet occurred.

INPUTOBJECT `<IApplicationsIdentity>`: Identity Parameter
  - `[AppId <String>]`: Alternate key of application
  - `[AppManagementPolicyId <String>]`: The unique identifier of appManagementPolicy
  - `[AppRoleAssignmentId <String>]`: The unique identifier of appRoleAssignment
  - `[ApplicationId <String>]`: The unique identifier of application
  - `[ApplicationTemplateId <String>]`: The unique identifier of applicationTemplate
  - `[ClaimsMappingPolicyId <String>]`: The unique identifier of claimsMappingPolicy
  - `[ConnectorGroupId <String>]`: The unique identifier of connectorGroup
  - `[ConnectorId <String>]`: The unique identifier of connector
  - `[DelegatedPermissionClassificationId <String>]`: The unique identifier of delegatedPermissionClassification
  - `[DirectoryDefinitionId <String>]`: The unique identifier of directoryDefinition
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[EndpointId <String>]`: The unique identifier of endpoint
  - `[ExtensionPropertyId <String>]`: The unique identifier of extensionProperty
  - `[FederatedIdentityCredentialId <String>]`: The unique identifier of federatedIdentityCredential
  - `[GroupId <String>]`: The unique identifier of group
  - `[HomeRealmDiscoveryPolicyId <String>]`: The unique identifier of homeRealmDiscoveryPolicy
  - `[IPApplicationSegmentId <String>]`: The unique identifier of ipApplicationSegment
  - `[LicenseDetailsId <String>]`: The unique identifier of licenseDetails
  - `[Name <String>]`: Alternate key of federatedIdentityCredential
  - `[OAuth2PermissionGrantId <String>]`: The unique identifier of oAuth2PermissionGrant
  - `[OnPremisesAgentGroupId <String>]`: The unique identifier of onPremisesAgentGroup
  - `[OnPremisesAgentGroupId1 <String>]`: The unique identifier of onPremisesAgentGroup
  - `[OnPremisesAgentId <String>]`: The unique identifier of onPremisesAgent
  - `[OnPremisesPublishingProfileId <String>]`: The unique identifier of onPremisesPublishingProfile
  - `[PermissionGrantPreApprovalPolicyId <String>]`: The unique identifier of permissionGrantPreApprovalPolicy
  - `[PublishedResourceId <String>]`: The unique identifier of publishedResource
  - `[ServicePrincipalId <String>]`: The unique identifier of servicePrincipal
  - `[SynchronizationJobId <String>]`: The unique identifier of synchronizationJob
  - `[SynchronizationTemplateId <String>]`: The unique identifier of synchronizationTemplate
  - `[TargetDeviceGroupId <String>]`: The unique identifier of targetDeviceGroup
  - `[TokenIssuancePolicyId <String>]`: The unique identifier of tokenIssuancePolicy
  - `[TokenLifetimePolicyId <String>]`: The unique identifier of tokenLifetimePolicy
  - `[UniqueName <String>]`: Alternate key of application
  - `[UserId <String>]`: The unique identifier of user

SYNCHRONIZATIONRULES `<IMicrosoftGraphSynchronizationRule- `[]`>`: A collection of synchronization rules configured for the synchronizationJob or synchronizationTemplate.
  - `[ContainerFilter <IMicrosoftGraphContainerFilter>]`: containerFilter
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IncludedContainers <String- `[]`>]`: The identifiers of containers, such as organizational units, that are in scope for a synchronization rule.
For Active Directory organizational units, use the distinguished names.
An empty list means no container filtering is configured.
  - `[Editable <Boolean?>]`: true if the synchronization rule can be customized; false if this rule is read-only and shouldn't be changed.
  - `[GroupFilter <IMicrosoftGraphGroupFilter>]`: groupFilter
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IncludedGroups <String- `[]`>]`: Identifiers of groups that are in scope for a synchronization rule.
For Active Directory groups, use the distinguished names.
An empty list means no group filtering is configured.
  - `[Id <String>]`: Synchronization rule identifier.
Must be one of the identifiers recognized by the synchronization engine.
Supported rule identifiers can be found in the synchronization template returned by the API.
  - `[Metadata <IMicrosoftGraphStringKeyStringValuePair- `[]`>]`: Additional extension properties.
Unless instructed explicitly by the support team, metadata values shouldn't be changed.
    - `[Key <String>]`: Key.
    - `[Value <String>]`: Value.
  - `[Name <String>]`: Human-readable name of the synchronization rule.
Not nullable.
  - `[ObjectMappings <IMicrosoftGraphObjectMapping- `[]`>]`: Collection of object mappings supported by the rule.
Tells the synchronization engine which objects should be synchronized.
    - `[AttributeMappings <IMicrosoftGraphAttributeMapping- `[]`>]`: Attribute mappings define which attributes to map from the source object into the target object and how they should flow.
A number of functions are available to support the transformation of the original source values.
      - `[DefaultValue <String>]`: Default value to be used in case the source property was evaluated to null.
Optional.
      - `[ExportMissingReferences <Boolean?>]`: For internal use only.
      - `[FlowBehavior <String>]`: attributeFlowBehavior
      - `[FlowType <String>]`: attributeFlowType
      - `[MatchingPriority <Int32?>]`: If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.
The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.
If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.
Only attributes that are expected to have unique values, such as email, should be used as matching attributes.
      - `[Source <IMicrosoftGraphAttributeMappingSource>]`: attributeMappingSource
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Expression <String>]`: Equivalent expression representation of this attributeMappingSource object.
        - `[Name <String>]`: Name parameter of the mapping source.
Depending on the type property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.
        - `[Parameters <IMicrosoftGraphStringKeyAttributeMappingSourceValuePair- `[]`>]`: If this object represents a function, lists function parameters.
Parameters consist of attributeMappingSource objects themselves, allowing for complex expressions.
If type isn't Function, this property is null/empty array.
          - `[Key <String>]`: The name of the parameter.
          - `[Value <IMicrosoftGraphAttributeMappingSource>]`: attributeMappingSource
        - `[Type <String>]`: attributeMappingSourceType
      - `[TargetAttributeName <String>]`: Name of the attribute on the target object.
    - `[Enabled <Boolean?>]`: When true, this object mapping will be processed during synchronization.
When false, this object mapping will be skipped.
    - `[FlowTypes <String>]`: objectFlowTypes
    - `[Metadata <IMicrosoftGraphObjectMappingMetadataEntry- `[]`>]`: Additional extension properties.
Unless mentioned explicitly, metadata values should not be changed.
      - `[Key <String>]`: objectMappingMetadata
      - `[Value <String>]`: Value of the metadata property.
    - `[Name <String>]`: Human-friendly name of the object mapping.
    - `[Scope <IMicrosoftGraphFilter>]`: filter
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[CategoryFilterGroups <IMicrosoftGraphFilterGroup- `[]`>]`: *Experimental* Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.
An object is considered in scope if ANY of the groups in the collection is evaluated to true.
        - `[Clauses <IMicrosoftGraphFilterClause- `[]`>]`: Filter clauses (conditions) of this group.
All clauses in a group must be satisfied in order for the filter group to evaluate to true.
          - `[OperatorName <String>]`: Name of the operator to be applied to the source and target operands.
Must be one of the supported operators.
Supported operators can be discovered.
          - `[SourceOperandName <String>]`: Name of source operand (the operand being tested).
The source operand name must match one of the attribute names on the source object.
          - `[TargetOperand <IMicrosoftGraphFilterOperand>]`: filterOperand
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
            - `[Values <String- `[]`>]`: Collection of values.
        - `[Name <String>]`: Human-readable name of the filter group.
      - `[Groups <IMicrosoftGraphFilterGroup- `[]`>]`: Filter group set used to decide whether given object is in scope for provisioning.
This is the filter which should be used in most cases.
If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter isn't satisfied any longer, such object will get de-provisioned'.
An object is considered in scope if ANY of the groups in the collection is evaluated to true.
      - `[InputFilterGroups <IMicrosoftGraphFilterGroup- `[]`>]`: *Experimental* Filter group set used to filter out objects at the early stage of reading them from the directory.
If an object doesn't satisfy this filter, it will not be processed further.
Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object will NOT get de-provisioned.
An object is considered in scope if ANY of the groups in the collection is evaluated to true.
    - `[SourceObjectName <String>]`: Name of the object in the source directory.
Must match the object name from the source directory definition.
    - `[TargetObjectName <String>]`: Name of the object in target directory.
Must match the object name from the target directory definition.
  - `[Priority <Int32?>]`: Priority relative to other rules in the synchronizationSchema.
Rules with the lowest priority number will be processed first.
  - `[SourceDirectoryName <String>]`: Name of the source directory.
Must match one of the directory definitions in synchronizationSchema.
  - `[TargetDirectoryName <String>]`: Name of the target directory.
Must match one of the directory definitions in synchronizationSchema.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/update-mgbetaserviceprincipalsynchronizationtemplateschema](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/update-mgbetaserviceprincipalsynchronizationtemplateschema)
























