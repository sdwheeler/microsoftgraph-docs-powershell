---
external help file: Microsoft.Graph.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgoauth2permissiongrant
schema: 2.0.0
ms.subservice: entra-applications
---

# New-MgOauth2PermissionGrant

## SYNOPSIS
Create a delegated permission grant represented by an oAuth2PermissionGrant object.
A delegated permission grant authorizes a client service principal (representing a client application) to access a resource service principal (representing an API), on behalf of a signed-in user, for the level of access limited by the delegated permissions which were granted.

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaOauth2PermissionGrant](/powershell/module/Microsoft.Graph.Beta.Identity.SignIns/New-MgBetaOauth2PermissionGrant?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgOauth2PermissionGrant [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-ClientId <String>] [-ConsentType <String>] [-Id <String>] [-PrincipalId <String>] [-ResourceId <String>]
 [-Scope <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Create
```
New-MgOauth2PermissionGrant -BodyParameter <IMicrosoftGraphOAuth2PermissionGrant>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a delegated permission grant represented by an oAuth2PermissionGrant object.
A delegated permission grant authorizes a client service principal (representing a client application) to access a resource service principal (representing an API), on behalf of a signed-in user, for the level of access limited by the delegated permissions which were granted.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	clientId = "ef969797-201d-4f6b-960c-e9ed5f31dab5"
	consentType = "AllPrincipals"
	resourceId = "943603e4-e787-4fe9-93d1-e30f749aae39"
	scope = "DelegatedPermissionGrant.ReadWrite.All"
}

New-MgOauth2PermissionGrant -BodyParameter $params

```
This example shows how to use the New-MgOauth2PermissionGrant Cmdlet.


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
oAuth2PermissionGrant
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphOAuth2PermissionGrant
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ClientId
The object id (not appId) of the client service principal for the application that's authorized to act on behalf of a signed-in user when accessing an API.
Required.
Supports $filter (eq only).

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

### -ConsentType
Indicates if authorization is granted for the client application to impersonate all users or only a specific user.
AllPrincipals indicates authorization to impersonate all users.
Principal indicates authorization to impersonate a specific user.
Consent on behalf of all users can be granted by an administrator.
Nonadmin users might be authorized to consent on behalf of themselves in some cases, for some delegated permissions.
Required.
Supports $filter (eq only).

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

### -PrincipalId
The id of the user on behalf of whom the client is authorized to access the resource, when consentType is Principal.
If consentType is AllPrincipals this value is null.
Required when consentType is Principal.
Supports $filter (eq only).

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

### -ResourceId
The id of the resource service principal to which access is authorized.
This identifies the API that the client is authorized to attempt to call on behalf of a signed-in user.
Supports $filter (eq only).

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

### -Scope
A space-separated list of the claim values for delegated permissions that should be included in access tokens for the resource application (the API).
For example, openid User.Read GroupMember.Read.All.
Each claim value should match the value field of one of the delegated permissions defined by the API, listed in the oauth2PermissionScopes property of the resource service principal.
Must not exceed 3,850 characters in length.

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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphOAuth2PermissionGrant
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphOAuth2PermissionGrant
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphOAuth2PermissionGrant>`: oAuth2PermissionGrant
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ClientId <String>]`: The object id (not appId) of the client service principal for the application that's authorized to act on behalf of a signed-in user when accessing an API.
Required.
Supports $filter (eq only).
  - `[ConsentType <String>]`: Indicates if authorization is granted for the client application to impersonate all users or only a specific user.
AllPrincipals indicates authorization to impersonate all users.
Principal indicates authorization to impersonate a specific user.
Consent on behalf of all users can be granted by an administrator.
Nonadmin users might be authorized to consent on behalf of themselves in some cases, for some delegated permissions.
Required.
Supports $filter (eq only).
  - `[PrincipalId <String>]`: The id of the user on behalf of whom the client is authorized to access the resource, when consentType is Principal.
If consentType is AllPrincipals this value is null.
Required when consentType is Principal.
Supports $filter (eq only).
  - `[ResourceId <String>]`: The id of the resource service principal to which access is authorized.
This identifies the API that the client is authorized to attempt to call on behalf of a signed-in user.
Supports $filter (eq only).
  - `[Scope <String>]`: A space-separated list of the claim values for delegated permissions that should be included in access tokens for the resource application (the API).
For example, openid User.Read GroupMember.Read.All.
Each claim value should match the value field of one of the delegated permissions defined by the API, listed in the oauth2PermissionScopes property of the resource service principal.
Must not exceed 3,850 characters in length.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgoauth2permissiongrant](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgoauth2permissiongrant)

[https://learn.microsoft.com/graph/api/oauth2permissiongrant-post?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/oauth2permissiongrant-post?view=graph-rest-1.0)























