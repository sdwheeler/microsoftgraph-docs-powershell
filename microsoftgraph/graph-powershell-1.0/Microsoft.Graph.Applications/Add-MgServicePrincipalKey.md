---
external help file: Microsoft.Graph.Applications-help.xml
Module Name: Microsoft.Graph.Applications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.applications/add-mgserviceprincipalkey
schema: 2.0.0
ms.subservice: entra-applications
---

# Add-MgServicePrincipalKey

## SYNOPSIS
Adds a key credential to a servicePrincipal.
This method along with removeKey can be used by a servicePrincipal to automate rolling its expiring keys.
As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.
ServicePrincipals that don't have any existing valid certificates (i.e.: no certificates have been added yet, or all certificates have expired), won't be able to use this service action.
Update servicePrincipal can be used to perform an update instead.

## SYNTAX

### AddExpanded (Default)
```
Add-MgServicePrincipalKey -ServicePrincipalId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-KeyCredential <IMicrosoftGraphKeyCredential>]
 [-PasswordCredential <IMicrosoftGraphPasswordCredential>] [-Proof <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Add
```
Add-MgServicePrincipalKey -ServicePrincipalId <String>
 -BodyParameter <IPathsN3Fx9GServiceprincipalsServiceprincipalIdMicrosoftGraphAddkeyPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### AddViaIdentityExpanded
```
Add-MgServicePrincipalKey -InputObject <IApplicationsIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-KeyCredential <IMicrosoftGraphKeyCredential>]
 [-PasswordCredential <IMicrosoftGraphPasswordCredential>] [-Proof <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### AddViaIdentity
```
Add-MgServicePrincipalKey -InputObject <IApplicationsIdentity>
 -BodyParameter <IPathsN3Fx9GServiceprincipalsServiceprincipalIdMicrosoftGraphAddkeyPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Adds a key credential to a servicePrincipal.
This method along with removeKey can be used by a servicePrincipal to automate rolling its expiring keys.
As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.
ServicePrincipals that don't have any existing valid certificates (i.e.: no certificates have been added yet, or all certificates have expired), won't be able to use this service action.
Update servicePrincipal can be used to perform an update instead.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Application.ReadWrite.All, Directory.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Application.ReadWrite.OwnedBy, Directory.ReadWrite.All, Application.ReadWrite.All,  |

## EXAMPLES
### Example 1: Adding a new key credential to a servicePrincipal

```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
	keyCredential = @{
		type = "AsymmetricX509Cert"
		usage = "Verify"
		key = [System.Text.Encoding]::ASCII.GetBytes("MIIDYDCCAki...")
	}
	passwordCredential = $null
	proof = "eyJ0eXAiOiJ..."
}

Add-MgServicePrincipalKey -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```
This example shows adding a new key credential to a serviceprincipal

### Example 2: Adding a key credential and an associated password for the key

```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
	keyCredential = @{
		type = "X509CertAndPassword"
		usage = "Sign"
		key = [System.Text.Encoding]::ASCII.GetBytes("MIIDYDCCAki...")
	}
	passwordCredential = @{
		secretText = "MKTr0w1..."
	}
	proof = "eyJ0eXAiOiJ..."
}

Add-MgServicePrincipalKey -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```
This example shows adding a key credential and an associated password for the key


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: AddExpanded, AddViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter

To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPathsN3Fx9GServiceprincipalsServiceprincipalIdMicrosoftGraphAddkeyPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Add, AddViaIdentity
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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IApplicationsIdentity
Parameter Sets: AddViaIdentityExpanded, AddViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -KeyCredential
keyCredential
To construct, see NOTES section for KEYCREDENTIAL properties and create a hash table.

```yaml
Type: IMicrosoftGraphKeyCredential
Parameter Sets: AddExpanded, AddViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PasswordCredential
passwordCredential
To construct, see NOTES section for PASSWORDCREDENTIAL properties and create a hash table.

```yaml
Type: IMicrosoftGraphPasswordCredential
Parameter Sets: AddExpanded, AddViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Proof


```yaml
Type: String
Parameter Sets: AddExpanded, AddViaIdentityExpanded
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

### -ServicePrincipalId
The unique identifier of servicePrincipal

```yaml
Type: String
Parameter Sets: AddExpanded, Add
Aliases:

Required: True
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

### Microsoft.Graph.PowerShell.Models.IApplicationsIdentity
### Microsoft.Graph.PowerShell.Models.IPathsN3Fx9GServiceprincipalsServiceprincipalIdMicrosoftGraphAddkeyPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphKeyCredential
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPathsN3Fx9GServiceprincipalsServiceprincipalIdMicrosoftGraphAddkeyPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[KeyCredential <IMicrosoftGraphKeyCredential>]`: keyCredential
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[CustomKeyIdentifier <Byte- `[]`>]`: A 40-character binary type that can be used to identify the credential.
Optional.
When not provided in the payload, defaults to the thumbprint of the certificate.
    - `[DisplayName <String>]`: The friendly name for the key, with a maximum length of 90 characters.
