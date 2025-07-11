---
external help file: Microsoft.Graph.Identity.Governance-help.xml
Module Name: Microsoft.Graph.Identity.Governance
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/new-mgidentitygovernancetermsofuseagreement
schema: 2.0.0
ms.subservice: entra-id-governance
---

# New-MgIdentityGovernanceTermsOfUseAgreement

## SYNOPSIS
Create a new agreement object.

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaIdentityGovernanceTermsOfUseAgreement](/powershell/module/Microsoft.Graph.Beta.Identity.Governance/New-MgBetaIdentityGovernanceTermsOfUseAgreement?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgIdentityGovernanceTermsOfUseAgreement [-ResponseHeadersVariable <String>]
 [-Acceptances <IMicrosoftGraphAgreementAcceptance[]>] [-AdditionalProperties <Hashtable>]
 [-DisplayName <String>] [-File <IMicrosoftGraphAgreementFile>]
 [-Files <IMicrosoftGraphAgreementFileLocalization[]>] [-Id <String>] [-IsPerDeviceAcceptanceRequired]
 [-IsViewingBeforeAcceptanceRequired] [-TermsExpiration <IMicrosoftGraphTermsExpiration>]
 [-UserReacceptRequiredFrequency <TimeSpan>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgIdentityGovernanceTermsOfUseAgreement -BodyParameter <IMicrosoftGraphAgreement>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new agreement object.

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	displayName = "Contoso ToU for guest users"
	isViewingBeforeAcceptanceRequired = $true
	files = @(
		@{
			fileName = "TOU.pdf"
			language = "en"
			isDefault = $true
			fileData = @{
				data = [System.Text.Encoding]::ASCII.GetBytes("SGVsbG8gd29ybGQ=//truncated-binary")
			}
		}
	)
}

New-MgIdentityGovernanceTermsOfUseAgreement -BodyParameter $params

```
This example shows how to use the New-MgIdentityGovernanceTermsOfUseAgreement Cmdlet.


## PARAMETERS

### -Acceptances
Read-only.
Information about acceptances of this agreement.
To construct, see NOTES section for ACCEPTANCES properties and create a hash table.

```yaml
Type: IMicrosoftGraphAgreementAcceptance[]
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
agreement
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAgreement
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

### -DisplayName
Display name of the agreement.
The display name is used for internal tracking of the agreement but isn't shown to end users who view the agreement.
Supports $filter (eq).

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

### -File
agreementFile
To construct, see NOTES section for FILE properties and create a hash table.

```yaml
Type: IMicrosoftGraphAgreementFile
Parameter Sets: CreateExpanded
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

### -IsPerDeviceAcceptanceRequired
Indicates whether end users are required to accept this agreement on every device that they access it from.
The end user is required to register their device in Microsoft Entra ID, if they haven't already done so.
Supports $filter (eq).

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

### -IsViewingBeforeAcceptanceRequired
Indicates whether the user has to expand the agreement before accepting.
Supports $filter (eq).

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
Parameter Sets: CreateExpanded
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

TERMSEXPIRATION `<IMicrosoftGraphTermsExpiration>`: termsExpiration
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Frequency <TimeSpan?>]`: Represents the frequency at which the terms will expire, after its first expiration as set in startDateTime.
The value is represented in ISO 8601 format for durations.
For example, PT1M represents a time period of one month.
  - `[StartDateTime <DateTime?>]`: The DateTime when the agreement is set to expire for all users.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/new-mgidentitygovernancetermsofuseagreement](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/new-mgidentitygovernancetermsofuseagreement)

[https://learn.microsoft.com/graph/api/termsofusecontainer-post-agreements?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/termsofusecontainer-post-agreements?view=graph-rest-1.0)























