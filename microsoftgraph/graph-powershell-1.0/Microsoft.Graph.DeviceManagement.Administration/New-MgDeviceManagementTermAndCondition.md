---
external help file: Microsoft.Graph.DeviceManagement.Administration-help.xml
Module Name: Microsoft.Graph.DeviceManagement.Administration
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement.administration/new-mgdevicemanagementtermandcondition
schema: 2.0.0
ms.subservice: intune
---

# New-MgDeviceManagementTermAndCondition

## SYNOPSIS
Create a new termsAndConditions object.

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaDeviceManagementTermAndCondition](/powershell/module/Microsoft.Graph.Beta.DeviceManagement.Administration/New-MgBetaDeviceManagementTermAndCondition?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgDeviceManagementTermAndCondition [-ResponseHeadersVariable <String>] [-AcceptanceStatement <String>]
 [-AcceptanceStatuses <IMicrosoftGraphTermsAndConditionsAcceptanceStatus[]>]
 [-AdditionalProperties <Hashtable>] [-Assignments <IMicrosoftGraphTermsAndConditionsAssignment[]>]
 [-BodyText <String>] [-CreatedDateTime <DateTime>] [-Description <String>] [-DisplayName <String>]
 [-Id <String>] [-LastModifiedDateTime <DateTime>] [-Title <String>] [-Version <Int32>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgDeviceManagementTermAndCondition -BodyParameter <IMicrosoftGraphTermsAndConditions>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new termsAndConditions object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | DeviceManagementServiceConfig.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | DeviceManagementServiceConfig.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

$params = @{
	"@odata.type" = "#microsoft.graph.termsAndConditions"
	displayName = "Display Name value"
	description = "Description value"
	title = "Title value"
	bodyText = "Body Text value"
	acceptanceStatement = "Acceptance Statement value"
	version = 7
}

New-MgDeviceManagementTermAndCondition -BodyParameter $params

```
This example shows how to use the New-MgDeviceManagementTermAndCondition Cmdlet.


## PARAMETERS

### -AcceptanceStatement
Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.
This is shown to the user on prompts to accept the T&C policy.

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

### -AcceptanceStatuses
The list of acceptance statuses for this T&C policy.
To construct, see NOTES section for ACCEPTANCESTATUSES properties and create a hash table.

```yaml
Type: IMicrosoftGraphTermsAndConditionsAcceptanceStatus[]
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

### -Assignments
The list of assignments for this T&C policy.
To construct, see NOTES section for ASSIGNMENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphTermsAndConditionsAssignment[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy.
T&C policies' contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance.
They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphTermsAndConditions
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -BodyText
Administrator-supplied body text of the terms and conditions, typically the terms themselves.
This is shown to the user on prompts to accept the T&C policy.

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

### -CreatedDateTime
DateTime the object was created.

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

### -Description
Administrator-supplied description of the T&C policy.

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

### -DisplayName
Administrator-supplied name for the T&C policy.

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

### -LastModifiedDateTime
DateTime the object was last modified.

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

### -Title
Administrator-supplied title of the terms and conditions.
This is shown to the user on prompts to accept the T&C policy.

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

### -Version
Integer indicating the current version of the terms.
Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.

```yaml
Type: Int32
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: 0
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphTermsAndConditions
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphTermsAndConditions
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ACCEPTANCESTATUSES `<IMicrosoftGraphTermsAndConditionsAcceptanceStatus- `[]`>`: The list of acceptance statuses for this T&C policy.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AcceptedDateTime <DateTime?>]`: DateTime when the terms were last accepted by the user.
  - `[AcceptedVersion <Int32?>]`: Most recent version number of the T&C accepted by the user.
  - `[TermsAndConditions <IMicrosoftGraphTermsAndConditions>]`: A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy.
T&C policies' contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance.
They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AcceptanceStatement <String>]`: Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.
This is shown to the user on prompts to accept the T&C policy.
    - `[AcceptanceStatuses <IMicrosoftGraphTermsAndConditionsAcceptanceStatus- `[]`>]`: The list of acceptance statuses for this T&C policy.
    - `[Assignments <IMicrosoftGraphTermsAndConditionsAssignment- `[]`>]`: The list of assignments for this T&C policy.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Target <IMicrosoftGraphDeviceAndAppManagementAssignmentTarget>]`: Base type for assignment targets.
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[BodyText <String>]`: Administrator-supplied body text of the terms and conditions, typically the terms themselves.
This is shown to the user on prompts to accept the T&C policy.
    - `[CreatedDateTime <DateTime?>]`: DateTime the object was created.
    - `[Description <String>]`: Administrator-supplied description of the T&C policy.
    - `[DisplayName <String>]`: Administrator-supplied name for the T&C policy.
    - `[LastModifiedDateTime <DateTime?>]`: DateTime the object was last modified.
    - `[Title <String>]`: Administrator-supplied title of the terms and conditions.
This is shown to the user on prompts to accept the T&C policy.
    - `[Version <Int32?>]`: Integer indicating the current version of the terms.
Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.
  - `[UserDisplayName <String>]`: Display name of the user whose acceptance the entity represents.
  - `[UserPrincipalName <String>]`: The userPrincipalName of the User that accepted the term.

ASSIGNMENTS `<IMicrosoftGraphTermsAndConditionsAssignment- `[]`>`: The list of assignments for this T&C policy.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Target <IMicrosoftGraphDeviceAndAppManagementAssignmentTarget>]`: Base type for assignment targets.
    - `[(Any) <Object>]`: This indicates any property can be added to this object.

BODYPARAMETER `<IMicrosoftGraphTermsAndConditions>`: A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy.
T&C policies' contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance.
They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AcceptanceStatement <String>]`: Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.
This is shown to the user on prompts to accept the T&C policy.
  - `[AcceptanceStatuses <IMicrosoftGraphTermsAndConditionsAcceptanceStatus- `[]`>]`: The list of acceptance statuses for this T&C policy.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AcceptedDateTime <DateTime?>]`: DateTime when the terms were last accepted by the user.
    - `[AcceptedVersion <Int32?>]`: Most recent version number of the T&C accepted by the user.
    - `[TermsAndConditions <IMicrosoftGraphTermsAndConditions>]`: A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy.
T&C policies' contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance.
They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.
    - `[UserDisplayName <String>]`: Display name of the user whose acceptance the entity represents.
    - `[UserPrincipalName <String>]`: The userPrincipalName of the User that accepted the term.
  - `[Assignments <IMicrosoftGraphTermsAndConditionsAssignment- `[]`>]`: The list of assignments for this T&C policy.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Target <IMicrosoftGraphDeviceAndAppManagementAssignmentTarget>]`: Base type for assignment targets.
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[BodyText <String>]`: Administrator-supplied body text of the terms and conditions, typically the terms themselves.
This is shown to the user on prompts to accept the T&C policy.
  - `[CreatedDateTime <DateTime?>]`: DateTime the object was created.
  - `[Description <String>]`: Administrator-supplied description of the T&C policy.
  - `[DisplayName <String>]`: Administrator-supplied name for the T&C policy.
  - `[LastModifiedDateTime <DateTime?>]`: DateTime the object was last modified.
  - `[Title <String>]`: Administrator-supplied title of the terms and conditions.
This is shown to the user on prompts to accept the T&C policy.
  - `[Version <Int32?>]`: Integer indicating the current version of the terms.
Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement.administration/new-mgdevicemanagementtermandcondition](https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement.administration/new-mgdevicemanagementtermandcondition)

[https://learn.microsoft.com/graph/api/intune-companyterms-termsandconditions-create?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/intune-companyterms-termsandconditions-create?view=graph-rest-1.0)























