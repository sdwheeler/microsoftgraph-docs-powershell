---
external help file: Microsoft.Graph.Beta.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Beta.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/get-mgbetapolicycrosstenantaccesspolicydefault
schema: 2.0.0
ms.subservice: entra-sign-in
---

# Get-MgBetaPolicyCrossTenantAccessPolicyDefault

## SYNOPSIS
Read the default configuration of a cross-tenant access policy.
This default configuration may be the service default assigned by Microsoft Entra ID (isServiceDefault is true) or may be customized in your tenant (isServiceDefault is false).

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Get-MgPolicyCrossTenantAccessPolicyDefault](/powershell/module/Microsoft.Graph.Identity.SignIns/Get-MgPolicyCrossTenantAccessPolicyDefault?view=graph-powershell-1.0)

## SYNTAX

```
Get-MgBetaPolicyCrossTenantAccessPolicyDefault [-ExpandProperty <String[]>] [-Property <String[]>]
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

## DESCRIPTION
Read the default configuration of a cross-tenant access policy.
This default configuration may be the service default assigned by Microsoft Entra ID (isServiceDefault is true) or may be customized in your tenant (isServiceDefault is false).

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Policy.Read.All, Policy.ReadWrite.CrossTenantAccess,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Policy.Read.All, Policy.ReadWrite.CrossTenantAccess,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Identity.SignIns

Get-MgBetaPolicyCrossTenantAccessPolicyDefault

```
This example shows how to use the Get-MgBetaPolicyCrossTenantAccessPolicyDefault Cmdlet.


## PARAMETERS

### -ExpandProperty
Expand related entities

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Expand

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

### -Property
Select properties to be returned

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Select

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphCrossTenantAccessPolicyConfigurationDefault
## NOTES

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/get-mgbetapolicycrosstenantaccesspolicydefault](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/get-mgbetapolicycrosstenantaccesspolicydefault)

[https://learn.microsoft.com/graph/api/crosstenantaccesspolicyconfigurationdefault-get?view=graph-rest-beta](https://learn.microsoft.com/graph/api/crosstenantaccesspolicyconfigurationdefault-get?view=graph-rest-beta)























