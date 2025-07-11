---
external help file: Microsoft.Graph.Identity.DirectoryManagement-help.xml
Module Name: Microsoft.Graph.Identity.DirectoryManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.directorymanagement/new-mgorganizationbrandinglocalization
schema: 2.0.0
ms.subservice: entra-sign-in
---

# New-MgOrganizationBrandingLocalization

## SYNOPSIS
Create a new organizationalBrandingLocalization object.
This creates a localized branding and at the same time, the default branding if it doesn't exist.
The default branding is created only once.
It's loaded when a localized branding isn't configured for the user's browser language.
To retrieve the default branding, see Get branding.

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaOrganizationBrandingLocalization](/powershell/module/Microsoft.Graph.Beta.Identity.DirectoryManagement/New-MgBetaOrganizationBrandingLocalization?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgOrganizationBrandingLocalization -OrganizationId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-BackgroundColor <String>] [-BackgroundImageInputFile <String>]
 [-BackgroundImageRelativeUrl <String>] [-BannerLogoInputFile <String>] [-BannerLogoRelativeUrl <String>]
 [-CdnList <String[]>] [-ContentCustomization <IMicrosoftGraphContentCustomization>]
 [-CustomAccountResetCredentialsUrl <String>] [-CustomCannotAccessYourAccountText <String>]
 [-CustomCannotAccessYourAccountUrl <String>] [-CustomCssInputFile <String>] [-CustomCssRelativeUrl <String>]
 [-CustomForgotMyPasswordText <String>] [-CustomPrivacyAndCookiesText <String>]
 [-CustomPrivacyAndCookiesUrl <String>] [-CustomResetItNowText <String>] [-CustomTermsOfUseText <String>]
 [-CustomTermsOfUseUrl <String>] [-FaviconInputFile <String>] [-FaviconRelativeUrl <String>]
 [-HeaderBackgroundColor <String>] [-HeaderLogoInputFile <String>] [-HeaderLogoRelativeUrl <String>]
 [-Id <String>] [-LoginPageLayoutConfiguration <IMicrosoftGraphLoginPageLayoutConfiguration>]
 [-LoginPageTextVisibilitySettings <IMicrosoftGraphLoginPageTextVisibilitySettings>] [-SignInPageText <String>]
 [-SquareLogoDarkInputFile <String>] [-SquareLogoDarkRelativeUrl <String>] [-SquareLogoInputFile <String>]
 [-SquareLogoRelativeUrl <String>] [-UsernameHintText <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgOrganizationBrandingLocalization -OrganizationId <String> -BodyParameter <Hashtable>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgOrganizationBrandingLocalization -InputObject <IIdentityDirectoryManagementIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-BackgroundColor <String>]
 [-BackgroundImageInputFile <String>] [-BackgroundImageRelativeUrl <String>] [-BannerLogoInputFile <String>]
 [-BannerLogoRelativeUrl <String>] [-CdnList <String[]>]
 [-ContentCustomization <IMicrosoftGraphContentCustomization>] [-CustomAccountResetCredentialsUrl <String>]
 [-CustomCannotAccessYourAccountText <String>] [-CustomCannotAccessYourAccountUrl <String>]
 [-CustomCssInputFile <String>] [-CustomCssRelativeUrl <String>] [-CustomForgotMyPasswordText <String>]
 [-CustomPrivacyAndCookiesText <String>] [-CustomPrivacyAndCookiesUrl <String>]
 [-CustomResetItNowText <String>] [-CustomTermsOfUseText <String>] [-CustomTermsOfUseUrl <String>]
 [-FaviconInputFile <String>] [-FaviconRelativeUrl <String>] [-HeaderBackgroundColor <String>]
 [-HeaderLogoInputFile <String>] [-HeaderLogoRelativeUrl <String>] [-Id <String>]
 [-LoginPageLayoutConfiguration <IMicrosoftGraphLoginPageLayoutConfiguration>]
 [-LoginPageTextVisibilitySettings <IMicrosoftGraphLoginPageTextVisibilitySettings>] [-SignInPageText <String>]
 [-SquareLogoDarkInputFile <String>] [-SquareLogoDarkRelativeUrl <String>] [-SquareLogoInputFile <String>]
 [-SquareLogoRelativeUrl <String>] [-UsernameHintText <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgOrganizationBrandingLocalization -InputObject <IIdentityDirectoryManagementIdentity>
 -BodyParameter <Hashtable> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new organizationalBrandingLocalization object.
This creates a localized branding and at the same time, the default branding if it doesn't exist.
The default branding is created only once.
It's loaded when a localized branding isn't configured for the user's browser language.
To retrieve the default branding, see Get branding.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | OrganizationalBranding.ReadWrite.All, Organization.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | OrganizationalBranding.ReadWrite.All, Organization.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
	backgroundColor = "#00000F"
	id = "fr-FR"
	signInPageText = " "
}

