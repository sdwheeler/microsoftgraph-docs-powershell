---
external help file: Microsoft.Graph.Beta.Applications-help.xml
Module Name: Microsoft.Graph.Beta.Applications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/update-mgbetaapplicationfederatedidentitycredentialbyname
schema: 2.0.0
ms.subservice: entra-applications
---

# Update-MgBetaApplicationFederatedIdentityCredentialByName

## SYNOPSIS
Create a new federatedIdentityCredential object for an application if it doesn't exist, or update the properties of an existing federatedIdentityCredential object.
By configuring a trust relationship between your Microsoft Entra application registration and the identity provider for your compute platform, you can use tokens issued by that platform to authenticate with Microsoft identity platform and call APIs in the Microsoft ecosystem.
Maximum of 20 objects can be added to an application.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgApplicationFederatedIdentityCredentialByName](/powershell/module/Microsoft.Graph.Applications/Update-MgApplicationFederatedIdentityCredentialByName?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaApplicationFederatedIdentityCredentialByName -ApplicationId <String> -Name <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-Audiences <String[]>]
 [-ClaimsMatchingExpression <IMicrosoftGraphFederatedIdentityExpression>] [-Description <String>]
 [-Id <String>] [-Issuer <String>] [-Name1 <String>] [-Subject <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaApplicationFederatedIdentityCredentialByName -ApplicationId <String> -Name <String>
 -BodyParameter <IMicrosoftGraphFederatedIdentityCredential> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaApplicationFederatedIdentityCredentialByName [-Name <String>] -InputObject <IApplicationsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-Audiences <String[]>]
 [-ClaimsMatchingExpression <IMicrosoftGraphFederatedIdentityExpression>] [-Description <String>]
 [-Id <String>] [-Issuer <String>] [-Subject <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaApplicationFederatedIdentityCredentialByName -InputObject <IApplicationsIdentity>
 -BodyParameter <IMicrosoftGraphFederatedIdentityCredential> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new federatedIdentityCredential object for an application if it doesn't exist, or update the properties of an existing federatedIdentityCredential object.
By configuring a trust relationship between your Microsoft Entra application registration and the identity provider for your compute platform, you can use tokens issued by that platform to authenticate with Microsoft identity platform and call APIs in the Microsoft ecosystem.
Maximum of 20 objects can be added to an application.

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

### -ApplicationId
The unique identifier of application

```yaml
Type: String
Parameter Sets: UpdateExpanded, Update
Aliases: ObjectId

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Audiences
The audience that can appear in the external token.
This field is mandatory and should be set to api://AzureADTokenExchange for Microsoft Entra ID.
It says what Microsoft identity platform should accept in the aud claim in the incoming token.
This value represents Microsoft Entra ID in your external identity provider and has no fixed value across identity providers - you may need to create a new application registration in your identity provider to serve as the audience of this token.
This field can only accept a single value and has a limit of 600 characters.
Required.

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

### -BodyParameter
federatedIdentityCredential
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphFederatedIdentityCredential
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ClaimsMatchingExpression
federatedIdentityExpression
To construct, see NOTES section for CLAIMSMATCHINGEXPRESSION properties and create a hash table.

```yaml
Type: IMicrosoftGraphFederatedIdentityExpression
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

### -Description
The un-validated, user-provided description of the federated identity credential.
It has a limit of 600 characters.
Optional.

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

### -Issuer
The URL of the external identity provider and must match the issuer claim of the external token being exchanged.
The combination of the values of issuer and subject must be unique on the app.
It has a limit of 600 characters.
Required.

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

### -Name
Alternate key of federatedIdentityCredential

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

### -Name1
The unique identifier for the federated identity credential, which has a limit of 120 characters and must be URL friendly.
It is immutable once created.
Alternate key.
Required.
Not nullable.
Supports $filter (eq).

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

### -Subject
Nullable.
Defaults to null if not set.
The identifier of the external software workload within the external identity provider.
Like the audience value, it has no fixed format, as each identity provider uses their own - sometimes a GUID, sometimes a colon delimited identifier, sometimes arbitrary strings.
The value here must match the sub claim within the token presented to Microsoft Entra ID.
The combination of issuer and subject must be unique on the app.
It has a limit of 600 characters.
If subject is defined, claimsMatchingExpression must be null.
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
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphFederatedIdentityCredential
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphFederatedIdentityCredential
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphFederatedIdentityCredential>`: federatedIdentityCredential
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
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

CLAIMSMATCHINGEXPRESSION `<IMicrosoftGraphFederatedIdentityExpression>`: federatedIdentityExpression
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[LanguageVersion <Int32?>]`: Indicated the language version to be used.
Should always be set to 1.
Required.
  - `[Value <String>]`: Indicates the configured expression.
Required.

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

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/update-mgbetaapplicationfederatedidentitycredentialbyname](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.applications/update-mgbetaapplicationfederatedidentitycredentialbyname)

[https://learn.microsoft.com/graph/api/federatedidentitycredential-upsert?view=graph-rest-beta](https://learn.microsoft.com/graph/api/federatedidentitycredential-upsert?view=graph-rest-beta)
























