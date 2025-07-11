---
external help file: Microsoft.Graph.Beta.NetworkAccess-help.xml
Module Name: Microsoft.Graph.Beta.NetworkAccess
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.networkaccess/update-mgbetanetworkaccessconnectivitybranchforwardingprofile
schema: 2.0.0
---

# Update-MgBetaNetworkAccessConnectivityBranchForwardingProfile

## SYNOPSIS
Update the navigation property forwardingProfiles in networkAccess

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaNetworkAccessConnectivityBranchForwardingProfile -BranchSiteId <String>
 -ForwardingProfileId <String> [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Associations <IMicrosoftGraphNetworkaccessAssociation[]>] [-Description <String>] [-Id <String>]
 [-LastModifiedDateTime <DateTime>] [-Name <String>] [-Policies <IMicrosoftGraphNetworkaccessPolicyLink[]>]
 [-Priority <Int32>] [-ServicePrincipal <IMicrosoftGraphServicePrincipal>] [-State <String>]
 [-TrafficForwardingType <String>] [-Version <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaNetworkAccessConnectivityBranchForwardingProfile -BranchSiteId <String>
 -ForwardingProfileId <String> -BodyParameter <IMicrosoftGraphNetworkaccessForwardingProfile>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaNetworkAccessConnectivityBranchForwardingProfile -InputObject <INetworkAccessIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Associations <IMicrosoftGraphNetworkaccessAssociation[]>] [-Description <String>] [-Id <String>]
 [-LastModifiedDateTime <DateTime>] [-Name <String>] [-Policies <IMicrosoftGraphNetworkaccessPolicyLink[]>]
 [-Priority <Int32>] [-ServicePrincipal <IMicrosoftGraphServicePrincipal>] [-State <String>]
 [-TrafficForwardingType <String>] [-Version <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaNetworkAccessConnectivityBranchForwardingProfile -InputObject <INetworkAccessIdentity>
 -BodyParameter <IMicrosoftGraphNetworkaccessForwardingProfile> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property forwardingProfiles in networkAccess

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

### -Associations
Specifies the users, groups, devices, and remote networks whose traffic is associated with the given traffic forwarding profile.

```yaml
Type: IMicrosoftGraphNetworkaccessAssociation[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
forwardingProfile
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphNetworkaccessForwardingProfile
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -BranchSiteId
The unique identifier of branchSite

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

### -Description
Description.

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

### -ForwardingProfileId
The unique identifier of forwardingProfile

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
Type: INetworkAccessIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -LastModifiedDateTime
The date and time when the profile was last modified.

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

### -Name
The name of the profile.

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

### -Policies
The traffic forwarding policies associated with this profile.
To construct, see NOTES section for POLICIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphNetworkaccessPolicyLink[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Priority
Profile priority.

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

### -ServicePrincipal
servicePrincipal
To construct, see NOTES section for SERVICEPRINCIPAL properties and create a hash table.

```yaml
Type: IMicrosoftGraphServicePrincipal
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -State
status

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

### -TrafficForwardingType
trafficForwardingType

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

### -Version
Profile version.

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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphNetworkaccessForwardingProfile
### Microsoft.Graph.Beta.PowerShell.Models.INetworkAccessIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphNetworkaccessForwardingProfile
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphNetworkaccessForwardingProfile>`: forwardingProfile
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Description <String>]`: Description.
  - `[LastModifiedDateTime <DateTime?>]`: The date and time when the profile was last modified.
  - `[Name <String>]`: The name of the profile.
  - `[Policies <IMicrosoftGraphNetworkaccessPolicyLink- `[]`>]`: The traffic forwarding policies associated with this profile.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Policy <IMicrosoftGraphNetworkaccessPolicy>]`: policy
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Description <String>]`: Description.
      - `[Name <String>]`: Policy name.
      - `[PolicyRules <IMicrosoftGraphNetworkaccessPolicyRule- `[]`>]`: Represents the definition of the policy ruleset that makes up the core definition of a policy.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[Name <String>]`: Name.
      - `[Version <String>]`: Version.
    - `[State <String>]`: status
    - `[Version <String>]`: Version.
  - `[State <String>]`: status
  - `[Version <String>]`: Profile version.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Associations <IMicrosoftGraphNetworkaccessAssociation- `[]`>]`: Specifies the users, groups, devices, and remote networks whose traffic is associated with the given traffic forwarding profile.
  - `[Priority <Int32?>]`: Profile priority.
  - `[ServicePrincipal <IMicrosoftGraphServicePrincipal>]`: servicePrincipal
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AccountEnabled <Boolean?>]`: true if the service principal account is enabled; otherwise, false.
If set to false, then no users are able to sign in to this app, even if they're assigned to it.
Supports $filter (eq, ne, not, in).
    - `[AddIns <IMicrosoftGraphAddIn- `[]`>]`: Defines custom behavior that a consuming service can use to call an app in specific contexts.
For example, applications that can render file streams may set the addIns property for its 'FileHandler' functionality.
This lets services like Microsoft 365 call the application in the context of a document the user is working on.
      - `[Id <String>]`: The unique identifier for the addIn object.
      - `[Properties <IMicrosoftGraphKeyValue- `[]`>]`: The collection of key-value pairs that define parameters that the consuming service can use or call.
You must specify this property when performing a POST or a PATCH operation on the addIns collection.
Required.
        - `[Key <String>]`: Key.
        - `[Value <String>]`: Value.
      - `[Type <String>]`: The unique name for the functionality exposed by the app.
    - `[AlternativeNames <String- `[]`>]`: Used to retrieve service principals by subscription, identify resource group and full resource IDs for managed identities.
Supports $filter (eq, not, ge, le, startsWith).
    - `[AppDescription <String>]`: The description exposed by the associated application.
    - `[AppDisplayName <String>]`: The display name exposed by the associated application.
Maximum length is 256 characters.
    - `[AppId <String>]`: The unique identifier for the associated application (its appId property).
Alternate key.
Supports $filter (eq, ne, not, in, startsWith).
    - `[AppManagementPolicies <IMicrosoftGraphAppManagementPolicy- `[]`>]`: The appManagementPolicy applied to this service principal.
      - `[Description <String>]`: Description for this policy.
Required.
      - `[DisplayName <String>]`: Display name for this policy.
Required.
      - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AppliesTo <IMicrosoftGraphDirectoryObject- `[]`>]`: Collection of application and service principals to which a policy is applied.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
      - `[IsEnabled <Boolean?>]`: Denotes whether the policy is enabled.
      - `[Restrictions <IMicrosoftGraphCustomAppManagementConfiguration>]`: customAppManagementConfiguration
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[KeyCredentials <IMicrosoftGraphKeyCredentialConfiguration- `[]`>]`: 
          - `[CertificateBasedApplicationConfigurationIds <String- `[]`>]`: Collection of GUIDs that represent certificateBasedApplicationConfiguration that is allowed as root and intermediate certificate authorities.
          - `[MaxLifetime <TimeSpan?>]`: String value that indicates the maximum lifetime for key expiration, defined as an ISO 8601 duration.
For example, P4DT12H30M5S represents four days, 12 hours, 30 minutes, and five seconds.
This property is required when restrictionType is set to keyLifetime.
          - `[RestrictForAppsCreatedAfterDateTime <DateTime?>]`: Specifies the date from which the policy restriction applies to newly created applications.
For existing applications, the enforcement date can be retroactively applied.
          - `[RestrictionType <String>]`: appKeyCredentialRestrictionType
          - `[State <String>]`: appManagementRestrictionState
        - `[PasswordCredentials <IMicrosoftGraphPasswordCredentialConfiguration- `[]`>]`: 
          - `[MaxLifetime <TimeSpan?>]`: String value that indicates the maximum lifetime for password expiration, defined as an ISO 8601 duration.
For example, P4DT12H30M5S represents four days, 12 hours, 30 minutes, and five seconds.
This property is required when restrictionType is set to passwordLifetime.
          - `[RestrictForAppsCreatedAfterDateTime <DateTime?>]`: Specifies the date from which the policy restriction applies to newly created applications.
For existing applications, the enforcement date can be retroactively applied.
          - `[RestrictionType <String>]`: appCredentialRestrictionType
          - `[State <String>]`: appManagementRestrictionState
        - `[ApplicationRestrictions <IMicrosoftGraphCustomAppManagementApplicationConfiguration>]`: customAppManagementApplicationConfiguration
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Audiences <IMicrosoftGraphAudiencesConfiguration>]`: audiencesConfiguration
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
            - `[AzureAdMultipleOrgs <IMicrosoftGraphAudienceRestriction>]`: audienceRestriction
              - `[(Any) <Object>]`: This indicates any property can be added to this object.
              - `[ExcludeActors <IMicrosoftGraphAppManagementPolicyActorExemptions>]`: appManagementPolicyActorExemptions
                - `[(Any) <Object>]`: This indicates any property can be added to this object.
                - `[CustomSecurityAttributes <IMicrosoftGraphCustomSecurityAttributeExemption- `[]`>]`: 
                  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
                  - `[Operator <String>]`: customSecurityAttributeComparisonOperator
              - `[RestrictForAppsCreatedAfterDateTime <DateTime?>]`: Specifies the date from which the policy restriction applies to newly created applications.
For existing applications, the enforcement date can be retroactively applied.
              - `[State <String>]`: appManagementRestrictionState
            - `[PersonalMicrosoftAccount <IMicrosoftGraphAudienceRestriction>]`: audienceRestriction
          - `[IdentifierUris <IMicrosoftGraphIdentifierUriConfiguration>]`: identifierUriConfiguration
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
            - `[NonDefaultUriAddition <IMicrosoftGraphIdentifierUriRestriction>]`: identifierUriRestriction
              - `[(Any) <Object>]`: This indicates any property can be added to this object.
              - `[ExcludeActors <IMicrosoftGraphAppManagementPolicyActorExemptions>]`: appManagementPolicyActorExemptions
              - `[ExcludeAppsReceivingV2Tokens <Boolean?>]`: If true, the restriction isn't enforced for applications that are configured to receive V2 tokens in Microsoft Entra ID; else, the restriction isn't enforced for those applications.
              - `[ExcludeSaml <Boolean?>]`: If true, the restriction isn't enforced for SAML applications in Microsoft Entra ID; else, the restriction is enforced for those applications.
              - `[RestrictForAppsCreatedAfterDateTime <DateTime?>]`: Specifies the date from which the policy restriction applies to newly created applications.
For existing applications, the enforcement date can be retroactively applied.
              - `[State <String>]`: appManagementRestrictionState
    - `[AppOwnerOrganizationId <String>]`: Contains the tenant ID where the application is registered.
