---
external help file: Microsoft.Graph.Identity.Governance-help.xml
Module Name: Microsoft.Graph.Identity.Governance
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/update-mgagreement
schema: 2.0.0
---

# Update-MgAgreement

## SYNOPSIS
Update entity in agreements

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaAgreement](/powershell/module/Microsoft.Graph.Beta.Identity.Governance/Update-MgBetaAgreement?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgAgreement -AgreementId <String> [-ResponseHeadersVariable <String>]
 [-Acceptances <IMicrosoftGraphAgreementAcceptance[]>] [-AdditionalProperties <Hashtable>]
 [-DisplayName <String>] [-File <IMicrosoftGraphAgreementFile>]
 [-Files <IMicrosoftGraphAgreementFileLocalization[]>] [-Id <String>] [-IsPerDeviceAcceptanceRequired]
 [-IsViewingBeforeAcceptanceRequired] [-TermsExpiration <IMicrosoftGraphTermsExpiration>]
 [-UserReacceptRequiredFrequency <TimeSpan>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgAgreement -AgreementId <String> -BodyParameter <IMicrosoftGraphAgreement>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgAgreement -InputObject <IIdentityGovernanceIdentity> [-ResponseHeadersVariable <String>]
 [-Acceptances <IMicrosoftGraphAgreementAcceptance[]>] [-AdditionalProperties <Hashtable>]
 [-DisplayName <String>] [-File <IMicrosoftGraphAgreementFile>]
 [-Files <IMicrosoftGraphAgreementFileLocalization[]>] [-Id <String>] [-IsPerDeviceAcceptanceRequired]
 [-IsViewingBeforeAcceptanceRequired] [-TermsExpiration <IMicrosoftGraphTermsExpiration>]
 [-UserReacceptRequiredFrequency <TimeSpan>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgAgreement -InputObject <IIdentityGovernanceIdentity> -BodyParameter <IMicrosoftGraphAgreement>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update entity in agreements

## EXAMPLES

## PARAMETERS

### -Acceptances
Read-only.
Information about acceptances of this agreement.
To construct, see NOTES section for ACCEPTANCES properties and create a hash table.

```yaml
Type: IMicrosoftGraphAgreementAcceptance[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AgreementId
The unique identifier of agreement

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

### -BodyParameter
agreement
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAgreement
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

### -DisplayName
Display name of the agreement.
The display name is used for internal tracking of the agreement but isn't shown to end users who view the agreement.
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

### -File
agreementFile
To construct, see NOTES section for FILE properties and create a hash table.

```yaml
Type: IMicrosoftGraphAgreementFile
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Files
PDFs linked to this agreement.
This property is in the process of being deprecated.
Use the file property instead.
Supports $expand.
To construct, see NOTES section for FILES properties and create a hash table.

```yaml
Type: IMicrosoftGraphAgreementFileLocalization[]
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
Type: IIdentityGovernanceIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -IsPerDeviceAcceptanceRequired
Indicates whether end users are required to accept this agreement on every device that they access it from.
The end user is required to register their device in Microsoft Entra ID, if they haven't already done so.
Supports $filter (eq).

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

### -IsViewingBeforeAcceptanceRequired
Indicates whether the user has to expand the agreement before accepting.
Supports $filter (eq).

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

### -TermsExpiration
termsExpiration
To construct, see NOTES section for TERMSEXPIRATION properties and create a hash table.

```yaml
Type: IMicrosoftGraphTermsExpiration
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserReacceptRequiredFrequency
The duration after which the user must reaccept the terms of use.
The value is represented in ISO 8601 format for durations.
Supports $filter (eq).

```yaml
Type: TimeSpan
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

### Microsoft.Graph.PowerShell.Models.IIdentityGovernanceIdentity
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAgreement
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAgreement
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ACCEPTANCES `<IMicrosoftGraphAgreementAcceptance- `[]`>`: Read-only.
Information about acceptances of this agreement.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AgreementFileId <String>]`: The identifier of the agreement file accepted by the user.
  - `[AgreementId <String>]`: The identifier of the agreement.
  - `[DeviceDisplayName <String>]`: The display name of the device used for accepting the agreement.
  - `[DeviceId <String>]`: The unique identifier of the device used for accepting the agreement.
Supports $filter (eq) and eq for null values.
  - `[DeviceOSType <String>]`: The operating system used to accept the agreement.
  - `[DeviceOSVersion <String>]`: The operating system version of the device used to accept the agreement.
  - `[ExpirationDateTime <DateTime?>]`: The expiration date time of the acceptance.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Supports $filter (eq, ge, le) and eq for null values.
  - `[RecordedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[State <String>]`: agreementAcceptanceState
  - `[UserDisplayName <String>]`: Display name of the user when the acceptance was recorded.
  - `[UserEmail <String>]`: Email of the user when the acceptance was recorded.
  - `[UserId <String>]`: The identifier of the user who accepted the agreement.
Supports $filter (eq).
  - `[UserPrincipalName <String>]`: UPN of the user when the acceptance was recorded.

BODYPARAMETER `<IMicrosoftGraphAgreement>`: agreement
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Acceptances <IMicrosoftGraphAgreementAcceptance- `[]`>]`: Read-only.
Information about acceptances of this agreement.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AgreementFileId <String>]`: The identifier of the agreement file accepted by the user.
    - `[AgreementId <String>]`: The identifier of the agreement.
    - `[DeviceDisplayName <String>]`: The display name of the device used for accepting the agreement.
    - `[DeviceId <String>]`: The unique identifier of the device used for accepting the agreement.
Supports $filter (eq) and eq for null values.
    - `[DeviceOSType <String>]`: The operating system used to accept the agreement.
    - `[DeviceOSVersion <String>]`: The operating system version of the device used to accept the agreement.
    - `[ExpirationDateTime <DateTime?>]`: The expiration date time of the acceptance.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Supports $filter (eq, ge, le) and eq for null values.
    - `[RecordedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[State <String>]`: agreementAcceptanceState
    - `[UserDisplayName <String>]`: Display name of the user when the acceptance was recorded.
    - `[UserEmail <String>]`: Email of the user when the acceptance was recorded.
    - `[UserId <String>]`: The identifier of the user who accepted the agreement.
Supports $filter (eq).
    - `[UserPrincipalName <String>]`: UPN of the user when the acceptance was recorded.
  - `[DisplayName <String>]`: Display name of the agreement.
The display name is used for internal tracking of the agreement but isn't shown to end users who view the agreement.
Supports $filter (eq).
  - `[File <IMicrosoftGraphAgreementFile>]`: agreementFile
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[CreatedDateTime <DateTime?>]`: The date time representing when the file was created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[DisplayName <String>]`: Localized display name of the policy file of an agreement.
The localized display name is shown to end users who view the agreement.
    - `[FileData <IMicrosoftGraphAgreementFileData>]`: agreementFileData
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Data <Byte- `[]`>]`: Data that represents the terms of use PDF document.
Read-only.
    - `[FileName <String>]`: Name of the agreement file (for example, TOU.pdf).
Read-only.
    - `[IsDefault <Boolean?>]`: If none of the languages matches the client preference, indicates whether this is the default agreement file.
If none of the files are marked as default, the first one is treated as the default.
Read-only.
    - `[IsMajorVersion <Boolean?>]`: Indicates whether the agreement file is a major version update.
Major version updates invalidate the agreement's acceptances on the corresponding language.
    - `[Language <String>]`: The language of the agreement file in the format 'languagecode2-country/regioncode2'.
'languagecode2' is a lowercase two-letter code derived from ISO 639-1, while 'country/regioncode2' is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag.
For example, U.S.
English is en-US.
Read-only.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Localizations <IMicrosoftGraphAgreementFileLocalization- `[]`>]`: The localized version of the terms of use agreement files attached to the agreement.
      - `[CreatedDateTime <DateTime?>]`: The date time representing when the file was created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
      - `[DisplayName <String>]`: Localized display name of the policy file of an agreement.
The localized display name is shown to end users who view the agreement.
      - `[FileData <IMicrosoftGraphAgreementFileData>]`: agreementFileData
      - `[FileName <String>]`: Name of the agreement file (for example, TOU.pdf).
Read-only.
      - `[IsDefault <Boolean?>]`: If none of the languages matches the client preference, indicates whether this is the default agreement file.
If none of the files are marked as default, the first one is treated as the default.
Read-only.
      - `[IsMajorVersion <Boolean?>]`: Indicates whether the agreement file is a major version update.
Major version updates invalidate the agreement's acceptances on the corresponding language.
      - `[Language <String>]`: The language of the agreement file in the format 'languagecode2-country/regioncode2'.
'languagecode2' is a lowercase two-letter code derived from ISO 639-1, while 'country/regioncode2' is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag.
For example, U.S.
English is en-US.
Read-only.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Versions <IMicrosoftGraphAgreementFileVersion- `[]`>]`: Read-only.
Customized versions of the terms of use agreement in the Microsoft Entra tenant.
        - `[CreatedDateTime <DateTime?>]`: The date time representing when the file was created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
        - `[DisplayName <String>]`: Localized display name of the policy file of an agreement.
The localized display name is shown to end users who view the agreement.
        - `[FileData <IMicrosoftGraphAgreementFileData>]`: agreementFileData
        - `[FileName <String>]`: Name of the agreement file (for example, TOU.pdf).
Read-only.
        - `[IsDefault <Boolean?>]`: If none of the languages matches the client preference, indicates whether this is the default agreement file.
If none of the files are marked as default, the first one is treated as the default.
Read-only.
        - `[IsMajorVersion <Boolean?>]`: Indicates whether the agreement file is a major version update.
Major version updates invalidate the agreement's acceptances on the corresponding language.
        - `[Language <String>]`: The language of the agreement file in the format 'languagecode2-country/regioncode2'.
'languagecode2' is a lowercase two-letter code derived from ISO 639-1, while 'country/regioncode2' is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag.
For example, U.S.
English is en-US.
Read-only.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Files <IMicrosoftGraphAgreementFileLocalization- `[]`>]`: PDFs linked to this agreement.
This property is in the process of being deprecated.
Use the  file property instead.
Supports $expand.
  - `[IsPerDeviceAcceptanceRequired <Boolean?>]`: Indicates whether end users are required to accept this agreement on every device that they access it from.
