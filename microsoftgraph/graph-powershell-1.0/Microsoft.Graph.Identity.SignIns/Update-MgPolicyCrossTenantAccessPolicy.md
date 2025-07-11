---
external help file: Microsoft.Graph.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/update-mgpolicycrosstenantaccesspolicy
schema: 2.0.0
ms.subservice: entra-sign-in
---

# Update-MgPolicyCrossTenantAccessPolicy

## SYNOPSIS
Update the properties of a cross-tenant access policy.

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaPolicyCrossTenantAccessPolicy](/powershell/module/Microsoft.Graph.Beta.Identity.SignIns/Update-MgBetaPolicyCrossTenantAccessPolicy?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgPolicyCrossTenantAccessPolicy [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-AllowedCloudEndpoints <String[]>] [-Default <IMicrosoftGraphCrossTenantAccessPolicyConfigurationDefault>]
 [-DeletedDateTime <DateTime>] [-Description <String>] [-DisplayName <String>] [-Id <String>]
 [-Partners <IMicrosoftGraphCrossTenantAccessPolicyConfigurationPartner[]>]
 [-Templates <IMicrosoftGraphPolicyTemplate>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgPolicyCrossTenantAccessPolicy -BodyParameter <IMicrosoftGraphCrossTenantAccessPolicy>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the properties of a cross-tenant access policy.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Policy.ReadWrite.CrossTenantAccess,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Policy.ReadWrite.CrossTenantAccess,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	allowedCloudEndpoints = @(
	"microsoftonline.us"
)
}

Update-MgPolicyCrossTenantAccessPolicy -BodyParameter $params

```
This example shows how to use the Update-MgPolicyCrossTenantAccessPolicy Cmdlet.


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

### -AllowedCloudEndpoints
Used to specify which Microsoft clouds an organization would like to collaborate with.
By default, this value is empty.
Supported values for this field are: microsoftonline.com, microsoftonline.us, and partner.microsoftonline.cn.

```yaml
Type: String[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
crossTenantAccessPolicy
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphCrossTenantAccessPolicy
Parameter Sets: Update
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

### -Default
crossTenantAccessPolicyConfigurationDefault
To construct, see NOTES section for DEFAULT properties and create a hash table.

```yaml
Type: IMicrosoftGraphCrossTenantAccessPolicyConfigurationDefault
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeletedDateTime
Date and time when this object was deleted.
Always null when the object hasn't been deleted.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
Description for this policy.
Required.

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

### -DisplayName
Display name for this policy.
Required.

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

### -Partners
Defines partner-specific configurations for external Microsoft Entra organizations.
To construct, see NOTES section for PARTNERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphCrossTenantAccessPolicyConfigurationPartner[]
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

### -Templates
policyTemplate
To construct, see NOTES section for TEMPLATES properties and create a hash table.

```yaml
Type: IMicrosoftGraphPolicyTemplate
Parameter Sets: UpdateExpanded
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphCrossTenantAccessPolicy
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphCrossTenantAccessPolicy
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphCrossTenantAccessPolicy>`: crossTenantAccessPolicy
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Description <String>]`: Description for this policy.
Required.
  - `[DisplayName <String>]`: Display name for this policy.
Required.
  - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AllowedCloudEndpoints <String- `[]`>]`: Used to specify which Microsoft clouds an organization would like to collaborate with.
By default, this value is empty.
Supported values for this field are: microsoftonline.com, microsoftonline.us, and partner.microsoftonline.cn.
  - `[Default <IMicrosoftGraphCrossTenantAccessPolicyConfigurationDefault>]`: crossTenantAccessPolicyConfigurationDefault
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AutomaticUserConsentSettings <IMicrosoftGraphInboundOutboundPolicyConfiguration>]`: inboundOutboundPolicyConfiguration
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[InboundAllowed <Boolean?>]`: Defines whether external users coming inbound are allowed.
      - `[OutboundAllowed <Boolean?>]`: Defines whether internal users are allowed to go outbound.
    - `[B2BCollaborationInbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Applications <IMicrosoftGraphCrossTenantAccessPolicyTargetConfiguration>]`: crossTenantAccessPolicyTargetConfiguration
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[AccessType <String>]`: crossTenantAccessPolicyTargetConfigurationAccessType
        - `[Targets <IMicrosoftGraphCrossTenantAccessPolicyTarget- `[]`>]`: Specifies whether to target users, groups, or applications with this rule.
          - `[Target <String>]`: Defines the target for cross-tenant access policy settings and can have one of the following values:  The unique identifier of the user, group, or application  AllUsers  AllApplications - Refers to any Microsoft cloud application.
Office365 - Includes the applications mentioned as part of the Office 365 suite.
          - `[TargetType <String>]`: crossTenantAccessPolicyTargetType
      - `[UsersAndGroups <IMicrosoftGraphCrossTenantAccessPolicyTargetConfiguration>]`: crossTenantAccessPolicyTargetConfiguration
    - `[B2BCollaborationOutbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
    - `[B2BDirectConnectInbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
    - `[B2BDirectConnectOutbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
    - `[InboundTrust <IMicrosoftGraphCrossTenantAccessPolicyInboundTrust>]`: crossTenantAccessPolicyInboundTrust
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IsCompliantDeviceAccepted <Boolean?>]`: Specifies whether compliant devices from external Microsoft Entra organizations are trusted.
      - `[IsHybridAzureAdJoinedDeviceAccepted <Boolean?>]`: Specifies whether Microsoft Entra hybrid joined devices from external Microsoft Entra organizations are trusted.
      - `[IsMfaAccepted <Boolean?>]`: Specifies whether MFA from external Microsoft Entra organizations is trusted.
    - `[InvitationRedemptionIdentityProviderConfiguration <IMicrosoftGraphDefaultInvitationRedemptionIdentityProviderConfiguration>]`: defaultInvitationRedemptionIdentityProviderConfiguration
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[FallbackIdentityProvider <String>]`: b2bIdentityProvidersType
      - `[PrimaryIdentityProviderPrecedenceOrder <String- `[]`>]`: Collection of identity providers in priority order of preference to be used for guest invitation redemption.
Possible values are: azureActiveDirectory, externalFederation, or socialIdentityProviders.
    - `[IsServiceDefault <Boolean?>]`: If true, the default configuration is set to the system default configuration.
If false, the default settings are customized.
    - `[TenantRestrictions <IMicrosoftGraphCrossTenantAccessPolicyTenantRestrictions>]`: crossTenantAccessPolicyTenantRestrictions
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Applications <IMicrosoftGraphCrossTenantAccessPolicyTargetConfiguration>]`: crossTenantAccessPolicyTargetConfiguration
      - `[UsersAndGroups <IMicrosoftGraphCrossTenantAccessPolicyTargetConfiguration>]`: crossTenantAccessPolicyTargetConfiguration
      - `[Devices <IMicrosoftGraphDevicesFilter>]`: devicesFilter
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Mode <String>]`: crossTenantAccessPolicyTargetConfigurationAccessType
        - `[Rule <String>]`: Defines the rule to filter the devices.
For example, device.deviceAttribute2 -eq 'PrivilegedAccessWorkstation'.
  - `[Partners <IMicrosoftGraphCrossTenantAccessPolicyConfigurationPartner- `[]`>]`: Defines partner-specific configurations for external Microsoft Entra organizations.
    - `[AutomaticUserConsentSettings <IMicrosoftGraphInboundOutboundPolicyConfiguration>]`: inboundOutboundPolicyConfiguration
    - `[B2BCollaborationInbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
    - `[B2BCollaborationOutbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
    - `[B2BDirectConnectInbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
    - `[B2BDirectConnectOutbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
    - `[IdentitySynchronization <IMicrosoftGraphCrossTenantIdentitySyncPolicyPartner>]`: crossTenantIdentitySyncPolicyPartner
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: Display name for the cross-tenant user synchronization policy.
Use the name of the partner Microsoft Entra tenant to easily identify the policy.
Optional.
      - `[TenantId <String>]`: Tenant identifier for the partner Microsoft Entra organization.
Read-only.
      - `[UserSyncInbound <IMicrosoftGraphCrossTenantUserSyncInbound>]`: crossTenantUserSyncInbound
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[IsSyncAllowed <Boolean?>]`: Defines whether user objects should be synchronized from the partner tenant.
false causes any current user synchronization from the source tenant to the target tenant to stop.
This property has no impact on existing users who have already been synchronized.
    - `[InboundTrust <IMicrosoftGraphCrossTenantAccessPolicyInboundTrust>]`: crossTenantAccessPolicyInboundTrust
    - `[IsInMultiTenantOrganization <Boolean?>]`: Identifies whether a tenant is a member of a multitenant organization.
    - `[IsServiceProvider <Boolean?>]`: Identifies whether the partner-specific configuration is a Cloud Service Provider for your organization.
    - `[TenantId <String>]`: The tenant identifier for the partner Microsoft Entra organization.
Read-only.
Key.
    - `[TenantRestrictions <IMicrosoftGraphCrossTenantAccessPolicyTenantRestrictions>]`: crossTenantAccessPolicyTenantRestrictions
  - `[Templates <IMicrosoftGraphPolicyTemplate>]`: policyTemplate
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[MultiTenantOrganizationIdentitySynchronization <IMicrosoftGraphMultiTenantOrganizationIdentitySyncPolicyTemplate>]`: multiTenantOrganizationIdentitySyncPolicyTemplate
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[TemplateApplicationLevel <String>]`: templateApplicationLevel
      - `[UserSyncInbound <IMicrosoftGraphCrossTenantUserSyncInbound>]`: crossTenantUserSyncInbound
    - `[MultiTenantOrganizationPartnerConfiguration <IMicrosoftGraphMultiTenantOrganizationPartnerConfigurationTemplate>]`: multiTenantOrganizationPartnerConfigurationTemplate
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AutomaticUserConsentSettings <IMicrosoftGraphInboundOutboundPolicyConfiguration>]`: inboundOutboundPolicyConfiguration
      - `[B2BCollaborationInbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
      - `[B2BCollaborationOutbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
      - `[B2BDirectConnectInbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
      - `[B2BDirectConnectOutbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
      - `[InboundTrust <IMicrosoftGraphCrossTenantAccessPolicyInboundTrust>]`: crossTenantAccessPolicyInboundTrust
      - `[TemplateApplicationLevel <String>]`: templateApplicationLevel

DEFAULT `<IMicrosoftGraphCrossTenantAccessPolicyConfigurationDefault>`: crossTenantAccessPolicyConfigurationDefault
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AutomaticUserConsentSettings <IMicrosoftGraphInboundOutboundPolicyConfiguration>]`: inboundOutboundPolicyConfiguration
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[InboundAllowed <Boolean?>]`: Defines whether external users coming inbound are allowed.
    - `[OutboundAllowed <Boolean?>]`: Defines whether internal users are allowed to go outbound.
  - `[B2BCollaborationInbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Applications <IMicrosoftGraphCrossTenantAccessPolicyTargetConfiguration>]`: crossTenantAccessPolicyTargetConfiguration
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[AccessType <String>]`: crossTenantAccessPolicyTargetConfigurationAccessType
      - `[Targets <IMicrosoftGraphCrossTenantAccessPolicyTarget- `[]`>]`: Specifies whether to target users, groups, or applications with this rule.
        - `[Target <String>]`: Defines the target for cross-tenant access policy settings and can have one of the following values:  The unique identifier of the user, group, or application  AllUsers  AllApplications - Refers to any Microsoft cloud application.
Office365 - Includes the applications mentioned as part of the Office 365 suite.
        - `[TargetType <String>]`: crossTenantAccessPolicyTargetType
    - `[UsersAndGroups <IMicrosoftGraphCrossTenantAccessPolicyTargetConfiguration>]`: crossTenantAccessPolicyTargetConfiguration
  - `[B2BCollaborationOutbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
  - `[B2BDirectConnectInbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
  - `[B2BDirectConnectOutbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
  - `[InboundTrust <IMicrosoftGraphCrossTenantAccessPolicyInboundTrust>]`: crossTenantAccessPolicyInboundTrust
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IsCompliantDeviceAccepted <Boolean?>]`: Specifies whether compliant devices from external Microsoft Entra organizations are trusted.
    - `[IsHybridAzureAdJoinedDeviceAccepted <Boolean?>]`: Specifies whether Microsoft Entra hybrid joined devices from external Microsoft Entra organizations are trusted.
    - `[IsMfaAccepted <Boolean?>]`: Specifies whether MFA from external Microsoft Entra organizations is trusted.
  - `[InvitationRedemptionIdentityProviderConfiguration <IMicrosoftGraphDefaultInvitationRedemptionIdentityProviderConfiguration>]`: defaultInvitationRedemptionIdentityProviderConfiguration
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[FallbackIdentityProvider <String>]`: b2bIdentityProvidersType
    - `[PrimaryIdentityProviderPrecedenceOrder <String- `[]`>]`: Collection of identity providers in priority order of preference to be used for guest invitation redemption.
Possible values are: azureActiveDirectory, externalFederation, or socialIdentityProviders.
  - `[IsServiceDefault <Boolean?>]`: If true, the default configuration is set to the system default configuration.
If false, the default settings are customized.
  - `[TenantRestrictions <IMicrosoftGraphCrossTenantAccessPolicyTenantRestrictions>]`: crossTenantAccessPolicyTenantRestrictions
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Applications <IMicrosoftGraphCrossTenantAccessPolicyTargetConfiguration>]`: crossTenantAccessPolicyTargetConfiguration
    - `[UsersAndGroups <IMicrosoftGraphCrossTenantAccessPolicyTargetConfiguration>]`: crossTenantAccessPolicyTargetConfiguration
    - `[Devices <IMicrosoftGraphDevicesFilter>]`: devicesFilter
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Mode <String>]`: crossTenantAccessPolicyTargetConfigurationAccessType
      - `[Rule <String>]`: Defines the rule to filter the devices.
For example, device.deviceAttribute2 -eq 'PrivilegedAccessWorkstation'.

PARTNERS `<IMicrosoftGraphCrossTenantAccessPolicyConfigurationPartner- `[]`>`: Defines partner-specific configurations for external Microsoft Entra organizations.
  - `[AutomaticUserConsentSettings <IMicrosoftGraphInboundOutboundPolicyConfiguration>]`: inboundOutboundPolicyConfiguration
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[InboundAllowed <Boolean?>]`: Defines whether external users coming inbound are allowed.
    - `[OutboundAllowed <Boolean?>]`: Defines whether internal users are allowed to go outbound.
  - `[B2BCollaborationInbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Applications <IMicrosoftGraphCrossTenantAccessPolicyTargetConfiguration>]`: crossTenantAccessPolicyTargetConfiguration
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[AccessType <String>]`: crossTenantAccessPolicyTargetConfigurationAccessType
      - `[Targets <IMicrosoftGraphCrossTenantAccessPolicyTarget- `[]`>]`: Specifies whether to target users, groups, or applications with this rule.
        - `[Target <String>]`: Defines the target for cross-tenant access policy settings and can have one of the following values:  The unique identifier of the user, group, or application  AllUsers  AllApplications - Refers to any Microsoft cloud application.
Office365 - Includes the applications mentioned as part of the Office 365 suite.
        - `[TargetType <String>]`: crossTenantAccessPolicyTargetType
    - `[UsersAndGroups <IMicrosoftGraphCrossTenantAccessPolicyTargetConfiguration>]`: crossTenantAccessPolicyTargetConfiguration
  - `[B2BCollaborationOutbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
  - `[B2BDirectConnectInbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
  - `[B2BDirectConnectOutbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
  - `[IdentitySynchronization <IMicrosoftGraphCrossTenantIdentitySyncPolicyPartner>]`: crossTenantIdentitySyncPolicyPartner
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: Display name for the cross-tenant user synchronization policy.
Use the name of the partner Microsoft Entra tenant to easily identify the policy.
Optional.
    - `[TenantId <String>]`: Tenant identifier for the partner Microsoft Entra organization.
Read-only.
    - `[UserSyncInbound <IMicrosoftGraphCrossTenantUserSyncInbound>]`: crossTenantUserSyncInbound
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IsSyncAllowed <Boolean?>]`: Defines whether user objects should be synchronized from the partner tenant.
false causes any current user synchronization from the source tenant to the target tenant to stop.
This property has no impact on existing users who have already been synchronized.
  - `[InboundTrust <IMicrosoftGraphCrossTenantAccessPolicyInboundTrust>]`: crossTenantAccessPolicyInboundTrust
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[IsCompliantDeviceAccepted <Boolean?>]`: Specifies whether compliant devices from external Microsoft Entra organizations are trusted.
    - `[IsHybridAzureAdJoinedDeviceAccepted <Boolean?>]`: Specifies whether Microsoft Entra hybrid joined devices from external Microsoft Entra organizations are trusted.
    - `[IsMfaAccepted <Boolean?>]`: Specifies whether MFA from external Microsoft Entra organizations is trusted.
  - `[IsInMultiTenantOrganization <Boolean?>]`: Identifies whether a tenant is a member of a multitenant organization.
  - `[IsServiceProvider <Boolean?>]`: Identifies whether the partner-specific configuration is a Cloud Service Provider for your organization.
  - `[TenantId <String>]`: The tenant identifier for the partner Microsoft Entra organization.
Read-only.
Key.
  - `[TenantRestrictions <IMicrosoftGraphCrossTenantAccessPolicyTenantRestrictions>]`: crossTenantAccessPolicyTenantRestrictions
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Applications <IMicrosoftGraphCrossTenantAccessPolicyTargetConfiguration>]`: crossTenantAccessPolicyTargetConfiguration
    - `[UsersAndGroups <IMicrosoftGraphCrossTenantAccessPolicyTargetConfiguration>]`: crossTenantAccessPolicyTargetConfiguration
    - `[Devices <IMicrosoftGraphDevicesFilter>]`: devicesFilter
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Mode <String>]`: crossTenantAccessPolicyTargetConfigurationAccessType
      - `[Rule <String>]`: Defines the rule to filter the devices.
For example, device.deviceAttribute2 -eq 'PrivilegedAccessWorkstation'.

TEMPLATES `<IMicrosoftGraphPolicyTemplate>`: policyTemplate
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[MultiTenantOrganizationIdentitySynchronization <IMicrosoftGraphMultiTenantOrganizationIdentitySyncPolicyTemplate>]`: multiTenantOrganizationIdentitySyncPolicyTemplate
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[TemplateApplicationLevel <String>]`: templateApplicationLevel
    - `[UserSyncInbound <IMicrosoftGraphCrossTenantUserSyncInbound>]`: crossTenantUserSyncInbound
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IsSyncAllowed <Boolean?>]`: Defines whether user objects should be synchronized from the partner tenant.
false causes any current user synchronization from the source tenant to the target tenant to stop.
This property has no impact on existing users who have already been synchronized.
  - `[MultiTenantOrganizationPartnerConfiguration <IMicrosoftGraphMultiTenantOrganizationPartnerConfigurationTemplate>]`: multiTenantOrganizationPartnerConfigurationTemplate
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AutomaticUserConsentSettings <IMicrosoftGraphInboundOutboundPolicyConfiguration>]`: inboundOutboundPolicyConfiguration
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[InboundAllowed <Boolean?>]`: Defines whether external users coming inbound are allowed.
      - `[OutboundAllowed <Boolean?>]`: Defines whether internal users are allowed to go outbound.
    - `[B2BCollaborationInbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Applications <IMicrosoftGraphCrossTenantAccessPolicyTargetConfiguration>]`: crossTenantAccessPolicyTargetConfiguration
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[AccessType <String>]`: crossTenantAccessPolicyTargetConfigurationAccessType
        - `[Targets <IMicrosoftGraphCrossTenantAccessPolicyTarget- `[]`>]`: Specifies whether to target users, groups, or applications with this rule.
          - `[Target <String>]`: Defines the target for cross-tenant access policy settings and can have one of the following values:  The unique identifier of the user, group, or application  AllUsers  AllApplications - Refers to any Microsoft cloud application.
Office365 - Includes the applications mentioned as part of the Office 365 suite.
          - `[TargetType <String>]`: crossTenantAccessPolicyTargetType
      - `[UsersAndGroups <IMicrosoftGraphCrossTenantAccessPolicyTargetConfiguration>]`: crossTenantAccessPolicyTargetConfiguration
    - `[B2BCollaborationOutbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
    - `[B2BDirectConnectInbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
    - `[B2BDirectConnectOutbound <IMicrosoftGraphCrossTenantAccessPolicyB2BSetting>]`: crossTenantAccessPolicyB2BSetting
    - `[InboundTrust <IMicrosoftGraphCrossTenantAccessPolicyInboundTrust>]`: crossTenantAccessPolicyInboundTrust
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[IsCompliantDeviceAccepted <Boolean?>]`: Specifies whether compliant devices from external Microsoft Entra organizations are trusted.
      - `[IsHybridAzureAdJoinedDeviceAccepted <Boolean?>]`: Specifies whether Microsoft Entra hybrid joined devices from external Microsoft Entra organizations are trusted.
      - `[IsMfaAccepted <Boolean?>]`: Specifies whether MFA from external Microsoft Entra organizations is trusted.
    - `[TemplateApplicationLevel <String>]`: templateApplicationLevel

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/update-mgpolicycrosstenantaccesspolicy](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/update-mgpolicycrosstenantaccesspolicy)

[https://learn.microsoft.com/graph/api/crosstenantaccesspolicy-update?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/crosstenantaccesspolicy-update?view=graph-rest-1.0)