This is applicable only to service principals backed by applications.
Supports $filter (eq, ne, NOT, ge, le).
    - `[AppRoleAssignedTo <IMicrosoftGraphAppRoleAssignment- `[]`>]`: App role assignments for this app or service, granted to users, groups, and other service principals.Supports $expand.
      - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AppRoleId <String>]`: The identifier (id) for the app role that is assigned to the principal.
This app role must be exposed in the appRoles property on the resource application's service principal (resourceId).
If the resource application hasn't declared any app roles, a default app role ID of 00000000-0000-0000-0000-000000000000 can be specified to signal that the principal is assigned to the resource app without any specific app roles.
Required on create.
      - `[CreationTimestamp <DateTime?>]`: The time when the app role assignment was created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
      - `[PrincipalDisplayName <String>]`: The display name of the user, group, or service principal that was granted the app role assignment.
Maximum length is 256 characters.
Read-only.
Supports $filter (eq and startswith).
      - `[PrincipalId <String>]`: The unique identifier (id) for the user, security group, or service principal being granted the app role.
Security groups with dynamic memberships are supported.
Required on create.
      - `[PrincipalType <String>]`: The type of the assigned principal.
This can either be User, Group, or ServicePrincipal.
Read-only.
      - `[ResourceDisplayName <String>]`: The display name of the resource app's service principal to which the assignment is made.
Maximum length is 256 characters.
      - `[ResourceId <String>]`: The unique identifier (id) for the resource service principal for which the assignment is made.
Required on create.
Supports $filter (eq only).
    - `[AppRoleAssignmentRequired <Boolean?>]`: Specifies whether users or other service principals need to be granted an app role assignment for this service principal before users can sign in or apps can get tokens.
The default value is false.
Not nullable.
Supports $filter (eq, ne, NOT).
    - `[AppRoleAssignments <IMicrosoftGraphAppRoleAssignment- `[]`>]`: App role assignment for another app or service, granted to this service principal.
Supports $expand.
    - `[AppRoles <IMicrosoftGraphAppRole- `[]`>]`: The roles exposed by the application, which this service principal represents.
For more information, see the appRoles property definition on the application entity.
Not nullable.
      - `[AllowedMemberTypes <String- `[]`>]`: Specifies whether this app role can be assigned to users and groups (by setting to - `['User']`), to other application's (by setting to - `['Application']`, or both (by setting to - `['User', 'Application']`).
App roles supporting assignment to other applications' service principals are also known as application permissions.
The 'Application' value is only supported for app roles defined on application entities.
      - `[Description <String>]`: The description for the app role.
This is displayed when the app role is being assigned and, if the app role functions as an application permission, during  consent experiences.
      - `[DisplayName <String>]`: Display name for the permission that appears in the app role assignment and consent experiences.
      - `[Id <String>]`: Unique role identifier inside the appRoles collection.
You must specify a new GUID identifier when you create a new app role.
      - `[IsEnabled <Boolean?>]`: When you create or updating an app role, this value must be true.
To delete a role, this must first be set to false.
At that point, in a subsequent call, this role might be removed.
Default value is true.
      - `[Origin <String>]`: Specifies if the app role is defined on the application object or on the servicePrincipal entity.
Must not be included in any POST or PATCH requests.
Read-only.
      - `[Value <String>]`: Specifies the value to include in the roles claim in ID tokens and access tokens authenticating an assigned user or service principal.
Must not exceed 120 characters in length.
Allowed characters are : ! # $ % & ' ( ) * + , - . / : ;  =  ? @ \[ \] ^ + _  {  } ~, and characters in the ranges


@ - `[ ]` ^ + _  {  } ~, and characters in the ranges 0-9, A-Z, and a-z.
Any other character, including the space character, aren't allowed.
May not begin with ..
    - `[ApplicationTemplateId <String>]`: Unique identifier of the applicationTemplate.
Supports $filter (eq, not, ne).
Read-only.
null if the app wasn't created from an application template.
    - `[ClaimsMappingPolicies <IMicrosoftGraphClaimsMappingPolicy- `[]`>]`: The claimsMappingPolicies assigned to this service principal.
Supports $expand.
      - `[AppliesTo <IMicrosoftGraphDirectoryObject- `[]`>]`: 
      - `[Definition <String- `[]`>]`: A string collection containing a JSON string that defines the rules and settings for a policy.
The syntax for the definition differs for each derived policy type.
Required.
      - `[IsOrganizationDefault <Boolean?>]`: If set to true, activates this policy.
There can be many policies for the same policy type, but only one can be activated as the organization default.
Optional, default value is false.
      - `[Description <String>]`: Description for this policy.
Required.
      - `[DisplayName <String>]`: Display name for this policy.
Required.
      - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ClaimsPolicy <IMicrosoftGraphCustomClaimsPolicy>]`: customClaimsPolicy
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AudienceOverride <String>]`: If specified, it overrides the content of the audience claim for WS-Federation and SAML2 protocols.
A custom signing key must be used for audienceOverride to be applied, otherwise, the audienceOverride value is ignored.
The value provided must be in the format of an absolute URI.
      - `[Claims <IMicrosoftGraphCustomClaimBase- `[]`>]`: Defines which claims are present in the tokens affected by the policy, in addition to the basic claim and the core claim set.
Inherited from customclaimbase.
        - `[Configurations <IMicrosoftGraphCustomClaimConfiguration- `[]`>]`: One or more configurations that describe how the claim is sourced and under what conditions.
          - `[Attribute <IMicrosoftGraphCustomClaimAttributeBase>]`: customClaimAttributeBase
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Condition <IMicrosoftGraphCustomClaimConditionBase>]`: customClaimConditionBase
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Transformations <IMicrosoftGraphCustomClaimTransformation- `[]`>]`: An ordered list of transformations that are applied in sequence.
            - `[Input <IMicrosoftGraphTransformationAttribute>]`: transformationAttribute
              - `[(Any) <Object>]`: This indicates any property can be added to this object.
              - `[Attribute <IMicrosoftGraphCustomClaimAttributeBase>]`: customClaimAttributeBase
              - `[TreatAsMultiValue <Boolean?>]`: This flag is only relevant in the case where the attribute is multivalued.
By default, transformations are only applied to the first element in a multi-valued claim, however setting this flag to true ensures the transformation is applied to all values, resulting in a multivalued output.
      - `[IncludeApplicationIdInIssuer <Boolean?>]`: Indicates whether the application ID is added to the claim.
It is relevant only for SAML2.0 and if a custom signing key is used.
the default value is true.
Optional.
      - `[IncludeBasicClaimSet <Boolean?>]`: Determines whether the basic claim set is included in tokens affected by this policy.
If set to true, all claims in the basic claim set are emitted in tokens affected by the policy.
By default the basic claim set isn't in the tokens unless they're explicitly configured in this policy.
    - `[CreatedObjects <IMicrosoftGraphDirectoryObject- `[]`>]`: Directory objects created by this service principal.
Read-only.
Nullable.
    - `[CustomSecurityAttributes <IMicrosoftGraphCustomSecurityAttributeValue>]`: customSecurityAttributeValue
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DelegatedPermissionClassifications <IMicrosoftGraphDelegatedPermissionClassification- `[]`>]`: The permission classifications for delegated permissions exposed by the app that this service principal represents.
Supports $expand.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Classification <String>]`: permissionClassificationType
      - `[PermissionId <String>]`: The unique identifier (id) for the delegated permission listed in the publishedPermissionScopes collection of the servicePrincipal.
Required on create.
Doesn't support $filter.
      - `[PermissionName <String>]`: The claim value (value) for the delegated permission listed in the publishedPermissionScopes collection of the servicePrincipal.
Doesn't support $filter.
    - `[Description <String>]`: Free text field to provide an internal end-user facing description of the service principal.
End-user portals such MyApps displays the application description in this field.
The maximum allowed size is 1,024 characters.
Supports $filter (eq, ne, not, ge, le, startsWith) and $search.
    - `[DisabledByMicrosoftStatus <String>]`: Specifies whether Microsoft has disabled the registered application.
Possible values are: null (default value), NotDisabled, and DisabledDueToViolationOfServicesAgreement (reasons may include suspicious, abusive, or malicious activity, or a violation of the Microsoft Services Agreement). 
Supports $filter (eq, ne, not).
    - `[DisplayName <String>]`: The display name for the service principal.
Supports $filter (eq, ne, not, ge, le, in, startsWith, and eq on null values), $search, and $orderby.
    - `[Endpoints <IMicrosoftGraphEndpoint- `[]`>]`: Endpoints available for discovery.
Services like Sharepoint populate this property with a tenant specific SharePoint endpoints that other applications can discover and use in their experiences.
      - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Capability <String>]`: Describes the capability that is associated with this resource.
(for example, Messages, Conversations, etc.) Not nullable.
Read-only.
      - `[ProviderId <String>]`: Application id of the publishing underlying service.
Not nullable.
Read-only.
      - `[ProviderName <String>]`: Name of the publishing underlying service.
Read-only.
      - `[ProviderResourceId <String>]`: For Microsoft 365 groups, this is set to a well-known name for the resource (for example, Yammer.FeedURL etc.).
Not nullable.
Read-only.
      - `[Uri <String>]`: URL of the published resource.
Not nullable.
Read-only.
    - `[ErrorUrl <String>]`: Deprecated.
Don't use.
    - `[FederatedIdentityCredentials <IMicrosoftGraphFederatedIdentityCredential- `[]`>]`: 
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Audiences <String- `[]`>]`: The audience that can appear in the external token.
This field is mandatory and should be set to api://AzureADTokenExchange for Microsoft Entra ID.
It says what Microsoft identity platform should accept in the aud claim in the incoming token.
This value represents Microsoft Entra ID in your external identity provider and has no fixed value across identity providers - you may need to create a new application registration in your identity provider to serve as the audience of this token.
This field can only accept a single value and has a limit of 600 characters.
Required.
      - `[ClaimsMatchingExpression <IMicrosoftGraphFederatedIdentityExpression>]`: federatedIdentityExpression
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[LanguageVersion <Int32?>]`: Indicated the language version to be used.
Should always be set to 1.
Required.
        - `[Value <String>]`: Indicates the configured expression.
Required.
      - `[Description <String>]`: The un-validated, user-provided description of the federated identity credential.
It has a limit of 600 characters.
Optional.
      - `[Issuer <String>]`: The URL of the external identity provider and must match the issuer claim of the external token being exchanged.
The combination of the values of issuer and subject must be unique on the app.
It has a limit of 600 characters.
Required.
      - `[Name <String>]`: The unique identifier for the federated identity credential, which has a limit of 120 characters and must be URL friendly.
It is immutable once created.
Alternate key.
Required.
Not nullable.
Supports $filter (eq).
      - `[Subject <String>]`: Nullable. 
Defaults to null if not set.
The identifier of the external software workload within the external identity provider.
Like the audience value, it has no fixed format, as each identity provider uses their own - sometimes a GUID, sometimes a colon delimited identifier, sometimes arbitrary strings.
The value here must match the sub claim within the token presented to Microsoft Entra ID.
The combination of issuer and subject must be unique on the app.
It has a limit of 600 characters.
If subject is defined, claimsMatchingExpression must be null.
Supports $filter (eq).
    - `[HomeRealmDiscoveryPolicies <IMicrosoftGraphHomeRealmDiscoveryPolicy- `[]`>]`: The homeRealmDiscoveryPolicies assigned to this service principal.
Supports $expand.
      - `[AppliesTo <IMicrosoftGraphDirectoryObject- `[]`>]`: 
      - `[Definition <String- `[]`>]`: A string collection containing a JSON string that defines the rules and settings for a policy.
The syntax for the definition differs for each derived policy type.
Required.
      - `[IsOrganizationDefault <Boolean?>]`: If set to true, activates this policy.
There can be many policies for the same policy type, but only one can be activated as the organization default.
Optional, default value is false.
      - `[Description <String>]`: Description for this policy.
Required.
      - `[DisplayName <String>]`: Display name for this policy.
Required.
      - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Homepage <String>]`: Home page or landing page of the application.
    - `[Info <IMicrosoftGraphInformationalUrl>]`: informationalUrl
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[LogoUrl <String>]`: CDN URL to the application's logo, Read-only.
      - `[MarketingUrl <String>]`: Link to the application's marketing page.
For example, https://www.contoso.com/app/marketing
      - `[PrivacyStatementUrl <String>]`: Link to the application's privacy statement.
