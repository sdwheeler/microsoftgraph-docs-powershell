---
external help file: Microsoft.Graph.Beta.Devices.CorporateManagement-help.xml
Module Name: Microsoft.Graph.Beta.Devices.CorporateManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.corporatemanagement/new-mgbetadeviceappmanagementvpptoken
schema: 2.0.0
---

# New-MgBetaDeviceAppManagementVppToken

## SYNOPSIS
Create new navigation property to vppTokens for deviceAppManagement

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [New-MgDeviceAppManagementVppToken](/powershell/module/Microsoft.Graph.Devices.CorporateManagement/New-MgDeviceAppManagementVppToken?view=graph-powershell-1.0)

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaDeviceAppManagementVppToken [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-AppleId <String>] [-AutomaticallyUpdateApps] [-ClaimTokenManagementFromExternalMdm]
 [-CountryOrRegion <String>] [-DataSharingConsentGranted] [-DisplayName <String>]
 [-ExpirationDateTime <DateTime>] [-Id <String>] [-LastModifiedDateTime <DateTime>]
 [-LastSyncDateTime <DateTime>] [-LastSyncStatus <VppTokenSyncStatus>] [-LocationName <String>]
 [-OrganizationName <String>] [-RoleScopeTagIds <String[]>] [-State <VppTokenState>] [-Token <String>]
 [-TokenActionResults <IMicrosoftGraphVppTokenActionResult[]>] [-VppTokenAccountType <VppTokenAccountType>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaDeviceAppManagementVppToken -BodyParameter <IMicrosoftGraphVppToken>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to vppTokens for deviceAppManagement

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All,  |

## EXAMPLES

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

### -AppleId
The apple Id associated with the given Apple Volume Purchase Program Token.

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

### -AutomaticallyUpdateApps
Whether or not apps for the VPP token will be automatically updated.

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

### -BodyParameter
You purchase multiple licenses for iOS apps through the Apple Volume Purchase Program for Business or Education.
This involves setting up an Apple VPP account from the Apple website and uploading the Apple VPP Business or Education token to Intune.
You can then synchronize your volume purchase information with Intune and track your volume-purchased app use.
You can upload multiple Apple VPP Business or Education tokens.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphVppToken
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ClaimTokenManagementFromExternalMdm
Admin consent to allow claiming token management from external MDM.

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

### -CountryOrRegion
Whether or not apps for the VPP token will be automatically updated.

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

### -DataSharingConsentGranted
Consent granted for data sharing with the Apple Volume Purchase Program.

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

### -DisplayName
An admin specified token friendly name.

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

### -ExpirationDateTime
The expiration date time of the Apple Volume Purchase Program Token.

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

### -LastModifiedDateTime
Last modification date time associated with the Apple Volume Purchase Program Token.

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

### -LastSyncDateTime
The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.

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

### -LastSyncStatus
Possible sync statuses associated with an Apple Volume Purchase Program token.

```yaml
Type: VppTokenSyncStatus
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LocationName
Token location returned from Apple VPP.

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

### -OrganizationName
The organization associated with the Apple Volume Purchase Program Token

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

### -RoleScopeTagIds
Role Scope Tags IDs assigned to this entity.

```yaml
Type: String[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -State
Possible states associated with an Apple Volume Purchase Program token.

```yaml
Type: VppTokenState
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Token
The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.

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

### -TokenActionResults
The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.
To construct, see NOTES section for TOKENACTIONRESULTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphVppTokenActionResult[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -VppTokenAccountType
Possible types of an Apple Volume Purchase Program token.

```yaml
Type: VppTokenAccountType
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphVppToken
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphVppToken
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphVppToken>`: You purchase multiple licenses for iOS apps through the Apple Volume Purchase Program for Business or Education.
This involves setting up an Apple VPP account from the Apple website and uploading the Apple VPP Business or Education token to Intune.
You can then synchronize your volume purchase information with Intune and track your volume-purchased app use.
You can upload multiple Apple VPP Business or Education tokens.
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AppleId <String>]`: The apple Id associated with the given Apple Volume Purchase Program Token.
  - `[AutomaticallyUpdateApps <Boolean?>]`: Whether or not apps for the VPP token will be automatically updated.
  - `[ClaimTokenManagementFromExternalMdm <Boolean?>]`: Admin consent to allow claiming token management from external MDM.
  - `[CountryOrRegion <String>]`: Whether or not apps for the VPP token will be automatically updated.
  - `[DataSharingConsentGranted <Boolean?>]`: Consent granted for data sharing with the Apple Volume Purchase Program.
  - `[DisplayName <String>]`: An admin specified token friendly name.
  - `[ExpirationDateTime <DateTime?>]`: The expiration date time of the Apple Volume Purchase Program Token.
  - `[LastModifiedDateTime <DateTime?>]`: Last modification date time associated with the Apple Volume Purchase Program Token.
  - `[LastSyncDateTime <DateTime?>]`: The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.
  - `[LastSyncStatus <VppTokenSyncStatus?>]`: Possible sync statuses associated with an Apple Volume Purchase Program token.
  - `[LocationName <String>]`: Token location returned from Apple VPP.
  - `[OrganizationName <String>]`: The organization associated with the Apple Volume Purchase Program Token
  - `[RoleScopeTagIds <String- `[]`>]`: Role Scope Tags IDs assigned to this entity.
  - `[State <VppTokenState?>]`: Possible states associated with an Apple Volume Purchase Program token.
  - `[Token <String>]`: The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.
  - `[TokenActionResults <IMicrosoftGraphVppTokenActionResult- `[]`>]`: The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.
    - `[ActionName <String>]`: Action name
    - `[ActionState <String>]`: actionState
    - `[LastUpdatedDateTime <DateTime?>]`: Time the action state was last updated
    - `[StartDateTime <DateTime?>]`: Time the action was initiated
  - `[VppTokenAccountType <VppTokenAccountType?>]`: Possible types of an Apple Volume Purchase Program token.

TOKENACTIONRESULTS `<IMicrosoftGraphVppTokenActionResult- `[]`>`: The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.
  - `[ActionName <String>]`: Action name
  - `[ActionState <String>]`: actionState
  - `[LastUpdatedDateTime <DateTime?>]`: Time the action state was last updated
  - `[StartDateTime <DateTime?>]`: Time the action was initiated

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.corporatemanagement/new-mgbetadeviceappmanagementvpptoken](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devices.corporatemanagement/new-mgbetadeviceappmanagementvpptoken)
