The end user is required to register their device in Microsoft Entra ID, if they haven't already done so.
Supports $filter (eq).
  - `[IsViewingBeforeAcceptanceRequired <Boolean?>]`: Indicates whether the user has to expand the agreement before accepting.
Supports $filter (eq).
  - `[TermsExpiration <IMicrosoftGraphTermsExpiration>]`: termsExpiration
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Frequency <TimeSpan?>]`: Represents the frequency at which the terms will expire, after its first expiration as set in startDateTime.
The value is represented in ISO 8601 format for durations.
For example, PT1M represents a time period of one month.
    - `[StartDateTime <DateTime?>]`: The DateTime when the agreement is set to expire for all users.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[UserReacceptRequiredFrequency <TimeSpan?>]`: The duration after which the user must reaccept the terms of use.
The value is represented in ISO 8601 format for durations.
Supports $filter (eq).

FILE `<IMicrosoftGraphAgreementFile>`: agreementFile
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[CreatedDateTime <DateTime?>]`: The date time representing when the file was created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[DisplayName <String>]`: Localized display name of the policy file of an agreement.
The localized display name is shown to end users who view the agreement.
  - `[FileData <IMicrosoftGraphAgreementFileData>]`: agreementFileData
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Data <Byte- `[]`>]`: Data that represents the terms of use PDF document.
Read-only.
  - `[FileName <String>]`: Name of the agreement file (for example, TOU.pdf).
Read-only.
  - `[IsDefault <Boolean?>]`: If none of the languages matches the client preference, indicates whether this is the default agreement file.
If none of the files are marked as default, the first one is treated as the default.
Read-only.
  - `[IsMajorVersion <Boolean?>]`: Indicates whether the agreement file is a major version update.
Major version updates invalidate the agreement's acceptances on the corresponding language.
  - `[Language <String>]`: The language of the agreement file in the format 'languagecode2-country/regioncode2'.
'languagecode2' is a lowercase two-letter code derived from ISO 639-1, while 'country/regioncode2' is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag.
For example, U.S.
English is en-US.
Read-only.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Localizations <IMicrosoftGraphAgreementFileLocalization- `[]`>]`: The localized version of the terms of use agreement files attached to the agreement.
    - `[CreatedDateTime <DateTime?>]`: The date time representing when the file was created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[DisplayName <String>]`: Localized display name of the policy file of an agreement.
The localized display name is shown to end users who view the agreement.
    - `[FileData <IMicrosoftGraphAgreementFileData>]`: agreementFileData
    - `[FileName <String>]`: Name of the agreement file (for example, TOU.pdf).
Read-only.
    - `[IsDefault <Boolean?>]`: If none of the languages matches the client preference, indicates whether this is the default agreement file.
If none of the files are marked as default, the first one is treated as the default.
Read-only.
    - `[IsMajorVersion <Boolean?>]`: Indicates whether the agreement file is a major version update.
Major version updates invalidate the agreement's acceptances on the corresponding language.
    - `[Language <String>]`: The language of the agreement file in the format 'languagecode2-country/regioncode2'.
'languagecode2' is a lowercase two-letter code derived from ISO 639-1, while 'country/regioncode2' is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag.
For example, U.S.
English is en-US.
Read-only.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Versions <IMicrosoftGraphAgreementFileVersion- `[]`>]`: Read-only.
Customized versions of the terms of use agreement in the Microsoft Entra tenant.
      - `[CreatedDateTime <DateTime?>]`: The date time representing when the file was created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
      - `[DisplayName <String>]`: Localized display name of the policy file of an agreement.