New-MgOrganizationBrandingLocalization -OrganizationId $organizationId -BodyParameter $params

```
This example shows how to use the New-MgOrganizationBrandingLocalization Cmdlet.


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

### -BackgroundColor
Color that appears in place of the background image in low-bandwidth connections.
We recommend that you use the primary color of your banner logo or your organization color.
Specify this in hexadecimal format, for example, white is #FFFFFF.

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

### -BackgroundImageInputFile
Input File for BackgroundImage (Image that appears as the background of the sign-in page.
The allowed types are PNG or JPEG not smaller than 300 KB and not larger than 1920 × 1080 pixels.
A smaller image reduces bandwidth requirements and make the page load faster.)

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

### -BackgroundImageRelativeUrl
A relative URL for the backgroundImage property that is combined with a CDN base URL from the cdnList to provide the version served by a CDN.
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

### -BannerLogoInputFile
Input File for BannerLogo (A banner version of your company logo that appears on the sign-in page.
The allowed types are PNG or JPEG not larger than 36 × 245 pixels.
We recommend using a transparent image with no padding around the logo.)

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

### -BannerLogoRelativeUrl
A relative URL for the bannerLogo property that is combined with a CDN base URL from the cdnList to provide the read-only version served by a CDN.
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

### -BodyParameter
organizationalBrandingLocalization

```yaml
Type: Hashtable
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CdnList
A list of base URLs for all available CDN providers that are serving the assets of the current resource.
Several CDN providers are used at the same time for high availability of read requests.
Read-only.

```yaml
Type: String[]
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

### -ContentCustomization
contentCustomization
To construct, see NOTES section for CONTENTCUSTOMIZATION properties and create a hash table.

```yaml
Type: IMicrosoftGraphContentCustomization
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CustomAccountResetCredentialsUrl
A custom URL for resetting account credentials.
This URL must be in ASCII format or non-ASCII characters must be URL encoded, and not exceed 128 characters.

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

### -CustomCannotAccessYourAccountText
A string to replace the default 'Can't access your account' self-service password reset (SSPR) hyperlink text on the sign-in page.
This text must be in Unicode format and not exceed 256 characters.

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

### -CustomCannotAccessYourAccountUrl
A custom URL to replace the default URL of the self-service password reset (SSPR) 'Can't access your account' hyperlink on the sign-in page.
This URL must be in ASCII format or non-ASCII characters must be URL encoded, and not exceed 128 characters.
DO NOT USE.
Use customAccountResetCredentialsUrl instead.

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

### -CustomCssInputFile
Input File for CustomCss (CSS styling that appears on the sign-in page.
The allowed format is .css format only and not larger than 25 KB.)

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

### -CustomCssRelativeUrl
A relative URL for the customCSS property that is combined with a CDN base URL from the cdnList to provide the version served by a CDN.
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

### -CustomForgotMyPasswordText
A string to replace the default 'Forgot my password' hyperlink text on the sign-in form.
This text must be in Unicode format and not exceed 256 characters.

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

### -CustomPrivacyAndCookiesText
A string to replace the default 'Privacy and Cookies' hyperlink text in the footer.
This text must be in Unicode format and not exceed 256 characters.

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

### -CustomPrivacyAndCookiesUrl
A custom URL to replace the default URL of the 'Privacy and Cookies' hyperlink in the footer.
This URL must be in ASCII format or non-ASCII characters must be URL encoded, and not exceed 128 characters.

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

### -CustomResetItNowText
A string to replace the default 'reset it now' hyperlink text on the sign-in form.
This text must be in Unicode format and not exceed 256 characters.
DO NOT USE: Customization of the 'reset it now' hyperlink text is currently not supported.

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

