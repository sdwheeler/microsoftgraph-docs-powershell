---
external help file: Microsoft.Graph.Beta.Identity.Governance-help.xml
Module Name: Microsoft.Graph.Beta.Identity.Governance
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/new-mgbetaentitlementmanagementaccesspackageresourcerequest
schema: 2.0.0
ms.subservice: entra-id-governance
---

# New-MgBetaEntitlementManagementAccessPackageResourceRequest

## SYNOPSIS
Create a new accessPackageResourceRequest object to request the addition of a resource to an access package catalog, update of a resource, or the removal of a resource from a catalog.
A resource must be included in an access package catalog before a role of that resource can be added to an access package.

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaEntitlementManagementAccessPackageResourceRequest [-ResponseHeadersVariable <String>]
 [-AccessPackageResource <IMicrosoftGraphAccessPackageResource>] [-AdditionalProperties <Hashtable>]
 [-CatalogId <String>] [-ExecuteImmediately] [-ExpirationDateTime <DateTime>] [-Id <String>]
 [-IsValidationOnly] [-Justification <String>] [-RequestState <String>] [-RequestStatus <String>]
 [-RequestType <String>] [-Requestor <IMicrosoftGraphAccessPackageSubject>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaEntitlementManagementAccessPackageResourceRequest
 -BodyParameter <IMicrosoftGraphAccessPackageResourceRequest> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new accessPackageResourceRequest object to request the addition of a resource to an access package catalog, update of a resource, or the removal of a resource from a catalog.
A resource must be included in an access package catalog before a role of that resource can be added to an access package.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | EntitlementManagement.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | EntitlementManagement.ReadWrite.All,  |

## EXAMPLES
### Example 1: Create a new access package resource request

```powershell
Connect-MgGraph -Scopes 'EntitlementManagement.ReadWrite.All', 'Group.ReadWrite.All'
$accessPackageResource = @{
  "originSystem" = "AadGroup "
  OriginId= "b5cd9d19-91c0-4622-93e2-537ad8a0b3ad"
  }
New-MgBetaEntitlementManagementAccessPackageResourceRequest -CatalogId '54152ecb-c65d-47f2-8a4d-ba2732de0a7b' -RequestType "AdminAdd" -AccessPackageResource $accessPackageResource

AccessPackageResource : Microsoft.Graph.PowerShell.Models.MicrosoftGraphAccessPackageResource
CatalogId             : 54152ecb-c65d-47f2-8a4d-ba2732de0a7b
ExecuteImmediately    : False
ExpirationDateTime    :
Id                    : 88098a60-489a-4c28-bfe7-9fecd4713b81
IsValidationOnly      :
Justification         :
RequestState          : Delivered
RequestStatus         : Fulfilled
RequestType           : AdminAdd
Requestor             : Microsoft.Graph.PowerShell.Models.MicrosoftGraphAccessPackageSubject
AdditionalProperties  : {[@odata.context, https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceRequests/$entity]}                                                            
```

This example creates a new resource request for addition of a resource to an access package catalog.

## PARAMETERS

### -AccessPackageResource
accessPackageResource
To construct, see NOTES section for ACCESSPACKAGERESOURCE properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessPackageResource
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
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

### -BodyParameter
accessPackageResourceRequest
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessPackageResourceRequest
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CatalogId
The unique ID of the access package catalog.

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

### -ExecuteImmediately


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

### -ExpirationDateTime
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z

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

### -IsValidationOnly
If set, doesn't add the resource.

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

### -Justification
The requestor's justification for adding or removing the resource.

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

### -Requestor
accessPackageSubject
To construct, see NOTES section for REQUESTOR properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessPackageSubject
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RequestState
The outcome of whether the service was able to add the resource to the catalog.
The value is Delivered if the resource was added or removed.
Read-Only.

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

### -RequestStatus


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

### -RequestType
Use AdminAdd to add a resource, if the caller is an administrator or resource owner, AdminUpdate to update a resource, or AdminRemove to remove a resource.

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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAccessPackageResourceRequest
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAccessPackageResourceRequest
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ACCESSPACKAGERESOURCE `<IMicrosoftGraphAccessPackageResource>`: accessPackageResource
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AccessPackageResourceEnvironment <IMicrosoftGraphAccessPackageResourceEnvironment>]`: accessPackageResourceEnvironment
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AccessPackageResources <IMicrosoftGraphAccessPackageResource- `[]`>]`: Read-only.
Required.
    - `[ConnectionInfo <IMicrosoftGraphConnectionInfo>]`: connectionInfo
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Url <String>]`: The endpoint that is used by Entitlement Management to communicate with the access package resource.
    - `[CreatedBy <String>]`: The display name of the user that created this object.
    - `[CreatedDateTime <DateTime?>]`: The date and time that this object was created.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[Description <String>]`: The description of this object.
    - `[DisplayName <String>]`: The display name of this object.
    - `[IsDefaultEnvironment <Boolean?>]`: Determines whether this is default environment or not.