The localized display name is shown to end users who view the agreement.
      - `[FileData <IMicrosoftGraphAgreementFileData>]`: agreementFileData
      - `[FileName <String>]`: Name of the agreement file (for example, TOU.pdf).
Read-only.
      - `[IsDefault <Boolean?>]`: If none of the languages matches the client preference, indicates whether this is the default agreement file.
If none of the files are marked as default, the first one is treated as the default.
Read-only.
      - `[IsMajorVersion <Boolean?>]`: Indicates whether the agreement file is a major version update.
Major version updates invalidate the agreement's acceptances on the corresponding language.
      - `[Language <String>]`: The language of the agreement file in the format 'languagecode2-country/regioncode2'.
'languagecode2' is a lowercase two-letter code derived from ISO 639-1, while 'country/regioncode2' is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag.
For example, U.S.
English is en-US.
Read-only.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.

FILES `<IMicrosoftGraphAgreementFileLocalization- `[]`>`: PDFs linked to this agreement.
This property is in the process of being deprecated.
Use the file property instead.
Supports $expand.
  - `[CreatedDateTime <DateTime?>]`: The date time representing when the file was created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[DisplayName <String>]`: Localized display name of the policy file of an agreement.
The localized display name is shown to end users who view the agreement.
  - `[FileData <IMicrosoftGraphAgreementFileData>]`: agreementFileData
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Data <Byte- `[]`>]`: Data that represents the terms of use PDF document.
Read-only.
  - `[FileName <String>]`: Name of the agreement file (for example, TOU.pdf).