For example, https://www.contoso.com/app/privacy
      - `[SupportUrl <String>]`: Link to the application's support page.
For example, https://www.contoso.com/app/support
      - `[TermsOfServiceUrl <String>]`: Link to the application's terms of service statement.
For example, https://www.contoso.com/app/termsofservice
    - `[KeyCredentials <IMicrosoftGraphKeyCredential- `[]`>]`: The collection of key credentials associated with the service principal.
Not nullable.
Supports $filter (eq, not, ge, le).
      - `[CustomKeyIdentifier <Byte- `[]`>]`: A 40-character binary type that can be used to identify the credential.
Optional.
When not provided in the payload, defaults to the thumbprint of the certificate.
      - `[DisplayName <String>]`: The friendly name for the key, with a maximum length of 90 characters.
Longer values are accepted but shortened.
Optional.
      - `[EndDateTime <DateTime?>]`: The date and time at which the credential expires.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
      - `[Key <Byte- `[]`>]`: Value for the key credential.
Should be a Base64 encoded value.
Returned only on $select for a single object, that is, GET applications/{applicationId}?$select=keyCredentials or GET servicePrincipals/{servicePrincipalId}?$select=keyCredentials; otherwise, it's always null. 
From a .cer certificate, you can read the key using the Convert.ToBase64String() method.
For more information, see Get the certificate key.
      - `[KeyId <String>]`: The unique identifier for the key.
      - `[StartDateTime <DateTime?>]`: The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
      - `[Type <String>]`: The type of key credential; for example, Symmetric, AsymmetricX509Cert, or X509CertAndPassword.
      - `[Usage <String>]`: A string that describes the purpose for which the key can be used; for example, None​, Verify​, PairwiseIdentifier​, Delegation​, Decrypt​, Encrypt​, HashedIdentifier​, SelfSignedTls, or Sign.
If usage is Sign​, the type should be X509CertAndPassword​, and the passwordCredentials​ for signing should be defined.
    - `[LicenseDetails <IMicrosoftGraphLicenseDetails- `[]`>]`: 
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[ServicePlans <IMicrosoftGraphServicePlanInfo- `[]`>]`: Information about the service plans assigned with the license.
Read-only.
Not nullable.
        - `[AppliesTo <String>]`: The object the service plan can be assigned to.
The possible values are: User - service plan can be assigned to individual users.Company - service plan can be assigned to the entire tenant.
        - `[ProvisioningStatus <String>]`: The provisioning status of the service plan.
The possible values are:Success - Service is fully provisioned.Disabled - Service is disabled.Error - The service plan isn't provisioned and is in an error state.PendingInput - The service isn't provisioned and is awaiting service confirmation.PendingActivation - The service is provisioned but requires explicit activation by an administrator (for example, Intune_O365 service plan)PendingProvisioning - Microsoft has added a new service to the product SKU and it isn't activated in the tenant.
        - `[ServicePlanId <String>]`: The unique identifier of the service plan.
        - `[ServicePlanName <String>]`: The name of the service plan.
      - `[SkuId <String>]`: Unique identifier (GUID) for the service SKU.
Equal to the skuId property on the related subscribedSku object.
Read-only.
      - `[SkuPartNumber <String>]`: Unique SKU display name.
Equal to the skuPartNumber on the related subscribedSku object; for example, AAD_Premium.
Read-only.
    - `[LoginUrl <String>]`: Specifies the URL where the service provider redirects the user to Microsoft Entra ID to authenticate.
Microsoft Entra ID uses the URL to launch the application from Microsoft 365 or the Microsoft Entra My Apps.
When blank, Microsoft Entra ID performs IdP-initiated sign-on for applications configured with SAML-based single sign-on.
The user launches the application from Microsoft 365, the Microsoft Entra My Apps, or the Microsoft Entra SSO URL.
    - `[LogoutUrl <String>]`: Specifies the URL that the Microsoft's authorization service uses to sign out a user using OpenId Connect front-channel, back-channel, or SAML sign out protocols.
    - `[MemberOf <IMicrosoftGraphDirectoryObject- `[]`>]`: Roles that this service principal is a member of.
HTTP Methods: GET Read-only.
Nullable.
Supports $expand.
    - `[Notes <String>]`: Free text field to capture information about the service principal, typically used for operational purposes.
Maximum allowed size is 1,024 characters.
    - `[NotificationEmailAddresses <String- `[]`>]`: Specifies the list of email addresses where Microsoft Entra ID sends a notification when the active certificate is near the expiration date.
This is only for the certificates used to sign the SAML token issued for Microsoft Entra Gallery applications.
    - `[Oauth2PermissionGrants <IMicrosoftGraphOAuth2PermissionGrant- `[]`>]`: Delegated permission grants authorizing this service principal to access an API on behalf of a signed-in user.
Read-only.
Nullable.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[ClientId <String>]`: The object id (not appId) of the client service principal for the application that is authorized to act on behalf of a signed-in user when accessing an API.
Required.
Supports $filter (eq only).
      - `[ConsentType <String>]`: Indicates whether authorization is granted for the client application to impersonate all users or only a specific user.
AllPrincipals indicates authorization to impersonate all users.
Principal indicates authorization to impersonate a specific user.
Consent on behalf of all users can be granted by an administrator.
Nonadmin users may be authorized to consent on behalf of themselves in some cases, for some delegated permissions.
Required.
Supports $filter (eq only).
      - `[ExpiryTime <DateTime?>]`: Currently, the end time value is ignored, but a value is required when creating an oAuth2PermissionGrant.
Required.
      - `[PrincipalId <String>]`: The id of the user on behalf of whom the client is authorized to access the resource, when consentType is Principal.
If consentType is AllPrincipals this value is null.
Required when consentType is Principal.
Supports $filter (eq only).
      - `[ResourceId <String>]`: The id of the resource service principal to which access is authorized.
This identifies the API that the client is authorized to attempt to call on behalf of a signed-in user.
Supports $filter (eq only).
      - `[Scope <String>]`: A space-separated list of the claim values for delegated permissions that should be included in access tokens for the resource application (the API).
For example, openid User.Read GroupMember.Read.All.
Each claim value should match the value field of one of the delegated permissions defined by the API, listed in the publishedPermissionScopes property of the resource service principal.
Must not exceed 3850 characters in length.
      - `[StartTime <DateTime?>]`: Currently, the start time value is ignored, but a value is required when creating an oAuth2PermissionGrant.
Required.
    - `[OwnedObjects <IMicrosoftGraphDirectoryObject- `[]`>]`: Directory objects that are owned by this service principal.
Read-only.
Nullable.
Supports $expand and $filter (/$count eq 0, /$count ne 0, /$count eq 1, /$count ne 1).
    - `[Owners <IMicrosoftGraphDirectoryObject- `[]`>]`: Directory objects that are owners of this servicePrincipal.
The owners are a set of nonadmin users or servicePrincipals who are allowed to modify this object.
Supports $expand and $filter (/$count eq 0, /$count ne 0, /$count eq 1, /$count ne 1).
    - `[PasswordCredentials <IMicrosoftGraphPasswordCredential- `[]`>]`: The collection of password credentials associated with the service principal.
Not nullable.
      - `[CustomKeyIdentifier <Byte- `[]`>]`: Do not use.
      - `[DisplayName <String>]`: Friendly name for the password.
Optional.
      - `[EndDateTime <DateTime?>]`: The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Optional.
      - `[Hint <String>]`: Contains the first three characters of the password.
Read-only.
      - `[KeyId <String>]`: The unique identifier for the password.
      - `[SecretText <String>]`: Read-only; Contains the strong passwords generated by Microsoft Entra ID that are 16-64 characters in length.
The generated password value is only returned during the initial POST request to addPassword.
There is no way to retrieve this password in the future.
      - `[StartDateTime <DateTime?>]`: The date and time at which the password becomes valid.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Optional.
    - `[PasswordSingleSignOnSettings <IMicrosoftGraphPasswordSingleSignOnSettings>]`: passwordSingleSignOnSettings
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Fields <IMicrosoftGraphPasswordSingleSignOnField- `[]`>]`: The fields to capture to fill the user credentials for password-based single sign-on.
        - `[CustomizedLabel <String>]`: Title/label override for customization.
        - `[DefaultLabel <String>]`: Label that would be used if no customizedLabel is provided.
Read only.
        - `[FieldId <String>]`: Id used to identity the field type.
This is an internal ID and possible values are param1, param2, paramuserName, parampassword.
        - `[Type <String>]`: Type of the credential.
The values can be text, password.
    - `[PermissionGrantPreApprovalPolicies <IMicrosoftGraphPermissionGrantPreApprovalPolicy- `[]`>]`: 
      - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Conditions <IMicrosoftGraphPreApprovalDetail- `[]`>]`: A list of condition sets describing the conditions under which the permission to grant consent for the app has been preapproved.
        - `[Permissions <IMicrosoftGraphPreApprovedPermissions>]`: preApprovedPermissions
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[PermissionKind <String>]`: permissionKind
          - `[PermissionType <String>]`: permissionType
        - `[ScopeType <String>]`: resourceScopeType
        - `[SensitivityLabels <IMicrosoftGraphScopeSensitivityLabels>]`: scopeSensitivityLabels
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[LabelKind <String>]`: labelKind
    - `[PreferredSingleSignOnMode <String>]`: Specifies the single sign-on mode configured for this application.
Microsoft Entra ID uses the preferred single sign-on mode to launch the application from Microsoft 365 or the Microsoft Entra My Apps.
The supported values are password, saml, notSupported, and oidc.
Note: This field might be null for older SAML apps and for OIDC applications where it isn't set automatically.
    - `[PreferredTokenSigningKeyEndDateTime <DateTime?>]`: Specifies the expiration date of the keyCredential used for token signing, marked by preferredTokenSigningKeyThumbprint.
Updating this attribute isn't currently supported.
For details, see ServicePrincipal property differences.
    - `[PreferredTokenSigningKeyThumbprint <String>]`: This property can be used on SAML applications (apps that have preferredSingleSignOnMode set to saml) to control which certificate is used to sign the SAML responses.
For applications that aren't SAML, don't write or otherwise rely on this property.
    - `[PublishedPermissionScopes <IMicrosoftGraphPermissionScope- `[]`>]`: The delegated permissions exposed by the application.
For more information, see the oauth2PermissionScopes property on the application entity's api property.
Not nullable.
Note: This property is named oauth2PermissionScopes in v1.0.
      - `[AdminConsentDescription <String>]`: A description of the delegated permissions, intended to be read by an administrator granting the permission on behalf of all users.
This text appears in tenant-wide admin consent experiences.
      - `[AdminConsentDisplayName <String>]`: The permission's title, intended to be read by an administrator granting the permission on behalf of all users.
      - `[Id <String>]`: Unique delegated permission identifier inside the collection of delegated permissions defined for a resource application.
      - `[IsEnabled <Boolean?>]`: When you create or update a permission, this property must be set to true (which is the default).
To delete a permission, this property must first be set to false. 
At that point, in a subsequent call, the permission may be removed.
      - `[Origin <String>]`: 
      - `[Type <String>]`: The possible values are: User and Admin.
Specifies whether this delegated permission should be considered safe for non-admin users to consent to on behalf of themselves, or whether an administrator consent should always be required.
While Microsoft Graph defines the default consent requirement for each permission, the tenant administrator may override the behavior in their organization (by allowing, restricting, or limiting user consent to this delegated permission).
For more information, see Configure how users consent to applications.
      - `[UserConsentDescription <String>]`: A description of the delegated permissions, intended to be read by a user granting the permission on their own behalf.
