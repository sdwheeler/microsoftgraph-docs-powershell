---
external help file: Microsoft.Graph.Beta.Security-help.xml
Module Name: Microsoft.Graph.Beta.Security
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/new-mgbetasecurityaction
schema: 2.0.0
ms.subservice: security
---

# New-MgBetaSecurityAction

## SYNOPSIS
Create a new securityAction object.

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaSecurityAction [-ResponseHeadersVariable <String>] [-ActionReason <String>]
 [-AdditionalProperties <Hashtable>] [-AppId <String>] [-AzureTenantId <String>] [-ClientContext <String>]
 [-CompletedDateTime <DateTime>] [-CreatedDateTime <DateTime>] [-ErrorInfo <IMicrosoftGraphResultInfo>]
 [-Id <String>] [-LastActionDateTime <DateTime>] [-Name <String>] [-Parameters <IMicrosoftGraphKeyValuePair[]>]
 [-States <IMicrosoftGraphSecurityActionState[]>] [-Status <String>] [-User <String>]
 [-VendorInformation <IMicrosoftGraphSecurityVendorInformation>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaSecurityAction -BodyParameter <IMicrosoftGraphSecurityAction> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create a new securityAction object.

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	name = "BlockIp"
	actionReason = "Test"
	parameters = @(
		@{
			name = "IP"
			value = "1.2.3.4"
		}
	)
	vendorInformation = @{
		provider = "Windows Defender ATP"
		vendor = "Microsoft"
	}
}

New-MgBetaSecurityAction -BodyParameter $params

```
This example shows how to use the New-MgBetaSecurityAction Cmdlet.


## PARAMETERS

### -ActionReason
Reason for invoking this action.

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

### -AppId
The Application ID of the calling application that submitted (POST) the action.
The appId should be extracted from the auth token and not entered manually by the calling application.

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

### -AzureTenantId
Azure tenant ID of the entity to determine which tenant the entity belongs to (multi-tenancy support).
The azureTenantId should be extracted from the auth token and not entered manually by the calling application.

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

### -BodyParameter
securityAction
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityAction
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ClientContext
Unique client context string.
Can have a maximum of 256 characters.

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

### -CompletedDateTime
Timestamp when the action was completed.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.

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
Timestamp when the action is created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.

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

### -ErrorInfo
resultInfo
To construct, see NOTES section for ERRORINFO properties and create a hash table.

```yaml
Type: IMicrosoftGraphResultInfo
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

### -LastActionDateTime
Timestamp when this action was last updated.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.

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

### -Name
Action name.

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

### -Parameters
Collection of parameters (key-value pairs) necessary to invoke the action, for example, URL or fileHash to block.).
Required.
To construct, see NOTES section for PARAMETERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphKeyValuePair[]
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

### -States
Collection of securityActionState to keep the history of an action.
To construct, see NOTES section for STATES properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityActionState[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Status
operationStatus

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

### -User
The user principal name of the signed-in user that submitted (POST) the action.
The user should be extracted from the auth token and not entered manually by the calling application.

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

### -VendorInformation
securityVendorInformation
To construct, see NOTES section for VENDORINFORMATION properties and create a hash table.

```yaml
Type: IMicrosoftGraphSecurityVendorInformation
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSecurityAction
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSecurityAction
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphSecurityAction>`: securityAction
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ActionReason <String>]`: Reason for invoking this action.
  - `[AppId <String>]`: The Application ID of the calling application that submitted (POST) the action.
The appId should be extracted from the auth token and not entered manually by the calling application.
  - `[AzureTenantId <String>]`: Azure tenant ID of the entity to determine which tenant the entity belongs to (multi-tenancy support).
The azureTenantId should be extracted from the auth token and not entered manually by the calling application.
  - `[ClientContext <String>]`: Unique client context string.
Can have a maximum of 256 characters.
  - `[CompletedDateTime <DateTime?>]`: Timestamp when the action was completed.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[CreatedDateTime <DateTime?>]`: Timestamp when the action is created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[ErrorInfo <IMicrosoftGraphResultInfo>]`: resultInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Code <Int32?>]`: The result code.
    - `[Message <String>]`: The message.
    - `[Subcode <Int32?>]`: The result sub-code.
  - `[LastActionDateTime <DateTime?>]`: Timestamp when this action was last updated.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[Name <String>]`: Action name.
  - `[Parameters <IMicrosoftGraphKeyValuePair- `[]`>]`: Collection of parameters (key-value pairs) necessary to invoke the action, for example, URL or fileHash to block.).
Required.
    - `[Name <String>]`: Name for this key-value pair
    - `[Value <String>]`: Value for this key-value pair
  - `[States <IMicrosoftGraphSecurityActionState- `[]`>]`: Collection of securityActionState to keep the history of an action.
    - `[AppId <String>]`: The Application ID of the calling application that submitted an update (PATCH) to the action.
The appId should be extracted from the auth token and not entered manually by the calling application.
    - `[Status <String>]`: operationStatus
    - `[UpdatedDateTime <DateTime?>]`: Timestamp when the actionState was updated.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[User <String>]`: The user principal name of the signed-in user that submitted an update (PATCH) to the action.
The user should be extracted from the auth token and not entered manually by the calling application.
  - `[Status <String>]`: operationStatus
  - `[User <String>]`: The user principal name of the signed-in user that submitted  (POST) the action.
The user should be extracted from the auth token and not entered manually by the calling application.
  - `[VendorInformation <IMicrosoftGraphSecurityVendorInformation>]`: securityVendorInformation
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Provider <String>]`: Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.
    - `[ProviderVersion <String>]`: Version of the provider or subprovider, if it exists, that generated the alert.
Required
    - `[SubProvider <String>]`: Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.
    - `[Vendor <String>]`: Name of the alert vendor (for example, Microsoft, Dell, FireEye).
Required

ERRORINFO `<IMicrosoftGraphResultInfo>`: resultInfo
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Code <Int32?>]`: The result code.
  - `[Message <String>]`: The message.
  - `[Subcode <Int32?>]`: The result sub-code.

PARAMETERS `<IMicrosoftGraphKeyValuePair- `[]`>`: Collection of parameters (key-value pairs) necessary to invoke the action, for example, URL or fileHash to block.).
Required.
  - `[Name <String>]`: Name for this key-value pair
  - `[Value <String>]`: Value for this key-value pair

STATES `<IMicrosoftGraphSecurityActionState- `[]`>`: Collection of securityActionState to keep the history of an action.
  - `[AppId <String>]`: The Application ID of the calling application that submitted an update (PATCH) to the action.
The appId should be extracted from the auth token and not entered manually by the calling application.
  - `[Status <String>]`: operationStatus
  - `[UpdatedDateTime <DateTime?>]`: Timestamp when the actionState was updated.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[User <String>]`: The user principal name of the signed-in user that submitted an update (PATCH) to the action.
The user should be extracted from the auth token and not entered manually by the calling application.

VENDORINFORMATION `<IMicrosoftGraphSecurityVendorInformation>`: securityVendorInformation
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Provider <String>]`: Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.
  - `[ProviderVersion <String>]`: Version of the provider or subprovider, if it exists, that generated the alert.
Required
  - `[SubProvider <String>]`: Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.
  - `[Vendor <String>]`: Name of the alert vendor (for example, Microsoft, Dell, FireEye).
Required

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/new-mgbetasecurityaction](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.security/new-mgbetasecurityaction)

[https://learn.microsoft.com/graph/api/securityactions-post?view=graph-rest-beta](https://learn.microsoft.com/graph/api/securityactions-post?view=graph-rest-beta)























