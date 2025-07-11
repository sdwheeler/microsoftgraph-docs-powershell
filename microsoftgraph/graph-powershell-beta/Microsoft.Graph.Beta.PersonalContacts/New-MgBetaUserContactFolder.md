---
external help file: Microsoft.Graph.Beta.PersonalContacts-help.xml
Module Name: Microsoft.Graph.Beta.PersonalContacts
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.personalcontacts/new-mgbetausercontactfolder
schema: 2.0.0
---

# New-MgBetaUserContactFolder

## SYNOPSIS
Create new navigation property to contactFolders for users

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgUserContactFolder](/powershell/module/Microsoft.Graph.PersonalContacts/New-MgUserContactFolder?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaUserContactFolder -UserId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ChildFolders <IMicrosoftGraphContactFolder[]>]
 [-Contacts <IMicrosoftGraphContact[]>] [-DisplayName <String>] [-Id <String>]
 [-MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty[]>] [-ParentFolderId <String>]
 [-SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty[]>]
 [-WellKnownName <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Create
```
New-MgBetaUserContactFolder -UserId <String> -BodyParameter <IMicrosoftGraphContactFolder>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgBetaUserContactFolder -InputObject <IPersonalContactsIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ChildFolders <IMicrosoftGraphContactFolder[]>]
 [-Contacts <IMicrosoftGraphContact[]>] [-DisplayName <String>] [-Id <String>]
 [-MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty[]>] [-ParentFolderId <String>]
 [-SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty[]>]
 [-WellKnownName <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgBetaUserContactFolder -InputObject <IPersonalContactsIdentity>
 -BodyParameter <IMicrosoftGraphContactFolder> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to contactFolders for users

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Contacts.ReadWrite,  |
| Delegated (personal Microsoft account) | Contacts.ReadWrite,  |
| Application | Contacts.ReadWrite,  |

## EXAMPLES
### Example 1: Code snippet

```powershell
Import-Module Microsoft.Graph.Beta.PersonalContacts

$params = @{
	parentFolderId = "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA=="
	displayName = "Important contacts"
}

# A UPN can also be used as -UserId.
New-MgBetaUserContactFolder -UserId $userId -BodyParameter $params
```
This example shows how to use the New-MgBetaUserContactFolder Cmdlet.

To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).


## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
contactFolder
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphContactFolder
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ChildFolders
The collection of child folders in the folder.
Navigation property.
Read-only.
Nullable.
To construct, see NOTES section for CHILDFOLDERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphContactFolder[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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

### -Contacts
The contacts in the folder.
Navigation property.
Read-only.
Nullable.
To construct, see NOTES section for CONTACTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphContact[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
The folder's display name.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Type: IPersonalContactsIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -MultiValueExtendedProperties
The collection of multi-value extended properties defined for the contactFolder.
Read-only.
Nullable.
To construct, see NOTES section for MULTIVALUEEXTENDEDPROPERTIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphMultiValueLegacyExtendedProperty[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ParentFolderId
The ID of the folder's parent folder.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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

### -SingleValueExtendedProperties
The collection of single-value extended properties defined for the contactFolder.
Read-only.
Nullable.
To construct, see NOTES section for SINGLEVALUEEXTENDEDPROPERTIES properties and create a hash table.

```yaml
Type: IMicrosoftGraphSingleValueLegacyExtendedProperty[]
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserId
The unique identifier of user

```yaml
Type: String
Parameter Sets: CreateExpanded, Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WellKnownName
The name of the folder if the folder is a recognized folder.
Currently contacts is the only recognized contacts folder.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphContactFolder
### Microsoft.Graph.Beta.PowerShell.Models.IPersonalContactsIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphContactFolder
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphContactFolder>`: contactFolder
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ChildFolders <IMicrosoftGraphContactFolder- `[]`>]`: The collection of child folders in the folder.
Navigation property.
Read-only.
Nullable.
  - `[Contacts <IMicrosoftGraphContact- `[]`>]`: The contacts in the folder.
Navigation property.
Read-only.
Nullable.
    - `[Categories <String- `[]`>]`: The categories associated with the item.
    - `[ChangeKey <String>]`: Identifies the version of the item.
Every time the item is changed, changeKey changes as well.
This allows Exchange to apply changes to the correct version of the object.
Read-only.
    - `[CreatedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[LastModifiedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AssistantName <String>]`: The name of the contact's assistant.
    - `[Birthday <DateTime?>]`: The contact's birthday.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[Children <String- `[]`>]`: The names of the contact's children.
    - `[CompanyName <String>]`: The name of the contact's company.
    - `[Department <String>]`: The contact's department.
    - `[DisplayName <String>]`: The contact's display name.
You can specify the display name in a create or update operation.
Later updates to other properties might cause an automatically generated value to overwrite the displayName value you specified.
To preserve a pre-existing value, always include it as displayName in an update operation.
    - `[EmailAddresses <IMicrosoftGraphTypedEmailAddress- `[]`>]`: The contact's email addresses.
      - `[Address <String>]`: The email address of an entity instance.
      - `[Name <String>]`: The display name of an entity instance.
      - `[OtherLabel <String>]`: To specify a custom type of email address, set type to other, and assign otherLabel to a custom string.
For example, you may use a specific email address for your volunteer activities.
Set type to other, and set otherLabel to a custom string such as Volunteer work.
      - `[Type <String>]`: emailType
    - `[Extensions <IMicrosoftGraphExtension- `[]`>]`: The collection of open extensions defined for the contact.
Nullable.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[FileAs <String>]`: The name the contact is filed under.
    - `[Flag <IMicrosoftGraphFollowupFlag>]`: followupFlag
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[CompletedDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}).
For example, '2019-04-16T09:00:00'.
        - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'.
See below for possible values.
      - `[DueDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
      - `[FlagStatus <String>]`: followupFlagStatus
      - `[StartDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
    - `[Gender <String>]`: The contact's gender.
    - `[Generation <String>]`: The contact's suffix.
    - `[GivenName <String>]`: The contact's given name.
    - `[ImAddresses <String- `[]`>]`: The contact's instant messaging (IM) addresses.
    - `[Initials <String>]`: The contact's initials.
    - `[IsFavorite <Boolean?>]`: 
    - `[JobTitle <String>]`: The contact's job title.
    - `[Manager <String>]`: The name of the contact's manager.
    - `[MiddleName <String>]`: The contact's middle name.
    - `[MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty- `[]`>]`: The collection of multi-value extended properties defined for the contact.
Read-only.
Nullable.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Value <String- `[]`>]`: A collection of property values.
    - `[NickName <String>]`: The contact's nickname.
    - `[OfficeLocation <String>]`: The location of the contact's office.
    - `[ParentFolderId <String>]`: The ID of the contact's parent folder.
    - `[PersonalNotes <String>]`: The user's notes about the contact.
    - `[Phones <IMicrosoftGraphPhone- `[]`>]`: Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.
      - `[Number <String>]`: The phone number.
      - `[Type <String>]`: phoneType
    - `[Photo <IMicrosoftGraphProfilePhoto>]`: profilePhoto
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Height <Int32?>]`: The height of the photo.
Read-only.
      - `[Width <Int32?>]`: The width of the photo.
Read-only.
    - `[PostalAddresses <IMicrosoftGraphPhysicalAddress- `[]`>]`: Addresses associated with the contact, for example, home address and business address.
      - `[City <String>]`: The city.
      - `[CountryOrRegion <String>]`: The country or region.
It's a free-format string value, for example, 'United States'.
      - `[PostOfficeBox <String>]`: The post office box number.
      - `[PostalCode <String>]`: The postal code.
      - `[State <String>]`: The state.
      - `[Street <String>]`: The street.
      - `[Type <String>]`: physicalAddressType
    - `[Profession <String>]`: The contact's profession.
    - `[SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty- `[]`>]`: The collection of single-value extended properties defined for the contact.
Read-only.
Nullable.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Value <String>]`: A property value.
    - `[SpouseName <String>]`: The name of the contact's spouse/partner.
    - `[Surname <String>]`: The contact's surname.
    - `[Title <String>]`: The contact's title.
    - `[Websites <IMicrosoftGraphWebsite- `[]`>]`: Web sites associated with the contact.
      - `[Address <String>]`: The URL of the website.
      - `[DisplayName <String>]`: The display name of the web site.
      - `[Type <String>]`: websiteType
    - `[WeddingAnniversary <DateTime?>]`: The contact's wedding anniversary.
    - `[YomiCompanyName <String>]`: The phonetic Japanese company name of the contact.
    - `[YomiGivenName <String>]`: The phonetic Japanese given name (first name) of the contact.
    - `[YomiSurname <String>]`: The phonetic Japanese surname (last name)  of the contact.
  - `[DisplayName <String>]`: The folder's display name.
  - `[MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty- `[]`>]`: The collection of multi-value extended properties defined for the contactFolder.
Read-only.
Nullable.
  - `[ParentFolderId <String>]`: The ID of the folder's parent folder.
  - `[SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty- `[]`>]`: The collection of single-value extended properties defined for the contactFolder.
Read-only.
Nullable.
  - `[WellKnownName <String>]`: The name of the folder if the folder is a recognized folder.
Currently contacts is the only recognized contacts folder.

CHILDFOLDERS `<IMicrosoftGraphContactFolder- `[]`>`: The collection of child folders in the folder.
Navigation property.
Read-only.
Nullable.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ChildFolders <IMicrosoftGraphContactFolder- `[]`>]`: The collection of child folders in the folder.
Navigation property.
Read-only.
Nullable.
  - `[Contacts <IMicrosoftGraphContact- `[]`>]`: The contacts in the folder.
Navigation property.
Read-only.
Nullable.
    - `[Categories <String- `[]`>]`: The categories associated with the item.
    - `[ChangeKey <String>]`: Identifies the version of the item.
Every time the item is changed, changeKey changes as well.
This allows Exchange to apply changes to the correct version of the object.
Read-only.
    - `[CreatedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[LastModifiedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AssistantName <String>]`: The name of the contact's assistant.
    - `[Birthday <DateTime?>]`: The contact's birthday.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[Children <String- `[]`>]`: The names of the contact's children.
    - `[CompanyName <String>]`: The name of the contact's company.
    - `[Department <String>]`: The contact's department.
    - `[DisplayName <String>]`: The contact's display name.
You can specify the display name in a create or update operation.
Later updates to other properties might cause an automatically generated value to overwrite the displayName value you specified.
To preserve a pre-existing value, always include it as displayName in an update operation.
    - `[EmailAddresses <IMicrosoftGraphTypedEmailAddress- `[]`>]`: The contact's email addresses.
      - `[Address <String>]`: The email address of an entity instance.
      - `[Name <String>]`: The display name of an entity instance.
      - `[OtherLabel <String>]`: To specify a custom type of email address, set type to other, and assign otherLabel to a custom string.
For example, you may use a specific email address for your volunteer activities.
Set type to other, and set otherLabel to a custom string such as Volunteer work.
      - `[Type <String>]`: emailType
    - `[Extensions <IMicrosoftGraphExtension- `[]`>]`: The collection of open extensions defined for the contact.
Nullable.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[FileAs <String>]`: The name the contact is filed under.
    - `[Flag <IMicrosoftGraphFollowupFlag>]`: followupFlag
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[CompletedDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}).
For example, '2019-04-16T09:00:00'.
        - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'.
See below for possible values.
      - `[DueDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
      - `[FlagStatus <String>]`: followupFlagStatus
      - `[StartDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
    - `[Gender <String>]`: The contact's gender.
    - `[Generation <String>]`: The contact's suffix.
    - `[GivenName <String>]`: The contact's given name.
    - `[ImAddresses <String- `[]`>]`: The contact's instant messaging (IM) addresses.
    - `[Initials <String>]`: The contact's initials.
    - `[IsFavorite <Boolean?>]`: 
    - `[JobTitle <String>]`: The contact's job title.
    - `[Manager <String>]`: The name of the contact's manager.
    - `[MiddleName <String>]`: The contact's middle name.
    - `[MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty- `[]`>]`: The collection of multi-value extended properties defined for the contact.
Read-only.
Nullable.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Value <String- `[]`>]`: A collection of property values.
    - `[NickName <String>]`: The contact's nickname.
    - `[OfficeLocation <String>]`: The location of the contact's office.
    - `[ParentFolderId <String>]`: The ID of the contact's parent folder.
    - `[PersonalNotes <String>]`: The user's notes about the contact.
    - `[Phones <IMicrosoftGraphPhone- `[]`>]`: Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.
      - `[Number <String>]`: The phone number.
      - `[Type <String>]`: phoneType
    - `[Photo <IMicrosoftGraphProfilePhoto>]`: profilePhoto
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Height <Int32?>]`: The height of the photo.
Read-only.
      - `[Width <Int32?>]`: The width of the photo.
Read-only.
    - `[PostalAddresses <IMicrosoftGraphPhysicalAddress- `[]`>]`: Addresses associated with the contact, for example, home address and business address.
      - `[City <String>]`: The city.
      - `[CountryOrRegion <String>]`: The country or region.
It's a free-format string value, for example, 'United States'.
      - `[PostOfficeBox <String>]`: The post office box number.
      - `[PostalCode <String>]`: The postal code.
      - `[State <String>]`: The state.
      - `[Street <String>]`: The street.
      - `[Type <String>]`: physicalAddressType
    - `[Profession <String>]`: The contact's profession.
    - `[SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty- `[]`>]`: The collection of single-value extended properties defined for the contact.
Read-only.
Nullable.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Value <String>]`: A property value.
    - `[SpouseName <String>]`: The name of the contact's spouse/partner.
    - `[Surname <String>]`: The contact's surname.
    - `[Title <String>]`: The contact's title.
    - `[Websites <IMicrosoftGraphWebsite- `[]`>]`: Web sites associated with the contact.
      - `[Address <String>]`: The URL of the website.
      - `[DisplayName <String>]`: The display name of the web site.
      - `[Type <String>]`: websiteType
    - `[WeddingAnniversary <DateTime?>]`: The contact's wedding anniversary.
    - `[YomiCompanyName <String>]`: The phonetic Japanese company name of the contact.
    - `[YomiGivenName <String>]`: The phonetic Japanese given name (first name) of the contact.
    - `[YomiSurname <String>]`: The phonetic Japanese surname (last name)  of the contact.
  - `[DisplayName <String>]`: The folder's display name.
  - `[MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty- `[]`>]`: The collection of multi-value extended properties defined for the contactFolder.
Read-only.
Nullable.
  - `[ParentFolderId <String>]`: The ID of the folder's parent folder.
  - `[SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty- `[]`>]`: The collection of single-value extended properties defined for the contactFolder.
Read-only.
Nullable.
  - `[WellKnownName <String>]`: The name of the folder if the folder is a recognized folder.
Currently contacts is the only recognized contacts folder.

CONTACTS `<IMicrosoftGraphContact- `[]`>`: The contacts in the folder.
Navigation property.
Read-only.
Nullable.
  - `[Categories <String- `[]`>]`: The categories associated with the item.
  - `[ChangeKey <String>]`: Identifies the version of the item.
Every time the item is changed, changeKey changes as well.
This allows Exchange to apply changes to the correct version of the object.
Read-only.
  - `[CreatedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[LastModifiedDateTime <DateTime?>]`: The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AssistantName <String>]`: The name of the contact's assistant.
  - `[Birthday <DateTime?>]`: The contact's birthday.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[Children <String- `[]`>]`: The names of the contact's children.
  - `[CompanyName <String>]`: The name of the contact's company.
  - `[Department <String>]`: The contact's department.
  - `[DisplayName <String>]`: The contact's display name.