This text appears in consent experiences where the user is consenting only on behalf of themselves.
      - `[UserConsentDisplayName <String>]`: A title for the permission, intended to be read by a user granting the permission on their own behalf.
This text appears in consent experiences where the user is consenting only on behalf of themselves.
      - `[Value <String>]`: Specifies the value to include in the scp (scope) claim in access tokens.
Must not exceed 120 characters in length.
Allowed characters are : ! # $ % & ' ( ) * + , - . / : ;  =  ? @ \[ \] ^ + _  {  } ~, and characters in the ranges


@ - `[ ]` ^ + _  {  } ~, and characters in the ranges 0-9, A-Z and a-z.
Any other character, including the space character, aren't allowed.
May not begin with ..
    - `[PublisherName <String>]`: The name of the Microsoft Entra tenant that published the application.
    - `[RemoteDesktopSecurityConfiguration <IMicrosoftGraphRemoteDesktopSecurityConfiguration>]`: remoteDesktopSecurityConfiguration
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[IsRemoteDesktopProtocolEnabled <Boolean?>]`: Determines if Microsoft Entra ID RDS authentication protocol for RDP is enabled.
      - `[TargetDeviceGroups <IMicrosoftGraphTargetDeviceGroup- `[]`>]`: The collection of target device groups that are associated with the RDS security configuration that will be enabled for SSO when a client connects to the target device over RDP using the new Microsoft Entra ID RDS authentication protocol.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[DisplayName <String>]`: Display name for the target device group.
    - `[ReplyUrls <String- `[]`>]`: The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.
Not nullable.
    - `[SamlMetadataUrl <String>]`: The url where the service exposes SAML metadata for federation.
    - `[SamlSingleSignOnSettings <IMicrosoftGraphSamlSingleSignOnSettings>]`: samlSingleSignOnSettings
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[RelayState <String>]`: The relative URI the service provider would redirect to after completion of the single sign-on flow.
    - `[ServicePrincipalNames <String- `[]`>]`: Contains the list of identifiersUris, copied over from the associated application.
More values can be added to hybrid applications.
These values can be used to identify the permissions exposed by this app within Microsoft Entra ID.
For example,Client apps can specify a resource URI that is based on the values of this property to acquire an access token, which is the URI returned in the 'aud' claim.The any operator is required for filter expressions on multi-valued properties.
Not nullable. 
Supports $filter (eq, not, ge, le, startsWith).
    - `[ServicePrincipalType <String>]`: Identifies if the service principal represents an application or a managed identity.
This is set by Microsoft Entra ID internally.
For a service principal that represents an application this is set as Application.
For a service principal that represents a managed identity this is set as ManagedIdentity.
The SocialIdp type is for internal use.
    - `[SignInAudience <String>]`: Specifies the Microsoft accounts that are supported for the current application.
Read-only.
Supported values are:AzureADMyOrg: Users with a Microsoft work or school account in my organization's Microsoft Entra tenant (single-tenant).AzureADMultipleOrgs: Users with a Microsoft work or school account in any organization's Microsoft Entra tenant (multitenant).AzureADandPersonalMicrosoftAccount: Users with a personal Microsoft account, or a work or school account in any organization's Microsoft Entra tenant.PersonalMicrosoftAccount: Users with a personal Microsoft account only.
    - `[Synchronization <IMicrosoftGraphSynchronization>]`: synchronization
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Jobs <IMicrosoftGraphSynchronizationJob- `[]`>]`: Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[BulkUpload <IMicrosoftGraphBulkUpload>]`: bulkUpload
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[Schedule <IMicrosoftGraphSynchronizationSchedule>]`: synchronizationSchedule
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Expiration <DateTime?>]`: Date and time when this job will expire.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
          - `[Interval <TimeSpan?>]`: The interval between synchronization iterations.
The value is represented in ISO 8601  format for durations.
For example, P1M represents a period of one month and PT1M represents a period of one minute.
          - `[State <String>]`: synchronizationScheduleState
        - `[Schema <IMicrosoftGraphSynchronizationSchema>]`: synchronizationSchema
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
        - `[Status <IMicrosoftGraphSynchronizationStatus>]`: synchronizationStatus
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Code <String>]`: synchronizationStatusCode
          - `[CountSuccessiveCompleteFailures <Int64?>]`: Number of consecutive times this job failed.
          - `[EscrowsPruned <Boolean?>]`: true if the job's escrows (object-level errors) were pruned during initial synchronization.
Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.
Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.
When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.
          - `[LastExecution <IMicrosoftGraphSynchronizationTaskExecution>]`: synchronizationTaskExecution
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
            - `[ActivityIdentifier <String>]`: Identifier of the job run.
            - `[CountEntitled <Int64?>]`: Count of processed entries that were assigned for this application.
            - `[CountEntitledForProvisioning <Int64?>]`: Count of processed entries that were assigned for provisioning.
            - `[CountEscrowed <Int64?>]`: Count of entries that were escrowed (errors).
            - `[CountEscrowedRaw <Int64?>]`: Count of entries that were escrowed, including system-generated escrows.
            - `[CountExported <Int64?>]`: Count of exported entries.
            - `[CountExports <Int64?>]`: Count of entries that were expected to be exported.
            - `[CountImported <Int64?>]`: Count of imported entries.
            - `[CountImportedDeltas <Int64?>]`: Count of imported delta-changes.
            - `[CountImportedReferenceDeltas <Int64?>]`: Count of imported delta-changes pertaining to reference changes.
            - `[Error <IMicrosoftGraphSynchronizationError>]`: synchronizationError
              - `[(Any) <Object>]`: This indicates any property can be added to this object.
              - `[Code <String>]`: The error code.
For example, AzureDirectoryB2BManagementPolicyCheckFailure.
              - `[Message <String>]`: The error message.
For example, Policy permitting auto-redemption of invitations not configured.
              - `[TenantActionable <Boolean?>]`: The action to take to resolve the error.
For example, false.
            - `[State <String>]`: synchronizationTaskExecutionResult
            - `[TimeBegan <DateTime?>]`: Time when this job run began.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
            - `[TimeEnded <DateTime?>]`: Time when this job run ended.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
          - `[LastSuccessfulExecution <IMicrosoftGraphSynchronizationTaskExecution>]`: synchronizationTaskExecution
          - `[LastSuccessfulExecutionWithExports <IMicrosoftGraphSynchronizationTaskExecution>]`: synchronizationTaskExecution
          - `[Progress <IMicrosoftGraphSynchronizationProgress- `[]`>]`: Details of the progress of a job toward completion.
            - `[CompletedUnits <Int64?>]`: The numerator of a progress ratio; the number of units of changes already processed.
            - `[ProgressObservationDateTime <DateTime?>]`: The time of a progress observation as an offset in minutes from UTC.
            - `[TotalUnits <Int64?>]`: The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.
            - `[Units <String>]`: An optional description of the units.
          - `[Quarantine <IMicrosoftGraphSynchronizationQuarantine>]`: synchronizationQuarantine
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
            - `[CurrentBegan <DateTime?>]`: Date and time when the quarantine was last evaluated and imposed.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
            - `[Error <IMicrosoftGraphSynchronizationError>]`: synchronizationError
            - `[NextAttempt <DateTime?>]`: Date and time when the next attempt to re-evaluate the quarantine will be made.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
            - `[Reason <String>]`: quarantineReason
            - `[SeriesBegan <DateTime?>]`: Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
            - `[SeriesCount <Int64?>]`: Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).
          - `[SteadyStateFirstAchievedTime <DateTime?>]`: The time when steady state (no more changes to the process) was first achieved.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
          - `[SteadyStateLastAchievedTime <DateTime?>]`: The time when steady state (no more changes to the process) was last achieved.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
          - `[SynchronizedEntryCountByType <IMicrosoftGraphStringKeyLongValuePair- `[]`>]`: Count of synchronized objects, listed by object type.
            - `[Key <String>]`: The mapping of the user type from the source system to the target system.
For example:User to User - For Microsoft Entra ID to Microsoft Entra synchronization worker to user - For Workday to Microsoft Entra synchronization.
            - `[Value <Int64?>]`: Total number of synchronized objects.
          - `[TroubleshootingUrl <String>]`: In the event of an error, the URL with the troubleshooting steps for the issue.
        - `[SynchronizationJobSettings <IMicrosoftGraphKeyValuePair- `[]`>]`: Settings associated with the job.
Some settings are inherited from the template.
          - `[Name <String>]`: Name for this key-value pair
          - `[Value <String>]`: Value for this key-value pair
        - `[TemplateId <String>]`: Identifier of the synchronization template this job is based on.
      - `[Secrets <IMicrosoftGraphSynchronizationSecretKeyStringValuePair- `[]`>]`: Represents a collection of credentials to access provisioned cloud applications.
        - `[Key <String>]`: synchronizationSecret
        - `[Value <String>]`: The value of the secret.
      - `[Templates <IMicrosoftGraphSynchronizationTemplate- `[]`>]`: Pre-configured synchronization settings for a particular application.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[ApplicationId <String>]`: Identifier of the application this template belongs to.
        - `[Default <Boolean?>]`: true if this template is recommended to be the default for the application.
        - `[Description <String>]`: Description of the template.
        - `[Discoverable <Boolean?>]`: true if this template should appear in the collection of templates available for the application instance (service principal).
        - `[FactoryTag <String>]`: One of the well-known factory tags supported by the synchronization engine.
The factoryTag tells the synchronization engine which implementation to use when processing jobs based on this template.
        - `[Metadata <IMicrosoftGraphSynchronizationMetadataEntry- `[]`>]`: Additional extension properties.
Unless mentioned explicitly, metadata values shouldn't be changed.
          - `[Key <String>]`: synchronizationMetadata
          - `[Value <String>]`: Value of the metadata property.
        - `[Schema <IMicrosoftGraphSynchronizationSchema>]`: synchronizationSchema
    - `[Tags <String- `[]`>]`: Custom strings that can be used to categorize and identify the service principal.
Not nullable.
The value is the union of strings set here and on the associated application entity's tags property.Supports $filter (eq, not, ge, le, startsWith).
    - `[TokenEncryptionKeyId <String>]`: Specifies the keyId of a public key from the keyCredentials collection.
When configured, Microsoft Entra ID issues tokens for this application encrypted using the key specified by this property.
The application code that receives the encrypted token must use the matching private key to decrypt the token before it can be used for the signed-in user.
    - `[TokenIssuancePolicies <IMicrosoftGraphTokenIssuancePolicy- `[]`>]`: The tokenIssuancePolicies assigned to this service principal.
Supports $expand.
      - `[AppliesTo <IMicrosoftGraphDirectoryObject- `[]`>]`: 
      - `[Definition <String- `[]`>]`: A string collection containing a JSON string that defines the rules and settings for a policy.
The syntax for the definition differs for each derived policy type.
Required.
      - `[IsOrganizationDefault <Boolean?>]`: If set to true, activates this policy.
There can be many policies for the same policy type, but only one can be activated as the organization default.
Optional, default value is false.
      - `[Description <String>]`: Description for this policy.
Required.
      - `[DisplayName <String>]`: Display name for this policy.
Required.
      - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[TokenLifetimePolicies <IMicrosoftGraphTokenLifetimePolicy- `[]`>]`: The tokenLifetimePolicies assigned to this service principal.
Supports $expand.
      - `[AppliesTo <IMicrosoftGraphDirectoryObject- `[]`>]`: 
      - `[Definition <String- `[]`>]`: A string collection containing a JSON string that defines the rules and settings for a policy.