It is set to true for all static origin systems, such as Microsoft Entra groups and Microsoft Entra Applications.
    - `[ModifiedBy <String>]`: The display name of the entity that last modified this object.
    - `[ModifiedDateTime <DateTime?>]`: The date and time that this object was last modified.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[OriginId <String>]`: The unique identifier of this environment in the origin system.
    - `[OriginSystem <String>]`: The type of the resource in the origin system, that is, SharePointOnline.
Requires $filter (eq).
  - `[AccessPackageResourceRoles <IMicrosoftGraphAccessPackageResourceRole- `[]`>]`: Read-only.
Nullable.
Supports $expand.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AccessPackageResource <IMicrosoftGraphAccessPackageResource>]`: accessPackageResource
    - `[Description <String>]`: A description for the resource role.
    - `[DisplayName <String>]`: The display name of the resource role such as the role defined by the application.
    - `[OriginId <String>]`: The unique identifier of the resource role in the origin system.
For a SharePoint Online site, the originId is the sequence number of the role in the site.
    - `[OriginSystem <String>]`: The type of the resource in the origin system, such as SharePointOnline, AadApplication or AadGroup.
  - `[AccessPackageResourceScopes <IMicrosoftGraphAccessPackageResourceScope- `[]`>]`: Read-only.
Nullable.
Supports $expand.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AccessPackageResource <IMicrosoftGraphAccessPackageResource>]`: accessPackageResource
    - `[Description <String>]`: The description of the scope.
    - `[DisplayName <String>]`: The display name of the scope.
    - `[IsRootScope <Boolean?>]`: True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.
    - `[OriginId <String>]`: The unique identifier for the scope in the resource as defined in the origin system.
    - `[OriginSystem <String>]`: The origin system for the scope.
    - `[RoleOriginId <String>]`: The origin system for the role, if different.
    - `[Url <String>]`: A resource locator for the scope.
  - `[AddedBy <String>]`: The name of the user or application that first added this resource.
Read-only.
  - `[AddedOn <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
  - `[Attributes <IMicrosoftGraphAccessPackageResourceAttribute- `[]`>]`: Contains information about the attributes to be collected from the requestor and sent to the resource application.
    - `[AttributeDestination <IMicrosoftGraphAccessPackageResourceAttributeDestination>]`: accessPackageResourceAttributeDestination
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AttributeName <String>]`: The name of the attribute in the end system.
If the destination is accessPackageUserDirectoryAttributeStore, then a user property such as jobTitle or a directory schema extension for the user object type, such as extension2b676109c7c74ae2b41549205f1947edpersonalTitle.
    - `[AttributeSource <IMicrosoftGraphAccessPackageResourceAttributeSource>]`: accessPackageResourceAttributeSource
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: Unique identifier for the attribute on the access package resource.
Read-only.
    - `[IsEditable <Boolean?>]`: Specifies whether or not an existing attribute value can be edited by the requester.
    - `[IsPersistedOnAssignmentRemoval <Boolean?>]`: Specifies whether the attribute will remain in the end system after an assignment ends.
  - `[Description <String>]`: A description for the resource.
  - `[DisplayName <String>]`: The display name of the resource, such as the application name, group name, or site name.
  - `[IsPendingOnboarding <Boolean?>]`: True if the resource is not yet available for assignment.
Read-only.
  - `[OriginId <String>]`: The unique identifier of the resource in the origin system.
In the case of a Microsoft Entra group, originId is the identifier of the group.
Supports $filter (eq).
  - `[OriginSystem <String>]`: The type of the resource in the origin system, such as SharePointOnline, AadApplication, or AadGroup.
Supports $filter (eq).
  - `[ResourceType <String>]`: The type of the resource, such as Application if it is a Microsoft Entra connected application, or SharePoint Online Site for a SharePoint Online site.
  - `[Url <String>]`: A unique resource locator for the resource, such as the URL for signing a user into an application.

BODYPARAMETER `<IMicrosoftGraphAccessPackageResourceRequest>`: accessPackageResourceRequest
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AccessPackageResource <IMicrosoftGraphAccessPackageResource>]`: accessPackageResource
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AccessPackageResourceEnvironment <IMicrosoftGraphAccessPackageResourceEnvironment>]`: accessPackageResourceEnvironment
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AccessPackageResources <IMicrosoftGraphAccessPackageResource- `[]`>]`: Read-only.
Required.
      - `[ConnectionInfo <IMicrosoftGraphConnectionInfo>]`: connectionInfo
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Url <String>]`: The endpoint that is used by Entitlement Management to communicate with the access package resource.
      - `[CreatedBy <String>]`: The display name of the user that created this object.
      - `[CreatedDateTime <DateTime?>]`: The date and time that this object was created.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
      - `[Description <String>]`: The description of this object.
      - `[DisplayName <String>]`: The display name of this object.
      - `[IsDefaultEnvironment <Boolean?>]`: Determines whether this is default environment or not.
It is set to true for all static origin systems, such as Microsoft Entra groups and Microsoft Entra Applications.
      - `[ModifiedBy <String>]`: The display name of the entity that last modified this object.
      - `[ModifiedDateTime <DateTime?>]`: The date and time that this object was last modified.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
      - `[OriginId <String>]`: The unique identifier of this environment in the origin system.
      - `[OriginSystem <String>]`: The type of the resource in the origin system, that is, SharePointOnline.
Requires $filter (eq).
    - `[AccessPackageResourceRoles <IMicrosoftGraphAccessPackageResourceRole- `[]`>]`: Read-only.
Nullable.
Supports $expand.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AccessPackageResource <IMicrosoftGraphAccessPackageResource>]`: accessPackageResource
      - `[Description <String>]`: A description for the resource role.
      - `[DisplayName <String>]`: The display name of the resource role such as the role defined by the application.
      - `[OriginId <String>]`: The unique identifier of the resource role in the origin system.
