---
external help file: Microsoft.Graph.Beta.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Beta.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/get-mgbetapolicyadminconsentrequestpolicy
schema: 2.0.0
ms.subservice: entra-id-governance
---

# Get-MgBetaPolicyAdminConsentRequestPolicy

## SYNOPSIS
Read the properties and relationships of an adminConsentRequestPolicy object.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Get-MgPolicyAdminConsentRequestPolicy](/powershell/module/Microsoft.Graph.Identity.SignIns/Get-MgPolicyAdminConsentRequestPolicy?view=graph-powershell-1.0)

## SYNTAX

```
Get-MgBetaPolicyAdminConsentRequestPolicy [-ExpandProperty <String[]>] [-Property <String[]>]
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

## DESCRIPTION
Read the properties and relationships of an adminConsentRequestPolicy object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.ReadWrite.All, Directory.Read.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.ReadWrite.All, Directory.Read.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Identity.SignIns

Get-MgBetaPolicyAdminConsentRequestPolicy

```
This example shows how to use the Get-MgBetaPolicyAdminConsentRequestPolicy Cmdlet.


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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphAdminConsentRequestPolicy
## NOTES

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/get-mgbetapolicyadminconsentrequestpolicy](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/get-mgbetapolicyadminconsentrequestpolicy)

[https://learn.microsoft.com/graph/api/adminconsentrequestpolicy-get?view=graph-rest-beta](https://learn.microsoft.com/graph/api/adminconsentrequestpolicy-get?view=graph-rest-beta)























