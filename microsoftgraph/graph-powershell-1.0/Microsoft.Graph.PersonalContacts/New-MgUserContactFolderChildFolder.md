---
external help file: Microsoft.Graph.PersonalContacts-help.xml
Module Name: Microsoft.Graph.PersonalContacts
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.personalcontacts/new-mgusercontactfolderchildfolder
schema: 2.0.0
---

# New-MgUserContactFolderChildFolder

## SYNOPSIS
Create new navigation property to childFolders for users

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaUserContactFolderChildFolder](/powershell/module/Microsoft.Graph.Beta.PersonalContacts/New-MgBetaUserContactFolderChildFolder?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgUserContactFolderChildFolder -ContactFolderId <String> -UserId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-ChildFolders <IMicrosoftGraphContactFolder[]>] [-Contacts <IMicrosoftGraphContact[]>]
 [-DisplayName <String>] [-Id <String>]
 [-MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty[]>] [-ParentFolderId <String>]
 [-SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgUserContactFolderChildFolder -ContactFolderId <String> -UserId <String>
 -BodyParameter <IMicrosoftGraphContactFolder> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgUserContactFolderChildFolder -InputObject <IPersonalContactsIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ChildFolders <IMicrosoftGraphContactFolder[]>]
 [-Contacts <IMicrosoftGraphContact[]>] [-DisplayName <String>] [-Id <String>]
 [-MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty[]>] [-ParentFolderId <String>]
 [-SingleValueExtendedProperties <IMicrosoftGraphSingleValueLegacyExtendedProperty[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgUserContactFolderChildFolder -InputObject <IPersonalContactsIdentity>
 -BodyParameter <IMicrosoftGraphContactFolder> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to childFolders for users

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Contacts.ReadWrite,  |
| Delegated (personal Microsoft account) | Contacts.ReadWrite,  |
| Application | Contacts.ReadWrite,  |

## EXAMPLES
### Example 1: Code snippet

```powershell
Import-Module Microsoft.Graph.PersonalContacts

$params = @{
	displayName = "Family"
}

# A UPN can also be used as -UserId.
New-MgUserContactFolderChildFolder -UserId $userId -ContactFolderId $contactFolderId -BodyParameter $params
```
This example shows how to use the New-MgUserContactFolderChildFolder Cmdlet.

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

### -ContactFolderId
The unique identifier of contactFolder

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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphContactFolder
### Microsoft.Graph.PowerShell.Models.IPersonalContactsIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphContactFolder
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
    - `[Categories <String- `[]`>]`: The categories associated with the item
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
    - `[BusinessAddress <IMicrosoftGraphPhysicalAddress>]`: physicalAddress
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[City <String>]`: The city.
      - `[CountryOrRegion <String>]`: The country or region.
It's a free-format string value, for example, 'United States'.
      - `[PostalCode <String>]`: The postal code.
      - `[State <String>]`: The state.
      - `[Street <String>]`: The street.
    - `[BusinessHomePage <String>]`: The business home page of the contact.
    - `[BusinessPhones <String- `[]`>]`: The contact's business phone numbers.
    - `[Children <String- `[]`>]`: The names of the contact's children.
    - `[CompanyName <String>]`: The name of the contact's company.
    - `[Department <String>]`: The contact's department.
    - `[DisplayName <String>]`: The contact's display name.
You can specify the display name in a create or update operation.
Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.
To preserve a pre-existing value, always include it as displayName in an update operation.
    - `[EmailAddresses <IMicrosoftGraphEmailAddress- `[]`>]`: The contact's email addresses.
      - `[Address <String>]`: The email address of the person or entity.
      - `[Name <String>]`: The display name of the person or entity.
    - `[Extensions <IMicrosoftGraphExtension- `[]`>]`: The collection of open extensions defined for the contact.
Read-only.
Nullable.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[FileAs <String>]`: The name the contact is filed under.
    - `[Generation <String>]`: The contact's suffix.
    - `[GivenName <String>]`: The contact's given name.
    - `[HomeAddress <IMicrosoftGraphPhysicalAddress>]`: physicalAddress
    - `[HomePhones <String- `[]`>]`: The contact's home phone numbers.
    - `[ImAddresses <String- `[]`>]`: The contact's instant messaging (IM) addresses.
    - `[Initials <String>]`: The contact's initials.
    - `[JobTitle <String>]`: The contact's job title.
    - `[Manager <String>]`: The name of the contact's manager.
    - `[MiddleName <String>]`: The contact's middle name.
    - `[MobilePhone <String>]`: The contact's mobile phone number.
    - `[MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty- `[]`>]`: The collection of multi-value extended properties defined for the contact.
Read-only.
Nullable.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Value <String- `[]`>]`: A collection of property values.
    - `[NickName <String>]`: The contact's nickname.
    - `[OfficeLocation <String>]`: The location of the contact's office.
    - `[OtherAddress <IMicrosoftGraphPhysicalAddress>]`: physicalAddress
    - `[ParentFolderId <String>]`: The ID of the contact's parent folder.
    - `[PersonalNotes <String>]`: The user's notes about the contact.
    - `[Photo <IMicrosoftGraphProfilePhoto>]`: profilePhoto
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Height <Int32?>]`: The height of the photo.
Read-only.
      - `[Width <Int32?>]`: The width of the photo.
Read-only.
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
    - `[Categories <String- `[]`>]`: The categories associated with the item
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
    - `[BusinessAddress <IMicrosoftGraphPhysicalAddress>]`: physicalAddress
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[City <String>]`: The city.
      - `[CountryOrRegion <String>]`: The country or region.
It's a free-format string value, for example, 'United States'.
      - `[PostalCode <String>]`: The postal code.
      - `[State <String>]`: The state.
      - `[Street <String>]`: The street.
    - `[BusinessHomePage <String>]`: The business home page of the contact.
    - `[BusinessPhones <String- `[]`>]`: The contact's business phone numbers.
    - `[Children <String- `[]`>]`: The names of the contact's children.
    - `[CompanyName <String>]`: The name of the contact's company.
    - `[Department <String>]`: The contact's department.
    - `[DisplayName <String>]`: The contact's display name.
You can specify the display name in a create or update operation.
Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.
To preserve a pre-existing value, always include it as displayName in an update operation.
    - `[EmailAddresses <IMicrosoftGraphEmailAddress- `[]`>]`: The contact's email addresses.
      - `[Address <String>]`: The email address of the person or entity.
      - `[Name <String>]`: The display name of the person or entity.
    - `[Extensions <IMicrosoftGraphExtension- `[]`>]`: The collection of open extensions defined for the contact.
Read-only.
Nullable.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[FileAs <String>]`: The name the contact is filed under.
    - `[Generation <String>]`: The contact's suffix.
    - `[GivenName <String>]`: The contact's given name.
    - `[HomeAddress <IMicrosoftGraphPhysicalAddress>]`: physicalAddress
    - `[HomePhones <String- `[]`>]`: The contact's home phone numbers.
    - `[ImAddresses <String- `[]`>]`: The contact's instant messaging (IM) addresses.
    - `[Initials <String>]`: The contact's initials.
    - `[JobTitle <String>]`: The contact's job title.
    - `[Manager <String>]`: The name of the contact's manager.
    - `[MiddleName <String>]`: The contact's middle name.
    - `[MobilePhone <String>]`: The contact's mobile phone number.
    - `[MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty- `[]`>]`: The collection of multi-value extended properties defined for the contact.
Read-only.
Nullable.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Value <String- `[]`>]`: A collection of property values.
    - `[NickName <String>]`: The contact's nickname.
    - `[OfficeLocation <String>]`: The location of the contact's office.
    - `[OtherAddress <IMicrosoftGraphPhysicalAddress>]`: physicalAddress
    - `[ParentFolderId <String>]`: The ID of the contact's parent folder.
    - `[PersonalNotes <String>]`: The user's notes about the contact.
    - `[Photo <IMicrosoftGraphProfilePhoto>]`: profilePhoto
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Height <Int32?>]`: The height of the photo.
Read-only.
      - `[Width <Int32?>]`: The width of the photo.