### -CustomTermsOfUseText
A string to replace the the default 'Terms of Use' hyperlink text in the footer.
This text must be in Unicode format and not exceed 256 characters.

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

### -CustomTermsOfUseUrl
A custom URL to replace the default URL of the 'Terms of Use' hyperlink in the footer.
This URL must be in ASCII format or non-ASCII characters must be URL encoded, and not exceed 128characters.

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

### -FaviconInputFile
Input File for Favicon (A custom icon (favicon) to replace a default Microsoft product favicon on a Microsoft Entra tenant.)

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

### -FaviconRelativeUrl
A relative url for the favicon above that is combined with a CDN base URL from the cdnList to provide the version served by a CDN.
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

### -HeaderBackgroundColor
The RGB color to apply to customize the color of the header.

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

### -HeaderLogoInputFile
Input File for HeaderLogo (A company logo that appears in the header of the sign-in page.
The allowed types are PNG or JPEG not larger than 36 × 245 pixels.
We recommend using a transparent image with no padding around the logo.)

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

### -HeaderLogoRelativeUrl
A relative URL for the headerLogo property that is combined with a CDN base URL from the cdnList to provide the read-only version served by a CDN.
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
Type: IIdentityDirectoryManagementIdentity
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -LoginPageLayoutConfiguration
loginPageLayoutConfiguration
To construct, see NOTES section for LOGINPAGELAYOUTCONFIGURATION properties and create a hash table.

```yaml
Type: IMicrosoftGraphLoginPageLayoutConfiguration
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LoginPageTextVisibilitySettings
loginPageTextVisibilitySettings
To construct, see NOTES section for LOGINPAGETEXTVISIBILITYSETTINGS properties and create a hash table.

```yaml
Type: IMicrosoftGraphLoginPageTextVisibilitySettings
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OrganizationId
The unique identifier of organization

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

### -SignInPageText
Text that appears at the bottom of the sign-in box.
Use this to communicate additional information, such as the phone number to your help desk or a legal statement.
This text must be in Unicode format and not exceed 1024 characters.

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

### -SquareLogoDarkInputFile
Input File for SquareLogoDark (A square dark version of your company logo that appears in Windows 10 out-of-box experiences (OOBE) and when Windows Autopilot is enabled for deployment.
Allowed types are PNG or JPEG not larger than 240 x 240 pixels and not more than 10 KB in size.
We recommend using a transparent image with no padding around the logo.)

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

### -SquareLogoDarkRelativeUrl
A relative URL for the squareLogoDark property that is combined with a CDN base URL from the cdnList to provide the version served by a CDN.
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

### -SquareLogoInputFile
Input File for SquareLogo (A square version of your company logo that appears in Windows 10 out-of-box experiences (OOBE) and when Windows Autopilot is enabled for deployment.
Allowed types are PNG or JPEG not larger than 240 x 240 pixels and not more than 10 KB in size.
We recommend using a transparent image with no padding around the logo.)

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

### -SquareLogoRelativeUrl
A relative URL for the squareLogo property that is combined with a CDN base URL from the cdnList to provide the version served by a CDN.
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

### -UsernameHintText
A string that shows as the hint in the username textbox on the sign-in screen.
This text must be a Unicode, without links or code, and can't exceed 64 characters.

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

### Microsoft.Graph.PowerShell.Models.IIdentityDirectoryManagementIdentity
### System.Collections.Hashtable
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphOrganizationalBrandingLocalization
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

