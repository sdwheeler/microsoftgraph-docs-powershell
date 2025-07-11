---
external help file: Microsoft.Graph.Beta.DeviceManagement-help.xml
Module Name: Microsoft.Graph.Beta.DeviceManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement/new-mgbetadevicemanagementmicrosofttunnelconfiguration
schema: 2.0.0
---

# New-MgBetaDeviceManagementMicrosoftTunnelConfiguration

## SYNOPSIS
Create new navigation property to microsoftTunnelConfigurations for deviceManagement

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaDeviceManagementMicrosoftTunnelConfiguration [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-AdvancedSettings <IMicrosoftGraphKeyValuePair[]>]
 [-DefaultDomainSuffix <String>] [-Description <String>] [-DisableUdpConnections] [-DisplayName <String>]
 [-DnsServers <String[]>] [-Id <String>] [-Ipv6Network <String>] [-LastUpdateDateTime <DateTime>]
 [-ListenPort <Int32>] [-Network <String>] [-RoleScopeTagIds <String[]>] [-RouteExcludes <String[]>]
 [-RouteIncludes <String[]>] [-RoutesExclude <String[]>] [-RoutesInclude <String[]>] [-SplitDns <String[]>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaDeviceManagementMicrosoftTunnelConfiguration
 -BodyParameter <IMicrosoftGraphMicrosoftTunnelConfiguration> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to microsoftTunnelConfigurations for deviceManagement

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | DeviceManagementConfiguration.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | DeviceManagementConfiguration.ReadWrite.All,  |

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

### -AdvancedSettings
Additional settings that may be applied to the server
To construct, see NOTES section for ADVANCEDSETTINGS properties and create a hash table.

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

### -BodyParameter
Entity that represents a collection of Microsoft Tunnel settings
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphMicrosoftTunnelConfiguration
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

### -DefaultDomainSuffix
The Default Domain appendix that will be used by the clients

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

### -Description
The configuration's description (optional)

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

### -DisableUdpConnections
When DisableUdpConnections is set, the clients and VPN server will not use DTLS connections to transfer data.

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
The display name for the server configuration.
This property is required when a server is created.

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

### -DnsServers
The DNS servers that will be used by the clients

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

### -Ipv6Network
The IPv6 subnet that will be used to allocate virtual address for the clients

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

### -LastUpdateDateTime
When the configuration was last updated

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

### -ListenPort
The port that both TCP and UPD will listen over on the server

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

### -Network
The IPv4 subnet that will be used to allocate virtual address for the clients

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
List of Scope Tags for this Entity instance

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

### -RouteExcludes
Subsets of the routes that will not be routed by the server

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

### -RouteIncludes
The routes that will be routed by the server

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

### -RoutesExclude
Subsets of the routes that will not be routed by the server.
This property is going to be deprecated with the option of using the new property, 'RouteExcludes'.

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

### -RoutesInclude
The routes that will be routed by the server.
This property is going to be deprecated with the option of using the new property, 'RouteIncludes'.

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

### -SplitDns
The domains that will be resolved using the provided dns servers

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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMicrosoftTunnelConfiguration
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphMicrosoftTunnelConfiguration
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ADVANCEDSETTINGS `<IMicrosoftGraphKeyValuePair- `[]`>`: Additional settings that may be applied to the server
  - `[Name <String>]`: Name for this key-value pair
  - `[Value <String>]`: Value for this key-value pair

BODYPARAMETER `<IMicrosoftGraphMicrosoftTunnelConfiguration>`: Entity that represents a collection of Microsoft Tunnel settings
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AdvancedSettings <IMicrosoftGraphKeyValuePair- `[]`>]`: Additional settings that may be applied to the server
    - `[Name <String>]`: Name for this key-value pair
    - `[Value <String>]`: Value for this key-value pair
  - `[DefaultDomainSuffix <String>]`: The Default Domain appendix that will be used by the clients
  - `[Description <String>]`: The configuration's description (optional)
  - `[DisableUdpConnections <Boolean?>]`: When DisableUdpConnections is set, the clients and VPN server will not use DTLS connections to transfer data.
  - `[DisplayName <String>]`: The display name for the server configuration.
This property is required when a server is created.
  - `[DnsServers <String- `[]`>]`: The DNS servers that will be used by the clients
  - `[Ipv6Network <String>]`: The IPv6 subnet that will be used to allocate virtual address for the clients
  - `[LastUpdateDateTime <DateTime?>]`: When the configuration was last updated
  - `[ListenPort <Int32?>]`: The port that both TCP and UPD will listen over on the server
  - `[Network <String>]`: The IPv4 subnet that will be used to allocate virtual address for the clients
  - `[RoleScopeTagIds <String- `[]`>]`: List of Scope Tags for this Entity instance
  - `[RouteExcludes <String- `[]`>]`: Subsets of the routes that will not be routed by the server
  - `[RouteIncludes <String- `[]`>]`: The routes that will be routed by the server
  - `[RoutesExclude <String- `[]`>]`: Subsets of the routes that will not be routed by the server.
This property is going to be deprecated with the option of using the new property, 'RouteExcludes'.
  - `[RoutesInclude <String- `[]`>]`: The routes that will be routed by the server.
This property is going to be deprecated with the option of using the new property, 'RouteIncludes'.
  - `[SplitDns <String- `[]`>]`: The domains that will be resolved using the provided dns servers

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement/new-mgbetadevicemanagementmicrosofttunnelconfiguration](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.devicemanagement/new-mgbetadevicemanagementmicrosofttunnelconfiguration)
