The syntax for the definition differs for each derived policy type.
Required.
      - `[IsOrganizationDefault <Boolean?>]`: If set to true, activates this policy.
There can be many policies for the same policy type, but only one can be activated as the organization default.
Optional, default value is false.
      - `[Description <String>]`: Description for this policy.
Required.
      - `[DisplayName <String>]`: Display name for this policy.
Required.
      - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[TransitiveMemberOf <IMicrosoftGraphDirectoryObject- `[]`>]`: 
    - `[VerifiedPublisher <IMicrosoftGraphVerifiedPublisher>]`: verifiedPublisher
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[AddedDateTime <DateTime?>]`: The timestamp when the verified publisher was first added or most recently updated.
      - `[DisplayName <String>]`: The verified publisher name from the app publisher's Microsoft Partner Network (MPN) account.
      - `[VerifiedPublisherId <String>]`: The ID of the verified publisher from the app publisher's Partner Center account.
  - `[TrafficForwardingType <String>]`: trafficForwardingType

INPUTOBJECT `<INetworkAccessIdentity>`: Identity Parameter
  - `[ActivityPivotDateTime <DateTime?>]`: Usage: activityPivotDateTime={activityPivotDateTime}
  - `[AggregatedBy <String>]`: Usage: aggregatedBy='{aggregatedBy}'
  - `[AlertId <String>]`: The unique identifier of alert
  - `[BranchSiteId <String>]`: The unique identifier of branchSite
  - `[ConditionalAccessPolicyId <String>]`: The unique identifier of conditionalAccessPolicy
  - `[ConnectivityConfigurationLinkId <String>]`: The unique identifier of connectivityConfigurationLink
  - `[DeviceLinkId <String>]`: The unique identifier of deviceLink
  - `[DiscoveryPivotDateTime <DateTime?>]`: Usage: discoveryPivotDateTime={discoveryPivotDateTime}
  - `[EndDateTime <DateTime?>]`: Usage: endDateTime={endDateTime}
  - `[FilteringPolicyId <String>]`: The unique identifier of filteringPolicy
  - `[FilteringProfileId <String>]`: The unique identifier of filteringProfile
  - `[ForwardingPolicyId <String>]`: The unique identifier of forwardingPolicy
  - `[ForwardingProfileId <String>]`: The unique identifier of forwardingProfile
  - `[NetworkAccessTrafficTransactionId <String>]`: The unique identifier of networkAccessTraffic
  - `[PolicyLinkId <String>]`: The unique identifier of policyLink
  - `[PolicyRuleId <String>]`: The unique identifier of policyRule
  - `[RemoteNetworkHealthEventId <String>]`: The unique identifier of remoteNetworkHealthEvent
  - `[RemoteNetworkId <String>]`: The unique identifier of remoteNetwork
  - `[StartDateTime <DateTime?>]`: Usage: startDateTime={startDateTime}

POLICIES `<IMicrosoftGraphNetworkaccessPolicyLink- `[]`>`: The traffic forwarding policies associated with this profile.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Policy <IMicrosoftGraphNetworkaccessPolicy>]`: policy
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Description <String>]`: Description.
    - `[Name <String>]`: Policy name.
    - `[PolicyRules <IMicrosoftGraphNetworkaccessPolicyRule- `[]`>]`: Represents the definition of the policy ruleset that makes up the core definition of a policy.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Name <String>]`: Name.
    - `[Version <String>]`: Version.
  - `[State <String>]`: status
  - `[Version <String>]`: Version.

SERVICEPRINCIPAL `<IMicrosoftGraphServicePrincipal>`: servicePrincipal
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AccountEnabled <Boolean?>]`: true if the service principal account is enabled; otherwise, false.
If set to false, then no users are able to sign in to this app, even if they're assigned to it.
Supports $filter (eq, ne, not, in).
  - `[AddIns <IMicrosoftGraphAddIn- `[]`>]`: Defines custom behavior that a consuming service can use to call an app in specific contexts.
For example, applications that can render file streams may set the addIns property for its 'FileHandler' functionality.
This lets services like Microsoft 365 call the application in the context of a document the user is working on.
    - `[Id <String>]`: The unique identifier for the addIn object.
    - `[Properties <IMicrosoftGraphKeyValue- `[]`>]`: The collection of key-value pairs that define parameters that the consuming service can use or call.
You must specify this property when performing a POST or a PATCH operation on the addIns collection.
Required.
      - `[Key <String>]`: Key.
      - `[Value <String>]`: Value.
    - `[Type <String>]`: The unique name for the functionality exposed by the app.
  - `[AlternativeNames <String- `[]`>]`: Used to retrieve service principals by subscription, identify resource group and full resource IDs for managed identities.
Supports $filter (eq, not, ge, le, startsWith).
  - `[AppDescription <String>]`: The description exposed by the associated application.
  - `[AppDisplayName <String>]`: The display name exposed by the associated application.
Maximum length is 256 characters.
  - `[AppId <String>]`: The unique identifier for the associated application (its appId property).
Alternate key.
Supports $filter (eq, ne, not, in, startsWith).
  - `[AppManagementPolicies <IMicrosoftGraphAppManagementPolicy- `[]`>]`: The appManagementPolicy applied to this service principal.
    - `[Description <String>]`: Description for this policy.
Required.
    - `[DisplayName <String>]`: Display name for this policy.
Required.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AppliesTo <IMicrosoftGraphDirectoryObject- `[]`>]`: Collection of application and service principals to which a policy is applied.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[IsEnabled <Boolean?>]`: Denotes whether the policy is enabled.
    - `[Restrictions <IMicrosoftGraphCustomAppManagementConfiguration>]`: customAppManagementConfiguration
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[KeyCredentials <IMicrosoftGraphKeyCredentialConfiguration- `[]`>]`: 
        - `[CertificateBasedApplicationConfigurationIds <String- `[]`>]`: Collection of GUIDs that represent certificateBasedApplicationConfiguration that is allowed as root and intermediate certificate authorities.
        - `[MaxLifetime <TimeSpan?>]`: String value that indicates the maximum lifetime for key expiration, defined as an ISO 8601 duration.
For example, P4DT12H30M5S represents four days, 12 hours, 30 minutes, and five seconds.
This property is required when restrictionType is set to keyLifetime.
        - `[RestrictForAppsCreatedAfterDateTime <DateTime?>]`: Specifies the date from which the policy restriction applies to newly created applications.
For existing applications, the enforcement date can be retroactively applied.
        - `[RestrictionType <String>]`: appKeyCredentialRestrictionType
        - `[State <String>]`: appManagementRestrictionState
      - `[PasswordCredentials <IMicrosoftGraphPasswordCredentialConfiguration- `[]`>]`: 
        - `[MaxLifetime <TimeSpan?>]`: String value that indicates the maximum lifetime for password expiration, defined as an ISO 8601 duration.
For example, P4DT12H30M5S represents four days, 12 hours, 30 minutes, and five seconds.
This property is required when restrictionType is set to passwordLifetime.
        - `[RestrictForAppsCreatedAfterDateTime <DateTime?>]`: Specifies the date from which the policy restriction applies to newly created applications.
For existing applications, the enforcement date can be retroactively applied.
        - `[RestrictionType <String>]`: appCredentialRestrictionType
        - `[State <String>]`: appManagementRestrictionState
      - `[ApplicationRestrictions <IMicrosoftGraphCustomAppManagementApplicationConfiguration>]`: customAppManagementApplicationConfiguration
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Audiences <IMicrosoftGraphAudiencesConfiguration>]`: audiencesConfiguration
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[AzureAdMultipleOrgs <IMicrosoftGraphAudienceRestriction>]`: audienceRestriction
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
            - `[ExcludeActors <IMicrosoftGraphAppManagementPolicyActorExemptions>]`: appManagementPolicyActorExemptions
              - `[(Any) <Object>]`: This indicates any property can be added to this object.
              - `[CustomSecurityAttributes <IMicrosoftGraphCustomSecurityAttributeExemption- `[]`>]`: 
                - `[Id <String>]`: The unique identifier for an entity.
Read-only.
                - `[Operator <String>]`: customSecurityAttributeComparisonOperator
            - `[RestrictForAppsCreatedAfterDateTime <DateTime?>]`: Specifies the date from which the policy restriction applies to newly created applications.
For existing applications, the enforcement date can be retroactively applied.
            - `[State <String>]`: appManagementRestrictionState
          - `[PersonalMicrosoftAccount <IMicrosoftGraphAudienceRestriction>]`: audienceRestriction
        - `[IdentifierUris <IMicrosoftGraphIdentifierUriConfiguration>]`: identifierUriConfiguration
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[NonDefaultUriAddition <IMicrosoftGraphIdentifierUriRestriction>]`: identifierUriRestriction
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
            - `[ExcludeActors <IMicrosoftGraphAppManagementPolicyActorExemptions>]`: appManagementPolicyActorExemptions
            - `[ExcludeAppsReceivingV2Tokens <Boolean?>]`: If true, the restriction isn't enforced for applications that are configured to receive V2 tokens in Microsoft Entra ID; else, the restriction isn't enforced for those applications.
            - `[ExcludeSaml <Boolean?>]`: If true, the restriction isn't enforced for SAML applications in Microsoft Entra ID; else, the restriction is enforced for those applications.
            - `[RestrictForAppsCreatedAfterDateTime <DateTime?>]`: Specifies the date from which the policy restriction applies to newly created applications.
For existing applications, the enforcement date can be retroactively applied.
            - `[State <String>]`: appManagementRestrictionState
  - `[AppOwnerOrganizationId <String>]`: Contains the tenant ID where the application is registered.