CONTENTCUSTOMIZATION `<IMicrosoftGraphContentCustomization>`: contentCustomization
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AttributeCollection <IMicrosoftGraphKeyValue- `[]`>]`: Represents the content options of External Identities to be customized throughout the authentication flow for a tenant.
    - `[Key <String>]`: Key for the key-value pair.
    - `[Value <String>]`: Value for the key-value pair.
  - `[AttributeCollectionRelativeUrl <String>]`: A relative URL for the content options of External Identities to be customized throughout the authentication flow for a tenant.
  - `[RegistrationCampaign <IMicrosoftGraphKeyValue- `[]`>]`: Represents content options to customize during MFA proofup interruptions.
  - `[RegistrationCampaignRelativeUrl <String>]`: The relative URL of the content options to customize during MFA proofup interruptions.

INPUTOBJECT `<IIdentityDirectoryManagementIdentity>`: Identity Parameter
  - `[AdministrativeUnitId <String>]`: The unique identifier of administrativeUnit
  - `[AllowedValueId <String>]`: The unique identifier of allowedValue
  - `[AttributeSetId <String>]`: The unique identifier of attributeSet
  - `[CommerceSubscriptionId <String>]`: Alternate key of companySubscription
  - `[CompanySubscriptionId <String>]`: The unique identifier of companySubscription
  - `[ContractId <String>]`: The unique identifier of contract
  - `[CustomSecurityAttributeDefinitionId <String>]`: The unique identifier of customSecurityAttributeDefinition
  - `[DeviceId <String>]`: The unique identifier of device
  - `[DeviceLocalCredentialInfoId <String>]`: The unique identifier of deviceLocalCredentialInfo
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[DirectoryRoleId <String>]`: The unique identifier of directoryRole
  - `[DirectoryRoleTemplateId <String>]`: The unique identifier of directoryRoleTemplate
  - `[DomainDnsRecordId <String>]`: The unique identifier of domainDnsRecord
  - `[DomainId <String>]`: The unique identifier of domain
  - `[DomainName <String>]`: Usage: domainName='{domainName}'
  - `[ExtensionId <String>]`: The unique identifier of extension
  - `[IdentityProviderBaseId <String>]`: The unique identifier of identityProviderBase
  - `[InternalDomainFederationId <String>]`: The unique identifier of internalDomainFederation
  - `[OnPremisesDirectorySynchronizationId <String>]`: The unique identifier of onPremisesDirectorySynchronization
  - `[OrgContactId <String>]`: The unique identifier of orgContact
  - `[OrganizationId <String>]`: The unique identifier of organization
  - `[OrganizationalBrandingLocalizationId <String>]`: The unique identifier of organizationalBrandingLocalization
  - `[ProfileCardPropertyId <String>]`: The unique identifier of profileCardProperty
  - `[RoleTemplateId <String>]`: Alternate key of directoryRole
  - `[ScopedRoleMembershipId <String>]`: The unique identifier of scopedRoleMembership
  - `[SubscribedSkuId <String>]`: The unique identifier of subscribedSku
  - `[TenantId <String>]`: Usage: tenantId='{tenantId}'
  - `[UserId <String>]`: The unique identifier of user

LOGINPAGELAYOUTCONFIGURATION `<IMicrosoftGraphLoginPageLayoutConfiguration>`: loginPageLayoutConfiguration
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[IsFooterShown <Boolean?>]`: Option to show the footer on the sign-in page.
  - `[IsHeaderShown <Boolean?>]`: Option to show the header on the sign-in page.
  - `[LayoutTemplateType <String>]`: layoutTemplateType

LOGINPAGETEXTVISIBILITYSETTINGS `<IMicrosoftGraphLoginPageTextVisibilitySettings>`: loginPageTextVisibilitySettings
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[HideAccountResetCredentials <Boolean?>]`: Option to hide the self-service password reset (SSPR) hyperlinks such as 'Can't access your account?', 'Forgot my password' and 'Reset it now' on the sign-in form.
  - `[HideCannotAccessYourAccount <Boolean?>]`: Option to hide the self-service password reset (SSPR) 'Can't access your account?' hyperlink on the sign-in form.
  - `[HideForgotMyPassword <Boolean?>]`: Option to hide the self-service password reset (SSPR) 'Forgot my password' hyperlink on the sign-in form.
  - `[HidePrivacyAndCookies <Boolean?>]`: Option to hide the 'Privacy & Cookies' hyperlink in the footer.
  - `[HideResetItNow <Boolean?>]`: Option to hide the self-service password reset (SSPR) 'reset it now' hyperlink on the sign-in form.
  - `[HideTermsOfUse <Boolean?>]`: Option to hide the 'Terms of Use' hyperlink in the footer.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.directorymanagement/new-mgorganizationbrandinglocalization](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.directorymanagement/new-mgorganizationbrandinglocalization)

[https://learn.microsoft.com/graph/api/organizationalbranding-post-localizations?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/organizationalbranding-post-localizations?view=graph-rest-1.0)























