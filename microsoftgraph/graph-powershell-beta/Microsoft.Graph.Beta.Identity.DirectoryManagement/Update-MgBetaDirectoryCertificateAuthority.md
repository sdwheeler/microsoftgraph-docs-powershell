---
external help file: Microsoft.Graph.Beta.Identity.DirectoryManagement-help.xml
Module Name: Microsoft.Graph.Beta.Identity.DirectoryManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/update-mgbetadirectorycertificateauthority
schema: 2.0.0
---

# Update-MgBetaDirectoryCertificateAuthority

## SYNOPSIS
Update the navigation property certificateAuthorities in directory

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaDirectoryCertificateAuthority [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>]
 [-CertificateBasedApplicationConfigurations <IMicrosoftGraphCertificateBasedApplicationConfiguration[]>]
 [-Id <String>] [-MutualTlsOauthConfigurations <IMicrosoftGraphMutualTlsOauthConfiguration[]>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaDirectoryCertificateAuthority -BodyParameter <IMicrosoftGraphCertificateAuthorityPath>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property certificateAuthorities in directory

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
certificateAuthorityPath
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphCertificateAuthorityPath
Parameter Sets: Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CertificateBasedApplicationConfigurations
Defines the trusted certificate authorities for certificates that can be added to apps and service principals in the tenant.
To construct, see NOTES section for CERTIFICATEBASEDAPPLICATIONCONFIGURATIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphCertificateBasedApplicationConfiguration[]
Parameter Sets: UpdateExpanded
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
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MutualTlsOauthConfigurations
Defines the trusted certificate authorities for certificates that can be added to Internet of Things (IoT) devices.
To construct, see NOTES section for MUTUALTLSOAUTHCONFIGURATIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphMutualTlsOauthConfiguration[]
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphCertificateAuthorityPath
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphCertificateAuthorityPath
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphCertificateAuthorityPath>`: certificateAuthorityPath
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[CertificateBasedApplicationConfigurations <IMicrosoftGraphCertificateBasedApplicationConfiguration- `[]`>]`: Defines the trusted certificate authorities for certificates that can be added to apps and service principals in the tenant.
    - `[TrustedCertificateAuthorities <IMicrosoftGraphCertificateAuthorityAsEntity- `[]`>]`: Collection of trusted certificate authorities.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Certificate <Byte- `[]`>]`: The trusted certificate.
      - `[IsRootAuthority <Boolean?>]`: Indicates if the certificate is a root authority.
In a certificateBasedApplicationConfiguration object, at least one object in the trustedCertificateAuthorities collection must be a root authority.
      - `[Issuer <String>]`: The issuer of the trusted certificate.
      - `[IssuerSubjectKeyIdentifier <String>]`: The subject key identifier of the trusted certificate.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Description <String>]`: The description of the trusted certificate authorities.
    - `[DisplayName <String>]`: The display name of the trusted certificate authorities.
  - `[MutualTlsOauthConfigurations <IMicrosoftGraphMutualTlsOauthConfiguration- `[]`>]`: Defines the trusted certificate authorities for certificates that can be added to Internet of Things (IoT) devices.
    - `[CertificateAuthorities <IMicrosoftGraphCertificateAuthority- `[]`>]`: Multi-value property that represents a list of trusted certificate authorities.
      - `[Certificate <Byte- `[]`>]`: Required.
The base64 encoded string representing the public certificate.
      - `[CertificateRevocationListUrl <String>]`: The URL of the certificate revocation list.
      - `[DeltaCertificateRevocationListUrl <String>]`: The URL contains the list of all revoked certificates since the last time a full certificate revocaton list was created.
      - `[IsRootAuthority <Boolean?>]`: Required.
true if the trusted certificate is a root authority, false if the trusted certificate is an intermediate authority.
      - `[Issuer <String>]`: The issuer of the certificate, calculated from the certificate value.
Read-only.
      - `[IssuerSki <String>]`: The subject key identifier of the certificate, calculated from the certificate value.
Read-only.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: Friendly name.
Supports $filter (eq, in).
    - `[TlsClientAuthParameter <String>]`: tlsClientRegistrationMetadata

CERTIFICATEBASEDAPPLICATIONCONFIGURATIONS `<IMicrosoftGraphCertificateBasedApplicationConfiguration- `[]`>`: Defines the trusted certificate authorities for certificates that can be added to apps and service principals in the tenant.
  - `[TrustedCertificateAuthorities <IMicrosoftGraphCertificateAuthorityAsEntity- `[]`>]`: Collection of trusted certificate authorities.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Certificate <Byte- `[]`>]`: The trusted certificate.
    - `[IsRootAuthority <Boolean?>]`: Indicates if the certificate is a root authority.
In a certificateBasedApplicationConfiguration object, at least one object in the trustedCertificateAuthorities collection must be a root authority.
    - `[Issuer <String>]`: The issuer of the trusted certificate.
    - `[IssuerSubjectKeyIdentifier <String>]`: The subject key identifier of the trusted certificate.
  - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Description <String>]`: The description of the trusted certificate authorities.
  - `[DisplayName <String>]`: The display name of the trusted certificate authorities.

MUTUALTLSOAUTHCONFIGURATIONS `<IMicrosoftGraphMutualTlsOauthConfiguration- `[]`>`: Defines the trusted certificate authorities for certificates that can be added to Internet of Things (IoT) devices.
  - `[CertificateAuthorities <IMicrosoftGraphCertificateAuthority- `[]`>]`: Multi-value property that represents a list of trusted certificate authorities.
    - `[Certificate <Byte- `[]`>]`: Required.
The base64 encoded string representing the public certificate.
    - `[CertificateRevocationListUrl <String>]`: The URL of the certificate revocation list.
    - `[DeltaCertificateRevocationListUrl <String>]`: The URL contains the list of all revoked certificates since the last time a full certificate revocaton list was created.
    - `[IsRootAuthority <Boolean?>]`: Required.
true if the trusted certificate is a root authority, false if the trusted certificate is an intermediate authority.
    - `[Issuer <String>]`: The issuer of the certificate, calculated from the certificate value.
Read-only.
    - `[IssuerSki <String>]`: The subject key identifier of the certificate, calculated from the certificate value.
Read-only.
  - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DisplayName <String>]`: Friendly name.
Supports $filter (eq, in).
  - `[TlsClientAuthParameter <String>]`: tlsClientRegistrationMetadata

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/update-mgbetadirectorycertificateauthority](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.directorymanagement/update-mgbetadirectorycertificateauthority)
