This is applicable only to service principals backed by applications.
Supports $filter (eq, ne, NOT, ge, le).
  - `[AppRoleAssignedTo <IMicrosoftGraphAppRoleAssignment- `[]`>]`: App role assignments for this app or service, granted to users, groups, and other service principals.Supports $expand.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AppRoleId <String>]`: The identifier (id) for the app role that is assigned to the principal.
This app role must be exposed in the appRoles property on the resource application's service principal (resourceId).
If the resource application hasn't declared any app roles, a default app role ID of 00000000-0000-0000-0000-000000000000 can be specified to signal that the principal is assigned to the resource app without any specific app roles.
Required on create.
    - `[CreationTimestamp <DateTime?>]`: The time when the app role assignment was created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
    - `[PrincipalDisplayName <String>]`: The display name of the user, group, or service principal that was granted the app role assignment.
Maximum length is 256 characters.
Read-only.
Supports $filter (eq and startswith).
    - `[PrincipalId <String>]`: The unique identifier (id) for the user, security group, or service principal being granted the app role.
Security groups with dynamic memberships are supported.
Required on create.
    - `[PrincipalType <String>]`: The type of the assigned principal.
This can either be User, Group, or ServicePrincipal.
Read-only.
    - `[ResourceDisplayName <String>]`: The display name of the resource app's service principal to which the assignment is made.
Maximum length is 256 characters.
    - `[ResourceId <String>]`: The unique identifier (id) for the resource service principal for which the assignment is made.
Required on create.
Supports $filter (eq only).
  - `[AppRoleAssignmentRequired <Boolean?>]`: Specifies whether users or other service principals need to be granted an app role assignment for this service principal before users can sign in or apps can get tokens.
The default value is false.
Not nullable.
Supports $filter (eq, ne, NOT).
  - `[AppRoleAssignments <IMicrosoftGraphAppRoleAssignment- `[]`>]`: App role assignment for another app or service, granted to this service principal.
Supports $expand.
  - `[AppRoles <IMicrosoftGraphAppRole- `[]`>]`: The roles exposed by the application, which this service principal represents.
For more information, see the appRoles property definition on the application entity.
Not nullable.
    - `[AllowedMemberTypes <String- `[]`>]`: Specifies whether this app role can be assigned to users and groups (by setting to - `['User']`), to other application's (by setting to - `['Application']`, or both (by setting to - `['User', 'Application']`).
App roles supporting assignment to other applications' service principals are also known as application permissions.
The 'Application' value is only supported for app roles defined on application entities.
    - `[Description <String>]`: The description for the app role.
This is displayed when the app role is being assigned and, if the app role functions as an application permission, during  consent experiences.
    - `[DisplayName <String>]`: Display name for the permission that appears in the app role assignment and consent experiences.
    - `[Id <String>]`: Unique role identifier inside the appRoles collection.
You must specify a new GUID identifier when you create a new app role.
    - `[IsEnabled <Boolean?>]`: When you create or updating an app role, this value must be true.
To delete a role, this must first be set to false.
At that point, in a subsequent call, this role might be removed.
Default value is true.
    - `[Origin <String>]`: Specifies if the app role is defined on the application object or on the servicePrincipal entity.
Must not be included in any POST or PATCH requests.
Read-only.
    - `[Value <String>]`: Specifies the value to include in the roles claim in ID tokens and access tokens authenticating an assigned user or service principal.
Must not exceed 120 characters in length.
Allowed characters are : ! # $ % & ' ( ) * + , - . / : ;  =  ? @ \[ \] ^ + _  {  } ~, and characters in the ranges


@ - `[ ]` ^ + _  {  } ~, and characters in the ranges 0-9, A-Z, and a-z.
Any other character, including the space character, aren't allowed.
May not begin with ..
  - `[ApplicationTemplateId <String>]`: Unique identifier of the applicationTemplate.
Supports $filter (eq, not, ne).
Read-only.
null if the app wasn't created from an application template.
  - `[ClaimsMappingPolicies <IMicrosoftGraphClaimsMappingPolicy- `[]`>]`: The claimsMappingPolicies assigned to this service principal.
Supports $expand.
    - `[AppliesTo <IMicrosoftGraphDirectoryObject- `[]`>]`: 
    - `[Definition <String- `[]`>]`: A string collection containing a JSON string that defines the rules and settings for a policy.
The syntax for the definition differs for each derived policy type.
Required.
    - `[IsOrganizationDefault <Boolean?>]`: If set to true, activates this policy.
There can be many policies for the same policy type, but only one can be activated as the organization default.
Optional, default value is false.
    - `[Description <String>]`: Description for this policy.
Required.
    - `[DisplayName <String>]`: Display name for this policy.
Required.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ClaimsPolicy <IMicrosoftGraphCustomClaimsPolicy>]`: customClaimsPolicy
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AudienceOverride <String>]`: If specified, it overrides the content of the audience claim for WS-Federation and SAML2 protocols.
A custom signing key must be used for audienceOverride to be applied, otherwise, the audienceOverride value is ignored.
The value provided must be in the format of an absolute URI.
    - `[Claims <IMicrosoftGraphCustomClaimBase- `[]`>]`: Defines which claims are present in the tokens affected by the policy, in addition to the basic claim and the core claim set.
Inherited from customclaimbase.
      - `[Configurations <IMicrosoftGraphCustomClaimConfiguration- `[]`>]`: One or more configurations that describe how the claim is sourced and under what conditions.
        - `[Attribute <IMicrosoftGraphCustomClaimAttributeBase>]`: customClaimAttributeBase
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Condition <IMicrosoftGraphCustomClaimConditionBase>]`: customClaimConditionBase
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Transformations <IMicrosoftGraphCustomClaimTransformation- `[]`>]`: An ordered list of transformations that are applied in sequence.
          - `[Input <IMicrosoftGraphTransformationAttribute>]`: transformationAttribute
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
            - `[Attribute <IMicrosoftGraphCustomClaimAttributeBase>]`: customClaimAttributeBase
            - `[TreatAsMultiValue <Boolean?>]`: This flag is only relevant in the case where the attribute is multivalued.
By default, transformations are only applied to the first element in a multi-valued claim, however setting this flag to true ensures the transformation is applied to all values, resulting in a multivalued output.
    - `[IncludeApplicationIdInIssuer <Boolean?>]`: Indicates whether the application ID is added to the claim.
It is relevant only for SAML2.0 and if a custom signing key is used.
the default value is true.
Optional.
    - `[IncludeBasicClaimSet <Boolean?>]`: Determines whether the basic claim set is included in tokens affected by this policy.
If set to true, all claims in the basic claim set are emitted in tokens affected by the policy.
By default the basic claim set isn't in the tokens unless they're explicitly configured in this policy.
  - `[CreatedObjects <IMicrosoftGraphDirectoryObject- `[]`>]`: Directory objects created by this service principal.
Read-only.
Nullable.
  - `[CustomSecurityAttributes <IMicrosoftGraphCustomSecurityAttributeValue>]`: customSecurityAttributeValue
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DelegatedPermissionClassifications <IMicrosoftGraphDelegatedPermissionClassification- `[]`>]`: The permission classifications for delegated permissions exposed by the app that this service principal represents.
Supports $expand.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Classification <String>]`: permissionClassificationType
    - `[PermissionId <String>]`: The unique identifier (id) for the delegated permission listed in the publishedPermissionScopes collection of the servicePrincipal.
Required on create.
Doesn't support $filter.
    - `[PermissionName <String>]`: The claim value (value) for the delegated permission listed in the publishedPermissionScopes collection of the servicePrincipal.
Doesn't support $filter.
  - `[Description <String>]`: Free text field to provide an internal end-user facing description of the service principal.
End-user portals such MyApps displays the application description in this field.
The maximum allowed size is 1,024 characters.
Supports $filter (eq, ne, not, ge, le, startsWith) and $search.
  - `[DisabledByMicrosoftStatus <String>]`: Specifies whether Microsoft has disabled the registered application.
Possible values are: null (default value), NotDisabled, and DisabledDueToViolationOfServicesAgreement (reasons may include suspicious, abusive, or malicious activity, or a violation of the Microsoft Services Agreement). 
Supports $filter (eq, ne, not).
  - `[DisplayName <String>]`: The display name for the service principal.
Supports $filter (eq, ne, not, ge, le, in, startsWith, and eq on null values), $search, and $orderby.
  - `[Endpoints <IMicrosoftGraphEndpoint- `[]`>]`: Endpoints available for discovery.
Services like Sharepoint populate this property with a tenant specific SharePoint endpoints that other applications can discover and use in their experiences.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Capability <String>]`: Describes the capability that is associated with this resource.
(for example, Messages, Conversations, etc.) Not nullable.
Read-only.
    - `[ProviderId <String>]`: Application id of the publishing underlying service.
Not nullable.
Read-only.
    - `[ProviderName <String>]`: Name of the publishing underlying service.
Read-only.
    - `[ProviderResourceId <String>]`: For Microsoft 365 groups, this is set to a well-known name for the resource (for example, Yammer.FeedURL etc.).
Not nullable.
Read-only.
    - `[Uri <String>]`: URL of the published resource.
Not nullable.
Read-only.
  - `[ErrorUrl <String>]`: Deprecated.
Don't use.
  - `[FederatedIdentityCredentials <IMicrosoftGraphFederatedIdentityCredential- `[]`>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Audiences <String- `[]`>]`: The audience that can appear in the external token.
This field is mandatory and should be set to api://AzureADTokenExchange for Microsoft Entra ID.
It says what Microsoft identity platform should accept in the aud claim in the incoming token.
This value represents Microsoft Entra ID in your external identity provider and has no fixed value across identity providers - you may need to create a new application registration in your identity provider to serve as the audience of this token.
This field can only accept a single value and has a limit of 600 characters.
Required.
    - `[ClaimsMatchingExpression <IMicrosoftGraphFederatedIdentityExpression>]`: federatedIdentityExpression
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[LanguageVersion <Int32?>]`: Indicated the language version to be used.
Should always be set to 1.
Required.
      - `[Value <String>]`: Indicates the configured expression.
Required.
    - `[Description <String>]`: The un-validated, user-provided description of the federated identity credential.
It has a limit of 600 characters.
Optional.
    - `[Issuer <String>]`: The URL of the external identity provider and must match the issuer claim of the external token being exchanged.
The combination of the values of issuer and subject must be unique on the app.
It has a limit of 600 characters.
Required.
    - `[Name <String>]`: The unique identifier for the federated identity credential, which has a limit of 120 characters and must be URL friendly.
It is immutable once created.
Alternate key.
Required.
Not nullable.
Supports $filter (eq).
    - `[Subject <String>]`: Nullable. 
Defaults to null if not set.
The identifier of the external software workload within the external identity provider.
Like the audience value, it has no fixed format, as each identity provider uses their own - sometimes a GUID, sometimes a colon delimited identifier, sometimes arbitrary strings.
The value here must match the sub claim within the token presented to Microsoft Entra ID.
The combination of issuer and subject must be unique on the app.
It has a limit of 600 characters.
If subject is defined, claimsMatchingExpression must be null.
Supports $filter (eq).
  - `[HomeRealmDiscoveryPolicies <IMicrosoftGraphHomeRealmDiscoveryPolicy- `[]`>]`: The homeRealmDiscoveryPolicies assigned to this service principal.
Supports $expand.
    - `[AppliesTo <IMicrosoftGraphDirectoryObject- `[]`>]`: 
    - `[Definition <String- `[]`>]`: A string collection containing a JSON string that defines the rules and settings for a policy.
The syntax for the definition differs for each derived policy type.
Required.
    - `[IsOrganizationDefault <Boolean?>]`: If set to true, activates this policy.
There can be many policies for the same policy type, but only one can be activated as the organization default.
Optional, default value is false.
    - `[Description <String>]`: Description for this policy.
Required.
    - `[DisplayName <String>]`: Display name for this policy.
Required.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Homepage <String>]`: Home page or landing page of the application.
  - `[Info <IMicrosoftGraphInformationalUrl>]`: informationalUrl
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[LogoUrl <String>]`: CDN URL to the application's logo, Read-only.
    - `[MarketingUrl <String>]`: Link to the application's marketing page.
For example, https://www.contoso.com/app/marketing
    - `[PrivacyStatementUrl <String>]`: Link to the application's privacy statement.
For example, https://www.contoso.com/app/privacy
    - `[SupportUrl <String>]`: Link to the application's support page.
For example, https://www.contoso.com/app/support
    - `[TermsOfServiceUrl <String>]`: Link to the application's terms of service statement.
For example, https://www.contoso.com/app/termsofservice
  - `[KeyCredentials <IMicrosoftGraphKeyCredential- `[]`>]`: The collection of key credentials associated with the service principal.
Not nullable.
Supports $filter (eq, not, ge, le).
    - `[CustomKeyIdentifier <Byte- `[]`>]`: A 40-character binary type that can be used to identify the credential.
Optional.
When not provided in the payload, defaults to the thumbprint of the certificate.
    - `[DisplayName <String>]`: The friendly name for the key, with a maximum length of 90 characters.
Longer values are accepted but shortened.
Optional.
    - `[EndDateTime <DateTime?>]`: The date and time at which the credential expires.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[Key <Byte- `[]`>]`: Value for the key credential.