Longer values are accepted but shortened.
Optional.
    - `[EndDateTime <DateTime?>]`: The date and time at which the credential expires.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[Key <Byte- `[]`>]`: The certificate's raw data in byte array converted to Base64 string.
Returned only on $select for a single object, that is, GET applications/{applicationId}?$select=keyCredentials or GET servicePrincipals/{servicePrincipalId}?$select=keyCredentials; otherwise, it's always null.
From a .cer certificate, you can read the key using the Convert.ToBase64String() method.
For more information, see Get the certificate key.
    - `[KeyId <String>]`: The unique identifier (GUID) for the key.
    - `[StartDateTime <DateTime?>]`: The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[Type <String>]`: The type of key credential; for example, Symmetric, AsymmetricX509Cert.
    - `[Usage <String>]`: A string that describes the purpose for which the key can be used; for example, Verify.
  - `[PasswordCredential <IMicrosoftGraphPasswordCredential>]`: passwordCredential
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
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
  - `[Proof <String>]`:

INPUTOBJECT `<IApplicationsIdentity>`: Identity Parameter
  - `[AppId <String>]`: Alternate key of application
  - `[AppManagementPolicyId <String>]`: The unique identifier of appManagementPolicy
  - `[AppRoleAssignmentId <String>]`: The unique identifier of appRoleAssignment
  - `[ApplicationId <String>]`: The unique identifier of application
  - `[ApplicationTemplateId <String>]`: The unique identifier of applicationTemplate
  - `[ClaimsMappingPolicyId <String>]`: The unique identifier of claimsMappingPolicy
  - `[DelegatedPermissionClassificationId <String>]`: The unique identifier of delegatedPermissionClassification
  - `[DirectoryDefinitionId <String>]`: The unique identifier of directoryDefinition
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[EndpointId <String>]`: The unique identifier of endpoint
  - `[ExtensionPropertyId <String>]`: The unique identifier of extensionProperty
  - `[FederatedIdentityCredentialId <String>]`: The unique identifier of federatedIdentityCredential
  - `[GroupId <String>]`: The unique identifier of group
  - `[HomeRealmDiscoveryPolicyId <String>]`: The unique identifier of homeRealmDiscoveryPolicy
  - `[Name <String>]`: Alternate key of federatedIdentityCredential
  - `[OAuth2PermissionGrantId <String>]`: The unique identifier of oAuth2PermissionGrant
  - `[ServicePrincipalId <String>]`: The unique identifier of servicePrincipal
  - `[SynchronizationJobId <String>]`: The unique identifier of synchronizationJob
  - `[SynchronizationTemplateId <String>]`: The unique identifier of synchronizationTemplate
  - `[TargetDeviceGroupId <String>]`: The unique identifier of targetDeviceGroup
  - `[TokenIssuancePolicyId <String>]`: The unique identifier of tokenIssuancePolicy
  - `[TokenLifetimePolicyId <String>]`: The unique identifier of tokenLifetimePolicy
  - `[UniqueName <String>]`: Alternate key of application
  - `[UserId <String>]`: The unique identifier of user

KEYCREDENTIAL `<IMicrosoftGraphKeyCredential>`: keyCredential
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[CustomKeyIdentifier <Byte- `[]`>]`: A 40-character binary type that can be used to identify the credential.
Optional.
When not provided in the payload, defaults to the thumbprint of the certificate.
  - `[DisplayName <String>]`: The friendly name for the key, with a maximum length of 90 characters.
Longer values are accepted but shortened.
Optional.
  - `[EndDateTime <DateTime?>]`: The date and time at which the credential expires.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[Key <Byte- `[]`>]`: The certificate's raw data in byte array converted to Base64 string.
Returned only on $select for a single object, that is, GET applications/{applicationId}?$select=keyCredentials or GET servicePrincipals/{servicePrincipalId}?$select=keyCredentials; otherwise, it's always null.
From a .cer certificate, you can read the key using the Convert.ToBase64String() method.
For more information, see Get the certificate key.
  - `[KeyId <String>]`: The unique identifier (GUID) for the key.
  - `[StartDateTime <DateTime?>]`: The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[Type <String>]`: The type of key credential; for example, Symmetric, AsymmetricX509Cert.
  - `[Usage <String>]`: A string that describes the purpose for which the key can be used; for example, Verify.

PASSWORDCREDENTIAL `<IMicrosoftGraphPasswordCredential>`: passwordCredential
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
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

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.applications/add-mgserviceprincipalkey](https://learn.microsoft.com/powershell/module/microsoft.graph.applications/add-mgserviceprincipalkey)

[https://learn.microsoft.com/graph/api/serviceprincipal-addkey?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/serviceprincipal-addkey?view=graph-rest-1.0)