Read-only.
  - `[IsDefault <Boolean?>]`: If none of the languages matches the client preference, indicates whether this is the default agreement file.
If none of the files are marked as default, the first one is treated as the default.
Read-only.
  - `[IsMajorVersion <Boolean?>]`: Indicates whether the agreement file is a major version update.
Major version updates invalidate the agreement's acceptances on the corresponding language.
  - `[Language <String>]`: The language of the agreement file in the format 'languagecode2-country/regioncode2'.
'languagecode2' is a lowercase two-letter code derived from ISO 639-1, while 'country/regioncode2' is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag.
For example, U.S.
English is en-US.
Read-only.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Versions <IMicrosoftGraphAgreementFileVersion- `[]`>]`: Read-only.
Customized versions of the terms of use agreement in the Microsoft Entra tenant.
    - `[CreatedDateTime <DateTime?>]`: The date time representing when the file was created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
    - `[DisplayName <String>]`: Localized display name of the policy file of an agreement.
The localized display name is shown to end users who view the agreement.
    - `[FileData <IMicrosoftGraphAgreementFileData>]`: agreementFileData
    - `[FileName <String>]`: Name of the agreement file (for example, TOU.pdf).
Read-only.
    - `[IsDefault <Boolean?>]`: If none of the languages matches the client preference, indicates whether this is the default agreement file.
If none of the files are marked as default, the first one is treated as the default.
Read-only.
    - `[IsMajorVersion <Boolean?>]`: Indicates whether the agreement file is a major version update.
Major version updates invalidate the agreement's acceptances on the corresponding language.
    - `[Language <String>]`: The language of the agreement file in the format 'languagecode2-country/regioncode2'.
'languagecode2' is a lowercase two-letter code derived from ISO 639-1, while 'country/regioncode2' is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag.
For example, U.S.
English is en-US.
Read-only.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.

INPUTOBJECT `<IIdentityGovernanceIdentity>`: Identity Parameter
  - `[AccessPackageAssignmentId <String>]`: The unique identifier of accessPackageAssignment
  - `[AccessPackageAssignmentPolicyId <String>]`: The unique identifier of accessPackageAssignmentPolicy
  - `[AccessPackageAssignmentRequestId <String>]`: The unique identifier of accessPackageAssignmentRequest
  - `[AccessPackageCatalogId <String>]`: The unique identifier of accessPackageCatalog
  - `[AccessPackageId <String>]`: The unique identifier of accessPackage
  - `[AccessPackageId1 <String>]`: The unique identifier of accessPackage
  - `[AccessPackageQuestionId <String>]`: The unique identifier of accessPackageQuestion
  - `[AccessPackageResourceEnvironmentId <String>]`: The unique identifier of accessPackageResourceEnvironment
  - `[AccessPackageResourceId <String>]`: The unique identifier of accessPackageResource
  - `[AccessPackageResourceRequestId <String>]`: The unique identifier of accessPackageResourceRequest
  - `[AccessPackageResourceRoleId <String>]`: The unique identifier of accessPackageResourceRole
  - `[AccessPackageResourceRoleId1 <String>]`: The unique identifier of accessPackageResourceRole
  - `[AccessPackageResourceRoleScopeId <String>]`: The unique identifier of accessPackageResourceRoleScope
  - `[AccessPackageResourceScopeId <String>]`: The unique identifier of accessPackageResourceScope
  - `[AccessPackageResourceScopeId1 <String>]`: The unique identifier of accessPackageResourceScope
  - `[AccessReviewHistoryDefinitionId <String>]`: The unique identifier of accessReviewHistoryDefinition
  - `[AccessReviewHistoryInstanceId <String>]`: The unique identifier of accessReviewHistoryInstance
  - `[AccessReviewInstanceDecisionItemId <String>]`: The unique identifier of accessReviewInstanceDecisionItem
  - `[AccessReviewInstanceId <String>]`: The unique identifier of accessReviewInstance
  - `[AccessReviewReviewerId <String>]`: The unique identifier of accessReviewReviewer
  - `[AccessReviewScheduleDefinitionId <String>]`: The unique identifier of accessReviewScheduleDefinition
  - `[AccessReviewStageId <String>]`: The unique identifier of accessReviewStage
  - `[AgreementAcceptanceId <String>]`: The unique identifier of agreementAcceptance
  - `[AgreementFileLocalizationId <String>]`: The unique identifier of agreementFileLocalization
  - `[AgreementFileVersionId <String>]`: The unique identifier of agreementFileVersion
  - `[AgreementId <String>]`: The unique identifier of agreement
  - `[AppConsentRequestId <String>]`: The unique identifier of appConsentRequest
  - `[ApprovalId <String>]`: The unique identifier of approval
  - `[ApprovalStageId <String>]`: The unique identifier of approvalStage
  - `[ConnectedOrganizationId <String>]`: The unique identifier of connectedOrganization
  - `[CustomCalloutExtensionId <String>]`: The unique identifier of customCalloutExtension
  - `[CustomExtensionStageSettingId <String>]`: The unique identifier of customExtensionStageSetting
  - `[CustomTaskExtensionId <String>]`: The unique identifier of customTaskExtension
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[EndDateTime <DateTime?>]`: Usage: endDateTime={endDateTime}
  - `[GovernanceInsightId <String>]`: The unique identifier of governanceInsight
  - `[IncompatibleAccessPackageId <String>]`: Usage: incompatibleAccessPackageId='{incompatibleAccessPackageId}'
  - `[On <String>]`: Usage: on='{on}'
  - `[PrivilegedAccessGroupAssignmentScheduleId <String>]`: The unique identifier of privilegedAccessGroupAssignmentSchedule
  - `[PrivilegedAccessGroupAssignmentScheduleInstanceId <String>]`: The unique identifier of privilegedAccessGroupAssignmentScheduleInstance
  - `[PrivilegedAccessGroupAssignmentScheduleRequestId <String>]`: The unique identifier of privilegedAccessGroupAssignmentScheduleRequest
  - `[PrivilegedAccessGroupEligibilityScheduleId <String>]`: The unique identifier of privilegedAccessGroupEligibilitySchedule
  - `[PrivilegedAccessGroupEligibilityScheduleInstanceId <String>]`: The unique identifier of privilegedAccessGroupEligibilityScheduleInstance
  - `[PrivilegedAccessGroupEligibilityScheduleRequestId <String>]`: The unique identifier of privilegedAccessGroupEligibilityScheduleRequest
  - `[RunId <String>]`: The unique identifier of run
  - `[StartDateTime <DateTime?>]`: Usage: startDateTime={startDateTime}
  - `[TaskDefinitionId <String>]`: The unique identifier of taskDefinition
  - `[TaskId <String>]`: The unique identifier of task
  - `[TaskProcessingResultId <String>]`: The unique identifier of taskProcessingResult
  - `[TaskReportId <String>]`: The unique identifier of taskReport
  - `[UnifiedRbacResourceActionId <String>]`: The unique identifier of unifiedRbacResourceAction
  - `[UnifiedRbacResourceNamespaceId <String>]`: The unique identifier of unifiedRbacResourceNamespace
  - `[UnifiedRoleAssignmentId <String>]`: The unique identifier of unifiedRoleAssignment
  - `[UnifiedRoleAssignmentScheduleId <String>]`: The unique identifier of unifiedRoleAssignmentSchedule
  - `[UnifiedRoleAssignmentScheduleInstanceId <String>]`: The unique identifier of unifiedRoleAssignmentScheduleInstance
  - `[UnifiedRoleAssignmentScheduleRequestId <String>]`: The unique identifier of unifiedRoleAssignmentScheduleRequest
  - `[UnifiedRoleDefinitionId <String>]`: The unique identifier of unifiedRoleDefinition
  - `[UnifiedRoleDefinitionId1 <String>]`: The unique identifier of unifiedRoleDefinition
  - `[UnifiedRoleEligibilityScheduleId <String>]`: The unique identifier of unifiedRoleEligibilitySchedule
  - `[UnifiedRoleEligibilityScheduleInstanceId <String>]`: The unique identifier of unifiedRoleEligibilityScheduleInstance
  - `[UnifiedRoleEligibilityScheduleRequestId <String>]`: The unique identifier of unifiedRoleEligibilityScheduleRequest
  - `[UserConsentRequestId <String>]`: The unique identifier of userConsentRequest
  - `[UserId <String>]`: The unique identifier of user
  - `[UserProcessingResultId <String>]`: The unique identifier of userProcessingResult
  - `[WorkflowId <String>]`: The unique identifier of workflow
  - `[WorkflowTemplateId <String>]`: The unique identifier of workflowTemplate
  - `[WorkflowVersionNumber <Int32?>]`: The unique identifier of workflowVersion

TERMSEXPIRATION `<IMicrosoftGraphTermsExpiration>`: termsExpiration
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Frequency <TimeSpan?>]`: Represents the frequency at which the terms will expire, after its first expiration as set in startDateTime.
The value is represented in ISO 8601 format for durations.
For example, PT1M represents a time period of one month.
  - `[StartDateTime <DateTime?>]`: The DateTime when the agreement is set to expire for all users.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/update-mgagreement](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/update-mgagreement)
