Should be a Base64 encoded value.
Returned only on $select for a single object, that is, GET applications/{applicationId}?$select=keyCredentials or GET servicePrincipals/{servicePrincipalId}?$select=keyCredentials; otherwise, it's always null. 
From a .cer certificate, you can read the key using the Convert.ToBase64String() method.
For more information, see Get the certificate key.
    - `[KeyId <String>]`: The unique identifier for the key.
    - `[StartDateTime <DateTime?>]`: The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[Type <String>]`: The type of key credential; for example, Symmetric, AsymmetricX509Cert, or X509CertAndPassword.
    - `[Usage <String>]`: A string that describes the purpose for which the key can be used; for example, None​, Verify​, PairwiseIdentifier​, Delegation​, Decrypt​, Encrypt​, HashedIdentifier​, SelfSignedTls, or Sign.
If usage is Sign​, the type should be X509CertAndPassword​, and the passwordCredentials​ for signing should be defined.
  - `[LicenseDetails <IMicrosoftGraphLicenseDetails- `[]`>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ServicePlans <IMicrosoftGraphServicePlanInfo- `[]`>]`: Information about the service plans assigned with the license.
Read-only.
Not nullable.
      - `[AppliesTo <String>]`: The object the service plan can be assigned to.
The possible values are: User - service plan can be assigned to individual users.Company - service plan can be assigned to the entire tenant.
      - `[ProvisioningStatus <String>]`: The provisioning status of the service plan.
The possible values are:Success - Service is fully provisioned.Disabled - Service is disabled.Error - The service plan isn't provisioned and is in an error state.PendingInput - The service isn't provisioned and is awaiting service confirmation.PendingActivation - The service is provisioned but requires explicit activation by an administrator (for example, Intune_O365 service plan)PendingProvisioning - Microsoft has added a new service to the product SKU and it isn't activated in the tenant.
      - `[ServicePlanId <String>]`: The unique identifier of the service plan.
      - `[ServicePlanName <String>]`: The name of the service plan.
    - `[SkuId <String>]`: Unique identifier (GUID) for the service SKU.
Equal to the skuId property on the related subscribedSku object.
Read-only.
    - `[SkuPartNumber <String>]`: Unique SKU display name.
Equal to the skuPartNumber on the related subscribedSku object; for example, AAD_Premium.
Read-only.
  - `[LoginUrl <String>]`: Specifies the URL where the service provider redirects the user to Microsoft Entra ID to authenticate.
Microsoft Entra ID uses the URL to launch the application from Microsoft 365 or the Microsoft Entra My Apps.
When blank, Microsoft Entra ID performs IdP-initiated sign-on for applications configured with SAML-based single sign-on.
The user launches the application from Microsoft 365, the Microsoft Entra My Apps, or the Microsoft Entra SSO URL.
  - `[LogoutUrl <String>]`: Specifies the URL that the Microsoft's authorization service uses to sign out a user using OpenId Connect front-channel, back-channel, or SAML sign out protocols.
  - `[MemberOf <IMicrosoftGraphDirectoryObject- `[]`>]`: Roles that this service principal is a member of.
HTTP Methods: GET Read-only.
Nullable.
Supports $expand.
  - `[Notes <String>]`: Free text field to capture information about the service principal, typically used for operational purposes.
Maximum allowed size is 1,024 characters.
  - `[NotificationEmailAddresses <String- `[]`>]`: Specifies the list of email addresses where Microsoft Entra ID sends a notification when the active certificate is near the expiration date.
This is only for the certificates used to sign the SAML token issued for Microsoft Entra Gallery applications.
  - `[Oauth2PermissionGrants <IMicrosoftGraphOAuth2PermissionGrant- `[]`>]`: Delegated permission grants authorizing this service principal to access an API on behalf of a signed-in user.
Read-only.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ClientId <String>]`: The object id (not appId) of the client service principal for the application that is authorized to act on behalf of a signed-in user when accessing an API.
Required.
Supports $filter (eq only).
    - `[ConsentType <String>]`: Indicates whether authorization is granted for the client application to impersonate all users or only a specific user.
AllPrincipals indicates authorization to impersonate all users.
Principal indicates authorization to impersonate a specific user.
Consent on behalf of all users can be granted by an administrator.
Nonadmin users may be authorized to consent on behalf of themselves in some cases, for some delegated permissions.
Required.
Supports $filter (eq only).
    - `[ExpiryTime <DateTime?>]`: Currently, the end time value is ignored, but a value is required when creating an oAuth2PermissionGrant.
Required.
    - `[PrincipalId <String>]`: The id of the user on behalf of whom the client is authorized to access the resource, when consentType is Principal.
If consentType is AllPrincipals this value is null.
Required when consentType is Principal.
Supports $filter (eq only).
    - `[ResourceId <String>]`: The id of the resource service principal to which access is authorized.
This identifies the API that the client is authorized to attempt to call on behalf of a signed-in user.
Supports $filter (eq only).
    - `[Scope <String>]`: A space-separated list of the claim values for delegated permissions that should be included in access tokens for the resource application (the API).
For example, openid User.Read GroupMember.Read.All.
Each claim value should match the value field of one of the delegated permissions defined by the API, listed in the publishedPermissionScopes property of the resource service principal.
Must not exceed 3850 characters in length.
    - `[StartTime <DateTime?>]`: Currently, the start time value is ignored, but a value is required when creating an oAuth2PermissionGrant.
Required.
  - `[OwnedObjects <IMicrosoftGraphDirectoryObject- `[]`>]`: Directory objects that are owned by this service principal.
Read-only.
Nullable.
Supports $expand and $filter (/$count eq 0, /$count ne 0, /$count eq 1, /$count ne 1).
  - `[Owners <IMicrosoftGraphDirectoryObject- `[]`>]`: Directory objects that are owners of this servicePrincipal.
The owners are a set of nonadmin users or servicePrincipals who are allowed to modify this object.
Supports $expand and $filter (/$count eq 0, /$count ne 0, /$count eq 1, /$count ne 1).
  - `[PasswordCredentials <IMicrosoftGraphPasswordCredential- `[]`>]`: The collection of password credentials associated with the service principal.
Not nullable.
    - `[CustomKeyIdentifier <Byte- `[]`>]`: Do not use.
    - `[DisplayName <String>]`: Friendly name for the password.
Optional.
    - `[EndDateTime <DateTime?>]`: The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Optional.
    - `[Hint <String>]`: Contains the first three characters of the password.
Read-only.
    - `[KeyId <String>]`: The unique identifier for the password.
    - `[SecretText <String>]`: Read-only; Contains the strong passwords generated by Microsoft Entra ID that are 16-64 characters in length.
The generated password value is only returned during the initial POST request to addPassword.
There is no way to retrieve this password in the future.
    - `[StartDateTime <DateTime?>]`: The date and time at which the password becomes valid.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Optional.
  - `[PasswordSingleSignOnSettings <IMicrosoftGraphPasswordSingleSignOnSettings>]`: passwordSingleSignOnSettings
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Fields <IMicrosoftGraphPasswordSingleSignOnField- `[]`>]`: The fields to capture to fill the user credentials for password-based single sign-on.
      - `[CustomizedLabel <String>]`: Title/label override for customization.
      - `[DefaultLabel <String>]`: Label that would be used if no customizedLabel is provided.
Read only.
      - `[FieldId <String>]`: Id used to identity the field type.
This is an internal ID and possible values are param1, param2, paramuserName, parampassword.
      - `[Type <String>]`: Type of the credential.
The values can be text, password.
  - `[PermissionGrantPreApprovalPolicies <IMicrosoftGraphPermissionGrantPreApprovalPolicy- `[]`>]`: 
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Conditions <IMicrosoftGraphPreApprovalDetail- `[]`>]`: A list of condition sets describing the conditions under which the permission to grant consent for the app has been preapproved.
      - `[Permissions <IMicrosoftGraphPreApprovedPermissions>]`: preApprovedPermissions
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[PermissionKind <String>]`: permissionKind
        - `[PermissionType <String>]`: permissionType
      - `[ScopeType <String>]`: resourceScopeType
      - `[SensitivityLabels <IMicrosoftGraphScopeSensitivityLabels>]`: scopeSensitivityLabels
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[LabelKind <String>]`: labelKind
  - `[PreferredSingleSignOnMode <String>]`: Specifies the single sign-on mode configured for this application.
Microsoft Entra ID uses the preferred single sign-on mode to launch the application from Microsoft 365 or the Microsoft Entra My Apps.
The supported values are password, saml, notSupported, and oidc.
Note: This field might be null for older SAML apps and for OIDC applications where it isn't set automatically.
  - `[PreferredTokenSigningKeyEndDateTime <DateTime?>]`: Specifies the expiration date of the keyCredential used for token signing, marked by preferredTokenSigningKeyThumbprint.
Updating this attribute isn't currently supported.
For details, see ServicePrincipal property differences.
  - `[PreferredTokenSigningKeyThumbprint <String>]`: This property can be used on SAML applications (apps that have preferredSingleSignOnMode set to saml) to control which certificate is used to sign the SAML responses.
For applications that aren't SAML, don't write or otherwise rely on this property.
  - `[PublishedPermissionScopes <IMicrosoftGraphPermissionScope- `[]`>]`: The delegated permissions exposed by the application.
For more information, see the oauth2PermissionScopes property on the application entity's api property.
Not nullable.
Note: This property is named oauth2PermissionScopes in v1.0.
    - `[AdminConsentDescription <String>]`: A description of the delegated permissions, intended to be read by an administrator granting the permission on behalf of all users.
This text appears in tenant-wide admin consent experiences.
    - `[AdminConsentDisplayName <String>]`: The permission's title, intended to be read by an administrator granting the permission on behalf of all users.
    - `[Id <String>]`: Unique delegated permission identifier inside the collection of delegated permissions defined for a resource application.
    - `[IsEnabled <Boolean?>]`: When you create or update a permission, this property must be set to true (which is the default).
To delete a permission, this property must first be set to false. 
At that point, in a subsequent call, the permission may be removed.
    - `[Origin <String>]`: 
    - `[Type <String>]`: The possible values are: User and Admin.
Specifies whether this delegated permission should be considered safe for non-admin users to consent to on behalf of themselves, or whether an administrator consent should always be required.
While Microsoft Graph defines the default consent requirement for each permission, the tenant administrator may override the behavior in their organization (by allowing, restricting, or limiting user consent to this delegated permission).
For more information, see Configure how users consent to applications.
    - `[UserConsentDescription <String>]`: A description of the delegated permissions, intended to be read by a user granting the permission on their own behalf.
This text appears in consent experiences where the user is consenting only on behalf of themselves.
    - `[UserConsentDisplayName <String>]`: A title for the permission, intended to be read by a user granting the permission on their own behalf.
This text appears in consent experiences where the user is consenting only on behalf of themselves.
    - `[Value <String>]`: Specifies the value to include in the scp (scope) claim in access tokens.
Must not exceed 120 characters in length.
Allowed characters are : ! # $ % & ' ( ) * + , - . / : ;  =  ? @ \[ \] ^ + _  {  } ~, and characters in the ranges


