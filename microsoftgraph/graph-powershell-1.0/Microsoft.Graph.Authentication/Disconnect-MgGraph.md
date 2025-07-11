﻿---
external help file: Microsoft.Graph.Authentication.dll-Help.xml
Module Name: Microsoft.Graph.Authentication
online version: https://learn.microsoft.com/en-us/powershell/module/microsoft.graph.authentication/disconnect-graph
schema: 2.0.0
---

# Disconnect-MgGraph

## SYNOPSIS
Use Disconnect-MgGraph to sign out.

## SYNTAX

```
Disconnect-MgGraph [<CommonParameters>]
```

## DESCRIPTION

Once you're signed in, you'll remain signed in until you invoke Disconnect-MgGraph. Microsoft Graph
PowerShell automatically refreshes the access token for you and sign-in persists across PowerShell
sessions because Microsoft Graph PowerShell securely caches the token.

## EXAMPLES

### Example 1: Using Disconnect-MgGraph
```
PS C:\> Disconnect-MgGraph
```

Use Disconnect-MgGraph to sign out.

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
## OUTPUTS

### Microsoft.Graph.PowerShell.Authentication.IAuthContext
## NOTES

## RELATED LINKS