For a SharePoint Online site, the originId is the sequence number of the role in the site.
      - `[OriginSystem <String>]`: The type of the resource in the origin system, such as SharePointOnline, AadApplication or AadGroup.
    - `[AccessPackageResourceScopes <IMicrosoftGraphAccessPackageResourceScope- `[]`>]`: Read-only.
Nullable.
Supports $expand.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AccessPackageResource <IMicrosoftGraphAccessPackageResource>]`: accessPackageResource
      - `[Description <String>]`: The description of the scope.
      - `[DisplayName <String>]`: The display name of the scope.
      - `[IsRootScope <Boolean?>]`: True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.
      - `[OriginId <String>]`: The unique identifier for the scope in the resource as defined in the origin system.
      - `[OriginSystem <String>]`: The origin system for the scope.
      - `[RoleOriginId <String>]`: The origin system for the role, if different.
      - `[Url <String>]`: A resource locator for the scope.
    - `[AddedBy <String>]`: The name of the user or application that first added this resource.
Read-only.
    - `[AddedOn <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
    - `[Attributes <IMicrosoftGraphAccessPackageResourceAttribute- `[]`>]`: Contains information about the attributes to be collected from the requestor and sent to the resource application.
      - `[AttributeDestination <IMicrosoftGraphAccessPackageResourceAttributeDestination>]`: accessPackageResourceAttributeDestination
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[AttributeName <String>]`: The name of the attribute in the end system.
If the destination is accessPackageUserDirectoryAttributeStore, then a user property such as jobTitle or a directory schema extension for the user object type, such as extension2b676109c7c74ae2b41549205f1947edpersonalTitle.
      - `[AttributeSource <IMicrosoftGraphAccessPackageResourceAttributeSource>]`: accessPackageResourceAttributeSource
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: Unique identifier for the attribute on the access package resource.
Read-only.
      - `[IsEditable <Boolean?>]`: Specifies whether or not an existing attribute value can be edited by the requester.
      - `[IsPersistedOnAssignmentRemoval <Boolean?>]`: Specifies whether the attribute will remain in the end system after an assignment ends.
    - `[Description <String>]`: A description for the resource.
    - `[DisplayName <String>]`: The display name of the resource, such as the application name, group name, or site name.
    - `[IsPendingOnboarding <Boolean?>]`: True if the resource is not yet available for assignment.
Read-only.
    - `[OriginId <String>]`: The unique identifier of the resource in the origin system.
In the case of a Microsoft Entra group, originId is the identifier of the group.
Supports $filter (eq).
    - `[OriginSystem <String>]`: The type of the resource in the origin system, such as SharePointOnline, AadApplication, or AadGroup.
Supports $filter (eq).
    - `[ResourceType <String>]`: The type of the resource, such as Application if it is a Microsoft Entra connected application, or SharePoint Online Site for a SharePoint Online site.
    - `[Url <String>]`: A unique resource locator for the resource, such as the URL for signing a user into an application.
  - `[CatalogId <String>]`: The unique ID of the access package catalog.
  - `[ExecuteImmediately <Boolean?>]`: 
  - `[ExpirationDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[IsValidationOnly <Boolean?>]`: If set, doesn't add the resource.
  - `[Justification <String>]`: The requestor's justification for adding or removing the resource.
  - `[RequestState <String>]`: The outcome of whether the service was able to add the resource to the catalog.
The value is Delivered if the resource was added or removed.
Read-Only.
  - `[RequestStatus <String>]`: 
  - `[RequestType <String>]`: Use AdminAdd to add a resource, if the caller is an administrator or resource owner, AdminUpdate to update a resource, or AdminRemove to remove a resource.
  - `[Requestor <IMicrosoftGraphAccessPackageSubject>]`: accessPackageSubject
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AltSecId <String>]`: Not Supported.
    - `[CleanupScheduledDateTime <DateTime?>]`: The date and time the subject is marked to be blocked from sign in or deleted.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
    - `[ConnectedOrganization <IMicrosoftGraphConnectedOrganization>]`: connectedOrganization
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[CreatedBy <String>]`: UPN of the user who created this resource.
Read-only.
      - `[CreatedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
      - `[Description <String>]`: The description of the connected organization.
      - `[DisplayName <String>]`: The display name of the connected organization.
Supports $filter (eq).
      - `[ExternalSponsors <IMicrosoftGraphDirectoryObject- `[]`>]`: 
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
      - `[IdentitySources <IMicrosoftGraphIdentitySource- `[]`>]`: The identity sources in this connected organization, one of azureActiveDirectoryTenant, crossCloudAzureActiveDirectoryTenant, domainIdentitySource, externalDomainFederation, or socialIdentitySource.
Read-only.
Nullable.
Supports $select and $filter(eq).
To filter by the derived types, you must declare the resource using its full OData cast, for example, $filter=identitySources/any(is:is/microsoft.graph.azureActiveDirectoryTenant/tenantId eq 'bcfdfff4-cbc3-43f2-9000-ba7b7515054f').
      - `[InternalSponsors <IMicrosoftGraphDirectoryObject- `[]`>]`: 
      - `[ModifiedBy <String>]`: UPN of the user who last modified this resource.
Read-only.
      - `[ModifiedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
      - `[State <String>]`: connectedOrganizationState
    - `[ConnectedOrganizationId <String>]`: The identifier of the connected organization of the subject.
    - `[DisplayName <String>]`: The display name of the subject.
    - `[Email <String>]`: The email address of the subject.
    - `[ObjectId <String>]`: The object identifier of the subject.
null if the subject isn't yet a user in the tenant.
Alternate key.
    - `[OnPremisesSecurityIdentifier <String>]`: A string representation of the principal's security identifier, if known, or null if the subject doesn't have a security identifier.
    - `[PrincipalName <String>]`: The principal name, if known, of the subject.
    - `[SubjectLifecycle <String>]`: accessPackageSubjectLifecycle
    - `[Type <String>]`: The resource type of the subject.

REQUESTOR `<IMicrosoftGraphAccessPackageSubject>`: accessPackageSubject
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AltSecId <String>]`: Not Supported.
  - `[CleanupScheduledDateTime <DateTime?>]`: The date and time the subject is marked to be blocked from sign in or deleted.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
  - `[ConnectedOrganization <IMicrosoftGraphConnectedOrganization>]`: connectedOrganization
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[CreatedBy <String>]`: UPN of the user who created this resource.
Read-only.
    - `[CreatedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
    - `[Description <String>]`: The description of the connected organization.
    - `[DisplayName <String>]`: The display name of the connected organization.
Supports $filter (eq).
    - `[ExternalSponsors <IMicrosoftGraphDirectoryObject- `[]`>]`: 
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[IdentitySources <IMicrosoftGraphIdentitySource- `[]`>]`: The identity sources in this connected organization, one of azureActiveDirectoryTenant, crossCloudAzureActiveDirectoryTenant, domainIdentitySource, externalDomainFederation, or socialIdentitySource.
Read-only.
Nullable.
Supports $select and $filter(eq).
To filter by the derived types, you must declare the resource using its full OData cast, for example, $filter=identitySources/any(is:is/microsoft.graph.azureActiveDirectoryTenant/tenantId eq 'bcfdfff4-cbc3-43f2-9000-ba7b7515054f').
    - `[InternalSponsors <IMicrosoftGraphDirectoryObject- `[]`>]`: 
    - `[ModifiedBy <String>]`: UPN of the user who last modified this resource.
Read-only.
    - `[ModifiedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Read-only.
    - `[State <String>]`: connectedOrganizationState
  - `[ConnectedOrganizationId <String>]`: The identifier of the connected organization of the subject.
  - `[DisplayName <String>]`: The display name of the subject.
  - `[Email <String>]`: The email address of the subject.
  - `[ObjectId <String>]`: The object identifier of the subject.
null if the subject isn't yet a user in the tenant.
Alternate key.
  - `[OnPremisesSecurityIdentifier <String>]`: A string representation of the principal's security identifier, if known, or null if the subject doesn't have a security identifier.
  - `[PrincipalName <String>]`: The principal name, if known, of the subject.
  - `[SubjectLifecycle <String>]`: accessPackageSubjectLifecycle
  - `[Type <String>]`: The resource type of the subject.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/new-mgbetaentitlementmanagementaccesspackageresourcerequest](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/new-mgbetaentitlementmanagementaccesspackageresourcerequest)

[https://learn.microsoft.com/graph/api/entitlementmanagement-post-accesspackageresourcerequests?view=graph-rest-beta](https://learn.microsoft.com/graph/api/entitlementmanagement-post-accesspackageresourcerequests?view=graph-rest-beta)























