---
external help file: Microsoft.Graph.Beta.Search-help.xml
Module Name: Microsoft.Graph.Beta.Search
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.search/get-mgbetaexternalauthorizationsystemdatacollectioninfo
schema: 2.0.0
---

# Get-MgBetaExternalAuthorizationSystemDataCollectionInfo

## SYNOPSIS
Defines how and whether Permissions Management collects data from the onboarded authorization system.
Supports $filter (eq) as follows:  $filter=dataCollectionInfo/entitlements/permissionsModificationCapability and $filter=dataCollectionInfo/entitlements/status.

## SYNTAX

### Get (Default)
```
Get-MgBetaExternalAuthorizationSystemDataCollectionInfo -AuthorizationSystemId <String>
 [-ExpandProperty <String[]>] [-Property <String[]>] [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgBetaExternalAuthorizationSystemDataCollectionInfo -InputObject <ISearchIdentity>
 [-ExpandProperty <String[]>] [-Property <String[]>] [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [<CommonParameters>]
```

## DESCRIPTION
Defines how and whether Permissions Management collects data from the onboarded authorization system.
Supports $filter (eq) as follows:  $filter=dataCollectionInfo/entitlements/permissionsModificationCapability and $filter=dataCollectionInfo/entitlements/status.

## EXAMPLES

## PARAMETERS

### -AuthorizationSystemId
The unique identifier of authorizationSystem

```yaml
Type: String
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: ISearchIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
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

### Microsoft.Graph.Beta.PowerShell.Models.ISearchIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphDataCollectionInfo
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<ISearchIdentity>`: Identity Parameter
  - `[AcronymId <String>]`: The unique identifier of acronym
  - `[AuthorizationSystemId <String>]`: The unique identifier of authorizationSystem
  - `[BookmarkId <String>]`: The unique identifier of bookmark
  - `[ConnectionOperationId <String>]`: The unique identifier of connectionOperation
  - `[ExternalActivityId <String>]`: The unique identifier of externalActivity
  - `[ExternalConnectionId <String>]`: The unique identifier of externalConnection
  - `[ExternalGroupId <String>]`: The unique identifier of externalGroup
  - `[ExternalItemId <String>]`: The unique identifier of externalItem
  - `[IdentityId <String>]`: The unique identifier of identity
  - `[InboundFlowId <String>]`: The unique identifier of inboundFlow
  - `[IndustryDataConnectorId <String>]`: The unique identifier of industryDataConnector
  - `[IndustryDataRunActivityId <String>]`: The unique identifier of industryDataRunActivity
  - `[IndustryDataRunId <String>]`: The unique identifier of industryDataRun
  - `[LongRunningOperationId <String>]`: The unique identifier of longRunningOperation
  - `[OutboundProvisioningFlowSetId <String>]`: The unique identifier of outboundProvisioningFlowSet
  - `[ProvisioningFlowId <String>]`: The unique identifier of provisioningFlow
  - `[QnaId <String>]`: The unique identifier of qna
  - `[ReferenceDefinitionId <String>]`: The unique identifier of referenceDefinition
  - `[RoleGroupId <String>]`: The unique identifier of roleGroup
  - `[SourceSystemDefinitionId <String>]`: The unique identifier of sourceSystemDefinition
  - `[YearTimePeriodDefinitionId <String>]`: The unique identifier of yearTimePeriodDefinition

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.search/get-mgbetaexternalauthorizationsystemdatacollectioninfo](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.search/get-mgbetaexternalauthorizationsystemdatacollectioninfo)
























