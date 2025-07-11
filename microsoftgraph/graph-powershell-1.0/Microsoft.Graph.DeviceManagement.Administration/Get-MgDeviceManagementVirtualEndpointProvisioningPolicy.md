---
external help file: Microsoft.Graph.DeviceManagement.Administration-help.xml
Module Name: Microsoft.Graph.DeviceManagement.Administration
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement.administration/get-mgdevicemanagementvirtualendpointprovisioningpolicy
schema: 2.0.0
ms.subservice: cloud-pc
ms.subservice: cloud-pc
---

# Get-MgDeviceManagementVirtualEndpointProvisioningPolicy

## SYNOPSIS
Read the properties and relationships of a cloudPcProvisioningPolicy object.

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaDeviceManagementVirtualEndpointProvisioningPolicy](/powershell/module/Microsoft.Graph.Beta.DeviceManagement.Administration/Get-MgBetaDeviceManagementVirtualEndpointProvisioningPolicy?view=graph-powershell-beta)

## SYNTAX

### List (Default)
```
Get-MgDeviceManagementVirtualEndpointProvisioningPolicy [-ExpandProperty <String[]>] [-Property <String[]>]
 [-Filter <String>] [-Search <String>] [-Skip <Int32>] [-Sort <String[]>] [-Top <Int32>]
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PageSize <Int32>] [-All]
 [-CountVariable <String>] [<CommonParameters>]
```

### Get
```
Get-MgDeviceManagementVirtualEndpointProvisioningPolicy -CloudPcProvisioningPolicyId <String>
 [-ExpandProperty <String[]>] [-Property <String[]>] [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgDeviceManagementVirtualEndpointProvisioningPolicy -InputObject <IDeviceManagementAdministrationIdentity>
 [-ExpandProperty <String[]>] [-Property <String[]>] [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [<CommonParameters>]
```

## DESCRIPTION
Read the properties and relationships of a cloudPcProvisioningPolicy object.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | CloudPC.Read.All, CloudPC.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | CloudPC.Read.All, CloudPC.ReadWrite.All,  |

## EXAMPLES
### Example 1: Get the properties of the specified provisioning policy

```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

Get-MgDeviceManagementVirtualEndpointProvisioningPolicy -CloudPcProvisioningPolicyId $cloudPcProvisioningPolicyId

```
This example will get the properties of the specified provisioning policy

### Example 2: Get the properties of the specified provisioning policy and expand on the assignments

```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

Get-MgDeviceManagementVirtualEndpointProvisioningPolicy -CloudPcProvisioningPolicyId $cloudPcProvisioningPolicyId -ExpandProperty "assignments"

```
This example will get the properties of the specified provisioning policy and expand on the assignments

### Example 3: Get the selected properties of the specified provisioning policy

```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

Get-MgDeviceManagementVirtualEndpointProvisioningPolicy -CloudPcProvisioningPolicyId $cloudPcProvisioningPolicyId -Property "id,description,displayName,domainJoinConfigurations,imageDisplayName,imageId,imageType,windowsSetting,cloudPcGroupDisplayName,gracePeriodInHours,localAdminEnabled,alternateResourceUrl"

```
This example will get the selected properties of the specified provisioning policy


## PARAMETERS

### -All
List all pages.

```yaml
Type: SwitchParameter
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -CloudPcProvisioningPolicyId
The unique identifier of cloudPcProvisioningPolicy

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

### -CountVariable
Specifies a count of the total number of items in a collection.
By default, this variable will be set in the global scope.

```yaml
Type: String
Parameter Sets: List
Aliases: CV

Required: False
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

### -Filter
Filter items by property values

```yaml
Type: String
Parameter Sets: List
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
Type: IDeviceManagementAdministrationIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PageSize
Sets the page size of results.

```yaml
Type: Int32
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
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

### -Search
Search items by search phrases

```yaml
Type: String
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Skip
Skip the first n items

```yaml
Type: Int32
Parameter Sets: List
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Sort
Order items by property values

```yaml
Type: String[]
Parameter Sets: List
Aliases: OrderBy

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Top
Show only the first n items

```yaml
Type: Int32
Parameter Sets: List
Aliases: Limit

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IDeviceManagementAdministrationIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphCloudPcProvisioningPolicy
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<IDeviceManagementAdministrationIdentity>`: Identity Parameter
  - `[AuditEventId <String>]`: The unique identifier of auditEvent
  - `[Category <String>]`: Usage: category='{category}'
  - `[CloudPcAuditEventId <String>]`: The unique identifier of cloudPcAuditEvent
  - `[CloudPcDeviceImageId <String>]`: The unique identifier of cloudPcDeviceImage
  - `[CloudPcGalleryImageId <String>]`: The unique identifier of cloudPcGalleryImage
  - `[CloudPcId <String>]`: The unique identifier of cloudPC
  - `[CloudPcOnPremisesConnectionId <String>]`: The unique identifier of cloudPcOnPremisesConnection
  - `[CloudPcProvisioningPolicyAssignmentId <String>]`: The unique identifier of cloudPcProvisioningPolicyAssignment
  - `[CloudPcProvisioningPolicyId <String>]`: The unique identifier of cloudPcProvisioningPolicy
  - `[CloudPcUserSettingAssignmentId <String>]`: The unique identifier of cloudPcUserSettingAssignment
  - `[CloudPcUserSettingId <String>]`: The unique identifier of cloudPcUserSetting
  - `[ComplianceManagementPartnerId <String>]`: The unique identifier of complianceManagementPartner
  - `[DeviceAndAppManagementRoleAssignmentId <String>]`: The unique identifier of deviceAndAppManagementRoleAssignment
  - `[DeviceManagementExchangeConnectorId <String>]`: The unique identifier of deviceManagementExchangeConnector
  - `[DeviceManagementPartnerId <String>]`: The unique identifier of deviceManagementPartner
  - `[IosUpdateDeviceStatusId <String>]`: The unique identifier of iosUpdateDeviceStatus
  - `[MobileThreatDefenseConnectorId <String>]`: The unique identifier of mobileThreatDefenseConnector
  - `[RemoteAssistancePartnerId <String>]`: The unique identifier of remoteAssistancePartner
  - `[ResourceOperationId <String>]`: The unique identifier of resourceOperation
  - `[RoleAssignmentId <String>]`: The unique identifier of roleAssignment
  - `[RoleDefinitionId <String>]`: The unique identifier of roleDefinition
  - `[TelecomExpenseManagementPartnerId <String>]`: The unique identifier of telecomExpenseManagementPartner
  - `[TermsAndConditionsAcceptanceStatusId <String>]`: The unique identifier of termsAndConditionsAcceptanceStatus
  - `[TermsAndConditionsAssignmentId <String>]`: The unique identifier of termsAndConditionsAssignment
  - `[TermsAndConditionsId <String>]`: The unique identifier of termsAndConditions
  - `[UserId <String>]`: The unique identifier of user
  - `[UserPrincipalName <String>]`: Alternate key of user

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement.administration/get-mgdevicemanagementvirtualendpointprovisioningpolicy](https://learn.microsoft.com/powershell/module/microsoft.graph.devicemanagement.administration/get-mgdevicemanagementvirtualendpointprovisioningpolicy)

[https://learn.microsoft.com/graph/api/cloudpcprovisioningpolicy-get?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/cloudpcprovisioningpolicy-get?view=graph-rest-1.0)

[https://learn.microsoft.com/graph/api/virtualendpoint-list-provisioningpolicies?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/virtualendpoint-list-provisioningpolicies?view=graph-rest-1.0)