@ - `[ ]` ^ + _  {  } ~, and characters in the ranges 0-9, A-Z and a-z.
Any other character, including the space character, aren't allowed.
May not begin with ..
  - `[PublisherName <String>]`: The name of the Microsoft Entra tenant that published the application.
  - `[RemoteDesktopSecurityConfiguration <IMicrosoftGraphRemoteDesktopSecurityConfiguration>]`: remoteDesktopSecurityConfiguration
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[IsRemoteDesktopProtocolEnabled <Boolean?>]`: Determines if Microsoft Entra ID RDS authentication protocol for RDP is enabled.
    - `[TargetDeviceGroups <IMicrosoftGraphTargetDeviceGroup- `[]`>]`: The collection of target device groups that are associated with the RDS security configuration that will be enabled for SSO when a client connects to the target device over RDP using the new Microsoft Entra ID RDS authentication protocol.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[DisplayName <String>]`: Display name for the target device group.
  - `[ReplyUrls <String- `[]`>]`: The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.
Not nullable.
  - `[SamlMetadataUrl <String>]`: The url where the service exposes SAML metadata for federation.
  - `[SamlSingleSignOnSettings <IMicrosoftGraphSamlSingleSignOnSettings>]`: samlSingleSignOnSettings
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[RelayState <String>]`: The relative URI the service provider would redirect to after completion of the single sign-on flow.
  - `[ServicePrincipalNames <String- `[]`>]`: Contains the list of identifiersUris, copied over from the associated application.
More values can be added to hybrid applications.
These values can be used to identify the permissions exposed by this app within Microsoft Entra ID.
For example,Client apps can specify a resource URI that is based on the values of this property to acquire an access token, which is the URI returned in the 'aud' claim.The any operator is required for filter expressions on multi-valued properties.
Not nullable. 
Supports $filter (eq, not, ge, le, startsWith).
  - `[ServicePrincipalType <String>]`: Identifies if the service principal represents an application or a managed identity.
This is set by Microsoft Entra ID internally.
For a service principal that represents an application this is set as Application.
For a service principal that represents a managed identity this is set as ManagedIdentity.
The SocialIdp type is for internal use.
  - `[SignInAudience <String>]`: Specifies the Microsoft accounts that are supported for the current application.
Read-only.
Supported values are:AzureADMyOrg: Users with a Microsoft work or school account in my organization's Microsoft Entra tenant (single-tenant).AzureADMultipleOrgs: Users with a Microsoft work or school account in any organization's Microsoft Entra tenant (multitenant).AzureADandPersonalMicrosoftAccount: Users with a personal Microsoft account, or a work or school account in any organization's Microsoft Entra tenant.PersonalMicrosoftAccount: Users with a personal Microsoft account only.
  - `[Synchronization <IMicrosoftGraphSynchronization>]`: synchronization
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Jobs <IMicrosoftGraphSynchronizationJob- `[]`>]`: Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[BulkUpload <IMicrosoftGraphBulkUpload>]`: bulkUpload
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Schedule <IMicrosoftGraphSynchronizationSchedule>]`: synchronizationSchedule
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Expiration <DateTime?>]`: Date and time when this job will expire.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
        - `[Interval <TimeSpan?>]`: The interval between synchronization iterations.
The value is represented in ISO 8601  format for durations.
For example, P1M represents a period of one month and PT1M represents a period of one minute.
        - `[State <String>]`: synchronizationScheduleState
      - `[Schema <IMicrosoftGraphSynchronizationSchema>]`: synchronizationSchema
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
      - `[Status <IMicrosoftGraphSynchronizationStatus>]`: synchronizationStatus
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Code <String>]`: synchronizationStatusCode
        - `[CountSuccessiveCompleteFailures <Int64?>]`: Number of consecutive times this job failed.
        - `[EscrowsPruned <Boolean?>]`: true if the job's escrows (object-level errors) were pruned during initial synchronization.
Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.
Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.
When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.
        - `[LastExecution <IMicrosoftGraphSynchronizationTaskExecution>]`: synchronizationTaskExecution
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[ActivityIdentifier <String>]`: Identifier of the job run.
          - `[CountEntitled <Int64?>]`: Count of processed entries that were assigned for this application.
          - `[CountEntitledForProvisioning <Int64?>]`: Count of processed entries that were assigned for provisioning.
          - `[CountEscrowed <Int64?>]`: Count of entries that were escrowed (errors).
          - `[CountEscrowedRaw <Int64?>]`: Count of entries that were escrowed, including system-generated escrows.
          - `[CountExported <Int64?>]`: Count of exported entries.
          - `[CountExports <Int64?>]`: Count of entries that were expected to be exported.
          - `[CountImported <Int64?>]`: Count of imported entries.
          - `[CountImportedDeltas <Int64?>]`: Count of imported delta-changes.
          - `[CountImportedReferenceDeltas <Int64?>]`: Count of imported delta-changes pertaining to reference changes.
          - `[Error <IMicrosoftGraphSynchronizationError>]`: synchronizationError
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
            - `[Code <String>]`: The error code.
For example, AzureDirectoryB2BManagementPolicyCheckFailure.
            - `[Message <String>]`: The error message.
For example, Policy permitting auto-redemption of invitations not configured.
            - `[TenantActionable <Boolean?>]`: The action to take to resolve the error.
For example, false.
          - `[State <String>]`: synchronizationTaskExecutionResult
          - `[TimeBegan <DateTime?>]`: Time when this job run began.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
          - `[TimeEnded <DateTime?>]`: Time when this job run ended.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
        - `[LastSuccessfulExecution <IMicrosoftGraphSynchronizationTaskExecution>]`: synchronizationTaskExecution
        - `[LastSuccessfulExecutionWithExports <IMicrosoftGraphSynchronizationTaskExecution>]`: synchronizationTaskExecution
        - `[Progress <IMicrosoftGraphSynchronizationProgress- `[]`>]`: Details of the progress of a job toward completion.
          - `[CompletedUnits <Int64?>]`: The numerator of a progress ratio; the number of units of changes already processed.
          - `[ProgressObservationDateTime <DateTime?>]`: The time of a progress observation as an offset in minutes from UTC.
          - `[TotalUnits <Int64?>]`: The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.
          - `[Units <String>]`: An optional description of the units.
        - `[Quarantine <IMicrosoftGraphSynchronizationQuarantine>]`: synchronizationQuarantine
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[CurrentBegan <DateTime?>]`: Date and time when the quarantine was last evaluated and imposed.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
          - `[Error <IMicrosoftGraphSynchronizationError>]`: synchronizationError
          - `[NextAttempt <DateTime?>]`: Date and time when the next attempt to re-evaluate the quarantine will be made.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
          - `[Reason <String>]`: quarantineReason
          - `[SeriesBegan <DateTime?>]`: Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
          - `[SeriesCount <Int64?>]`: Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).
        - `[SteadyStateFirstAchievedTime <DateTime?>]`: The time when steady state (no more changes to the process) was first achieved.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
        - `[SteadyStateLastAchievedTime <DateTime?>]`: The time when steady state (no more changes to the process) was last achieved.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
        - `[SynchronizedEntryCountByType <IMicrosoftGraphStringKeyLongValuePair- `[]`>]`: Count of synchronized objects, listed by object type.
          - `[Key <String>]`: The mapping of the user type from the source system to the target system.
For example:User to User - For Microsoft Entra ID to Microsoft Entra synchronization worker to user - For Workday to Microsoft Entra synchronization.
          - `[Value <Int64?>]`: Total number of synchronized objects.
        - `[TroubleshootingUrl <String>]`: In the event of an error, the URL with the troubleshooting steps for the issue.
      - `[SynchronizationJobSettings <IMicrosoftGraphKeyValuePair- `[]`>]`: Settings associated with the job.
Some settings are inherited from the template.
        - `[Name <String>]`: Name for this key-value pair
        - `[Value <String>]`: Value for this key-value pair
      - `[TemplateId <String>]`: Identifier of the synchronization template this job is based on.
    - `[Secrets <IMicrosoftGraphSynchronizationSecretKeyStringValuePair- `[]`>]`: Represents a collection of credentials to access provisioned cloud applications.
      - `[Key <String>]`: synchronizationSecret
      - `[Value <String>]`: The value of the secret.
    - `[Templates <IMicrosoftGraphSynchronizationTemplate- `[]`>]`: Pre-configured synchronization settings for a particular application.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[ApplicationId <String>]`: Identifier of the application this template belongs to.
      - `[Default <Boolean?>]`: true if this template is recommended to be the default for the application.
      - `[Description <String>]`: Description of the template.
      - `[Discoverable <Boolean?>]`: true if this template should appear in the collection of templates available for the application instance (service principal).
      - `[FactoryTag <String>]`: One of the well-known factory tags supported by the synchronization engine.
The factoryTag tells the synchronization engine which implementation to use when processing jobs based on this template.
      - `[Metadata <IMicrosoftGraphSynchronizationMetadataEntry- `[]`>]`: Additional extension properties.
Unless mentioned explicitly, metadata values shouldn't be changed.
        - `[Key <String>]`: synchronizationMetadata
        - `[Value <String>]`: Value of the metadata property.
      - `[Schema <IMicrosoftGraphSynchronizationSchema>]`: synchronizationSchema
  - `[Tags <String- `[]`>]`: Custom strings that can be used to categorize and identify the service principal.
Not nullable.
The value is the union of strings set here and on the associated application entity's tags property.Supports $filter (eq, not, ge, le, startsWith).
  - `[TokenEncryptionKeyId <String>]`: Specifies the keyId of a public key from the keyCredentials collection.
When configured, Microsoft Entra ID issues tokens for this application encrypted using the key specified by this property.
The application code that receives the encrypted token must use the matching private key to decrypt the token before it can be used for the signed-in user.
  - `[TokenIssuancePolicies <IMicrosoftGraphTokenIssuancePolicy- `[]`>]`: The tokenIssuancePolicies assigned to this service principal.
Supports $expand.
    - `[AppliesTo <IMicrosoftGraphDirectoryObject- `[]`>]`: 
    - `[Definition <String- `[]`>]`: A string collection containing a JSON string that defines the rules and settings for a policy.
The syntax for the definition differs for each derived policy type.
Required.
    - `[IsOrganizationDefault <Boolean?>]`: If set to true, activates this policy.
There can be many policies for the same policy type, but only one can be activated as the organization default.
Optional, default value is false.
    - `[Description <String>]`: Description for this policy.
Required.
    - `[DisplayName <String>]`: Display name for this policy.
Required.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[TokenLifetimePolicies <IMicrosoftGraphTokenLifetimePolicy- `[]`>]`: The tokenLifetimePolicies assigned to this service principal.
Supports $expand.
    - `[AppliesTo <IMicrosoftGraphDirectoryObject- `[]`>]`: 
    - `[Definition <String- `[]`>]`: A string collection containing a JSON string that defines the rules and settings for a policy.
The syntax for the definition differs for each derived policy type.
Required.
    - `[IsOrganizationDefault <Boolean?>]`: If set to true, activates this policy.
There can be many policies for the same policy type, but only one can be activated as the organization default.
Optional, default value is false.
    - `[Description <String>]`: Description for this policy.
Required.
    - `[DisplayName <String>]`: Display name for this policy.
Required.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[TransitiveMemberOf <IMicrosoftGraphDirectoryObject- `[]`>]`: 
  - `[VerifiedPublisher <IMicrosoftGraphVerifiedPublisher>]`: verifiedPublisher
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AddedDateTime <DateTime?>]`: The timestamp when the verified publisher was first added or most recently updated.
    - `[DisplayName <String>]`: The verified publisher name from the app publisher's Microsoft Partner Network (MPN) account.
    - `[VerifiedPublisherId <String>]`: The ID of the verified publisher from the app publisher's Partner Center account.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.networkaccess/update-mgbetanetworkaccessconnectivitybranchforwardingprofile](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.networkaccess/update-mgbetanetworkaccessconnectivitybranchforwardingprofile)
























