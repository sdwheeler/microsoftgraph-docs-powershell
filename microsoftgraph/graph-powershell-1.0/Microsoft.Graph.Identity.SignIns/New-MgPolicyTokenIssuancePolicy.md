---
external help file: Microsoft.Graph.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgpolicytokenissuancepolicy
schema: 2.0.0
ms.subservice: entra-sign-in
---

# New-MgPolicyTokenIssuancePolicy

## SYNOPSIS
Create a new tokenIssuancePolicy object.

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaPolicyTokenIssuancePolicy](/powershell/module/Microsoft.Graph.Beta.Identity.SignIns/New-MgBetaPolicyTokenIssuancePolicy?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgPolicyTokenIssuancePolicy [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-AppliesTo <IMicrosoftGraphDirectoryObject[]>] [-Definition <String[]>] [-DeletedDateTime <DateTime>]
 [-Description <String>] [-DisplayName <String>] [-Id <String>] [-IsOrganizationDefault]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgPolicyTokenIssuancePolicy -BodyParameter <Hashtable> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new tokenIssuancePolicy object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Policy.Read.ApplicationConfiguration, Policy.ReadWrite.ApplicationConfiguration,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Policy.Read.ApplicationConfiguration, Policy.ReadWrite.ApplicationConfiguration,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	definition = @(
	"definition-value"
)
displayName = "displayName-value"
isOrganizationDefault = $true
}

New-MgPolicyTokenIssuancePolicy -BodyParameter $params

```
This example shows how to use the New-MgPolicyTokenIssuancePolicy Cmdlet.


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

### -AppliesTo

To construct, see NOTES section for APPLIESTO properties and create a hash table.

```yaml
Type: IMicrosoftGraphDirectoryObject[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
tokenIssuancePolicy

```yaml
Type: Hashtable
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

### -Definition
A string collection containing a JSON string that defines the rules and settings for a policy.
The syntax for the definition differs for each derived policy type.
Required.

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

### -DeletedDateTime
Date and time when this object was deleted.
Always null when the object hasn't been deleted.

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
Description for this policy.
Required.

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
Display name for this policy.
Required.

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

### -IsOrganizationDefault
If set to true, activates this policy.
There can be many policies for the same policy type, but only one can be activated as the organization default.
Optional, default value is false.

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

### System.Collections.Hashtable
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphTokenIssuancePolicy
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

APPLIESTO `<IMicrosoftGraphDirectoryObject- `[]`>`: .
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgpolicytokenissuancepolicy](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.signins/new-mgpolicytokenissuancepolicy)

[https://learn.microsoft.com/graph/api/tokenissuancepolicy-post-tokenissuancepolicy?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/tokenissuancepolicy-post-tokenissuancepolicy?view=graph-rest-1.0)