You can specify the display name in a create or update operation.
Later updates to other properties might cause an automatically generated value to overwrite the displayName value you specified.
To preserve a pre-existing value, always include it as displayName in an update operation.
  - `[EmailAddresses <IMicrosoftGraphTypedEmailAddress- `[]`>]`: The contact's email addresses.
    - `[Address <String>]`: The email address of an entity instance.
    - `[Name <String>]`: The display name of an entity instance.
    - `[OtherLabel <String>]`: To specify a custom type of email address, set type to other, and assign otherLabel to a custom string.
For example, you may use a specific email address for your volunteer activities.
Set type to other, and set otherLabel to a custom string such as Volunteer work.
    - `[Type <String>]`: emailType
  - `[Extensions <IMicrosoftGraphExtension- `[]`>]`: The collection of open extensions defined for the contact.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[FileAs <String>]`: The name the contact is filed under.
  - `[Flag <IMicrosoftGraphFollowupFlag>]`: followupFlag
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[CompletedDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DateTime <String>]`: A single point of time in a combined date and time representation ({date}T{time}).
For example, '2019-04-16T09:00:00'.
      - `[TimeZone <String>]`: Represents a time zone, for example, 'Pacific Standard Time'.
See below for possible values.
    - `[DueDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
    - `[FlagStatus <String>]`: followupFlagStatus
    - `[StartDateTime <IMicrosoftGraphDateTimeZone>]`: dateTimeTimeZone
  - `[Gender <String>]`: The contact's gender.
  - `[Generation <String>]`: The contact's suffix.
  - `[GivenName <String>]`: The contact's given name.
  - `[ImAddresses <String- `[]`>]`: The contact's instant messaging (IM) addresses.
  - `[Initials <String>]`: The contact's initials.
  - `[IsFavorite <Boolean?>]`: 
  - `[JobTitle <String>]`: The contact's job title.
  - `[Manager <String>]`: The name of the contact's manager.
  - `[MiddleName <String>]`: The contact's middle name.
  - `[MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty- `[]`>]`: The collection of multi-value extended properties defined for the contact.
Read-only.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Value <String- `[]`>]`: A collection of property values.
  - `[NickName <String>]`: The contact's nickname.
  - `[OfficeLocation <String>]`: The location of the contact's office.
  - `[ParentFolderId <String>]`: The ID of the contact's parent folder.
  - `[PersonalNotes <String>]`: The user's notes about the contact.
  - `[Phones <IMicrosoftGraphPhone- `[]`>]`: Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.
    - `[Number <String>]`: The phone number.
    - `[Type <String>]`: phoneType
  - `[Photo <IMicrosoftGraphProfilePhoto>]`: profilePhoto
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Height <Int32?>]`: The height of the photo.
Read-only.
    - `[Width <Int32?>]`: The width of the photo.
Read-only.
  - `[PostalAddresses <IMicrosoftGraphPhysicalAddress- `[]`>]`: Addresses associated with the contact, for example, home address and business address.
    - `[City <String>]`: The city.
    - `[CountryOrRegion <String>]`: The country or region.
It's a free-format string value, for example, 'United States'.
    - `[PostOfficeBox <String>]`: The post office box number.
    - `[PostalCode <String>]`: The postal code.
    - `[State <String>]`: The state.
    - `[Street <String>]`: The street.
    - `[Type <String>]`: physicalAddressType
  - `[Profession <String>]`: The contact's profession.
  - `[SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty- `[]`>]`: The collection of single-value extended properties defined for the contact.
Read-only.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Value <String>]`: A property value.
  - `[SpouseName <String>]`: The name of the contact's spouse/partner.
  - `[Surname <String>]`: The contact's surname.
  - `[Title <String>]`: The contact's title.
  - `[Websites <IMicrosoftGraphWebsite- `[]`>]`: Web sites associated with the contact.
    - `[Address <String>]`: The URL of the website.
    - `[DisplayName <String>]`: The display name of the web site.
    - `[Type <String>]`: websiteType
  - `[WeddingAnniversary <DateTime?>]`: The contact's wedding anniversary.
  - `[YomiCompanyName <String>]`: The phonetic Japanese company name of the contact.
  - `[YomiGivenName <String>]`: The phonetic Japanese given name (first name) of the contact.
  - `[YomiSurname <String>]`: The phonetic Japanese surname (last name)  of the contact.

INPUTOBJECT `<IPersonalContactsIdentity>`: Identity Parameter
  - `[ContactFolderId <String>]`: The unique identifier of contactFolder
  - `[ContactFolderId1 <String>]`: The unique identifier of contactFolder
  - `[ContactId <String>]`: The unique identifier of contact
  - `[ExtensionId <String>]`: The unique identifier of extension
  - `[UserId <String>]`: The unique identifier of user

MULTIVALUEEXTENDEDPROPERTIES `<IMicrosoftGraphMultiValueLegacyExtendedProperty- `[]`>`: The collection of multi-value extended properties defined for the contactFolder.
Read-only.
Nullable.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Value <String- `[]`>]`: A collection of property values.

SINGLEVALUEEXTENDEDPROPERTIES `<IMicrosoftGraphSingleValueLegacyExtendedProperty- `[]`>`: The collection of single-value extended properties defined for the contactFolder.
Read-only.
Nullable.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Value <String>]`: A property value.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.personalcontacts/new-mgbetausercontactfolder](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.personalcontacts/new-mgbetausercontactfolder)