Read-only.
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

CONTACTS `<IMicrosoftGraphContact- `[]`>`: The contacts in the folder.
Navigation property.
Read-only.
Nullable.
  - `[Categories <String- `[]`>]`: The categories associated with the item
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
  - `[BusinessAddress <IMicrosoftGraphPhysicalAddress>]`: physicalAddress
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[City <String>]`: The city.
    - `[CountryOrRegion <String>]`: The country or region.
It's a free-format string value, for example, 'United States'.
    - `[PostalCode <String>]`: The postal code.
    - `[State <String>]`: The state.
    - `[Street <String>]`: The street.
  - `[BusinessHomePage <String>]`: The business home page of the contact.
  - `[BusinessPhones <String- `[]`>]`: The contact's business phone numbers.
  - `[Children <String- `[]`>]`: The names of the contact's children.
  - `[CompanyName <String>]`: The name of the contact's company.
  - `[Department <String>]`: The contact's department.
  - `[DisplayName <String>]`: The contact's display name.
You can specify the display name in a create or update operation.
Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.
To preserve a pre-existing value, always include it as displayName in an update operation.
  - `[EmailAddresses <IMicrosoftGraphEmailAddress- `[]`>]`: The contact's email addresses.
    - `[Address <String>]`: The email address of the person or entity.
    - `[Name <String>]`: The display name of the person or entity.
  - `[Extensions <IMicrosoftGraphExtension- `[]`>]`: The collection of open extensions defined for the contact.
Read-only.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[FileAs <String>]`: The name the contact is filed under.
  - `[Generation <String>]`: The contact's suffix.
  - `[GivenName <String>]`: The contact's given name.
  - `[HomeAddress <IMicrosoftGraphPhysicalAddress>]`: physicalAddress
  - `[HomePhones <String- `[]`>]`: The contact's home phone numbers.
  - `[ImAddresses <String- `[]`>]`: The contact's instant messaging (IM) addresses.
  - `[Initials <String>]`: The contact's initials.
  - `[JobTitle <String>]`: The contact's job title.
  - `[Manager <String>]`: The name of the contact's manager.
  - `[MiddleName <String>]`: The contact's middle name.
  - `[MobilePhone <String>]`: The contact's mobile phone number.
  - `[MultiValueExtendedProperties <IMicrosoftGraphMultiValueLegacyExtendedProperty- `[]`>]`: The collection of multi-value extended properties defined for the contact.
Read-only.
Nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Value <String- `[]`>]`: A collection of property values.
  - `[NickName <String>]`: The contact's nickname.
  - `[OfficeLocation <String>]`: The location of the contact's office.
  - `[OtherAddress <IMicrosoftGraphPhysicalAddress>]`: physicalAddress
  - `[ParentFolderId <String>]`: The ID of the contact's parent folder.
  - `[PersonalNotes <String>]`: The user's notes about the contact.
  - `[Photo <IMicrosoftGraphProfilePhoto>]`: profilePhoto
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Height <Int32?>]`: The height of the photo.
Read-only.
    - `[Width <Int32?>]`: The width of the photo.
Read-only.
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

[https://learn.microsoft.com/powershell/module/microsoft.graph.personalcontacts/new-mgusercontactfolderchildfolder](https://learn.microsoft.com/powershell/module/microsoft.graph.personalcontacts/new-mgusercontactfolderchildfolder)























