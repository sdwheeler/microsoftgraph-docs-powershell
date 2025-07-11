---
external help file: Microsoft.Graph.Beta.Security-help.xml
Module Name: Microsoft.Graph.Beta.Security
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/get-mgbetasecurityidentitysensordeploymentaccesskey
schema: 2.0.0
ms.subservice: security
---

# Get-MgBetaSecurityIdentitySensorDeploymentAccessKey

## SYNOPSIS
Get the deployment access key associated with a Microsoft Defender for Identity, needed to install sensors associated with the workspace.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Get-MgSecurityIdentitySensorDeploymentAccessKey](/powershell/module/Microsoft.Graph.Security/Get-MgSecurityIdentitySensorDeploymentAccessKey?view=graph-powershell-1.0)

## SYNTAX

```
Get-MgBetaSecurityIdentitySensorDeploymentAccessKey [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [<CommonParameters>]
```

## DESCRIPTION
Get the deployment access key associated with a Microsoft Defender for Identity, needed to install sensors associated with the workspace.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | SecurityIdentitiesSensors.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | SecurityIdentitiesSensors.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Security

Get-MgBetaSecurityIdentitySensorDeploymentAccessKey

```
This example shows how to use the Get-MgBetaSecurityIdentitySensorDeploymentAccessKey Cmdlet.


## PARAMETERS

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

### System.String
## NOTES

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/get-mgbetasecurityidentitysensordeploymentaccesskey](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/get-mgbetasecurityidentitysensordeploymentaccesskey)

[https://learn.microsoft.com/graph/api/security-sensor-getdeploymentaccesskey?view=graph-rest-beta](https://learn.microsoft.com/graph/api/security-sensor-getdeploymentaccesskey?view=graph-rest-beta)























