---
external help file: Microsoft.Graph.Identity.Partner-help.xml
Module Name: Microsoft.Graph.Identity.Partner
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.partner/get-mgtenantrelationshipdelegatedadminrelationshipaccessassignmentcount
schema: 2.0.0
---

# Get-MgTenantRelationshipDelegatedAdminRelationshipAccessAssignmentCount

## SYNOPSIS
Get the number of the resource

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaTenantRelationshipDelegatedAdminRelationshipAccessAssignmentCount](/powershell/module/Microsoft.Graph.Beta.Identity.Partner/Get-MgBetaTenantRelationshipDelegatedAdminRelationshipAccessAssignmentCount?view=graph-powershell-beta)

## SYNTAX

### Get (Default)
```
Get-MgTenantRelationshipDelegatedAdminRelationshipAccessAssignmentCount -DelegatedAdminRelationshipId <String>
 [-Filter <String>] [-Search <String>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgTenantRelationshipDelegatedAdminRelationshipAccessAssignmentCount -InputObject <IIdentityPartnerIdentity>
 [-Filter <String>] [-Search <String>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

## DESCRIPTION
Get the number of the resource

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | DelegatedAdminRelationship.Read.All, DelegatedAdminRelationship.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | DelegatedAdminRelationship.Read.All, DelegatedAdminRelationship.ReadWrite.All,  |

## EXAMPLES

## PARAMETERS

### -DelegatedAdminRelationshipId
The unique identifier of delegatedAdminRelationship

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

### -Filter
Filter items by property values

```yaml
Type: String
Parameter Sets: (All)
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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IIdentityPartnerIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
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

### -Search
Search items by search phrases

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IIdentityPartnerIdentity
### System.Collections.IDictionary
## OUTPUTS

### System.Int32
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<IIdentityPartnerIdentity>`: Identity Parameter
  - `[DelegatedAdminAccessAssignmentId <String>]`: The unique identifier of delegatedAdminAccessAssignment
  - `[DelegatedAdminCustomerId <String>]`: The unique identifier of delegatedAdminCustomer
  - `[DelegatedAdminRelationshipId <String>]`: The unique identifier of delegatedAdminRelationship
  - `[DelegatedAdminRelationshipOperationId <String>]`: The unique identifier of delegatedAdminRelationshipOperation
  - `[DelegatedAdminRelationshipRequestId <String>]`: The unique identifier of delegatedAdminRelationshipRequest
  - `[DelegatedAdminServiceManagementDetailId <String>]`: The unique identifier of delegatedAdminServiceManagementDetail

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.partner/get-mgtenantrelationshipdelegatedadminrelationshipaccessassignmentcount](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.partner/get-mgtenantrelationshipdelegatedadminrelationshipaccessassignmentcount)
























