---
external help file: Microsoft.Graph.Identity.DirectoryManagement-help.xml
Module Name: Microsoft.Graph.Identity.DirectoryManagement
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.directorymanagement/new-mgdirectorysubscription
schema: 2.0.0
---

# New-MgDirectorySubscription

## SYNOPSIS
Create new navigation property to subscriptions for directory

> [!NOTE]
> To view the beta release of this cmdlet, view [New-MgBetaDirectorySubscription](/powershell/module/Microsoft.Graph.Beta.Identity.DirectoryManagement/New-MgBetaDirectorySubscription?view=graph-powershell-beta)

## SYNTAX

### CreateExpanded (Default)
```
New-MgDirectorySubscription [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-CommerceSubscriptionId <String>] [-CreatedDateTime <DateTime>] [-Id <String>] [-IsTrial]
 [-NextLifecycleDateTime <DateTime>] [-OwnerId <String>] [-OwnerTenantId <String>] [-OwnerType <String>]
 [-ServiceStatus <IMicrosoftGraphServicePlanInfo[]>] [-SkuId <String>] [-SkuPartNumber <String>]
 [-Status <String>] [-TotalLicenses <Int32>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgDirectorySubscription -BodyParameter <IMicrosoftGraphCompanySubscription>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to subscriptions for directory

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

### -BodyParameter
companySubscription
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphCompanySubscription
Parameter Sets: Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CommerceSubscriptionId
The ID of this subscription in the commerce system.
Alternate key.

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
The date and time when this subscription was created.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
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

### -IsTrial
Whether the subscription is a free trial or purchased.

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

### -NextLifecycleDateTime
The date and time when the subscription will move to the next state (as defined by the status property) if not renewed by the tenant.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
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

### -OwnerId
The object ID of the account admin.

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

### -OwnerTenantId
The unique identifier for the Microsoft partner tenant that created the subscription on a customer tenant.

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

### -OwnerType
Indicates the entity that ownerId belongs to, for example, 'User'.

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

### -ServiceStatus
The provisioning status of each service included in this subscription.
To construct, see NOTES section for SERVICESTATUS properties and create a hash table.

```yaml
Type: IMicrosoftGraphServicePlanInfo[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SkuId
The object ID of the SKU associated with this subscription.

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

### -SkuPartNumber
The SKU associated with this subscription.

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

### -Status
The status of this subscription.
Possible values are: Enabled, Deleted, Suspended, Warning, LockedOut.

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

### -TotalLicenses
The number of licenses included in this subscription.

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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphCompanySubscription
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphCompanySubscription
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphCompanySubscription>`: companySubscription
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[CommerceSubscriptionId <String>]`: The ID of this subscription in the commerce system.
Alternate key.
  - `[CreatedDateTime <DateTime?>]`: The date and time when this subscription was created.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[IsTrial <Boolean?>]`: Whether the subscription is a free trial or purchased.
  - `[NextLifecycleDateTime <DateTime?>]`: The date and time when the subscription will move to the next state (as defined by the status property) if not renewed by the tenant.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
  - `[OwnerId <String>]`: The object ID of the account admin.
  - `[OwnerTenantId <String>]`: The unique identifier for the Microsoft partner tenant that created the subscription on a customer tenant.
  - `[OwnerType <String>]`: Indicates the entity that ownerId belongs to, for example, 'User'.
  - `[ServiceStatus <IMicrosoftGraphServicePlanInfo- `[]`>]`: The provisioning status of each service included in this subscription.
    - `[AppliesTo <String>]`: The object the service plan can be assigned to.
The possible values are:User - service plan can be assigned to individual users.Company - service plan can be assigned to the entire tenant.
    - `[ProvisioningStatus <String>]`: The provisioning status of the service plan.
The possible values are:Success - Service is fully provisioned.Disabled - Service is disabled.Error - The service plan isn't provisioned and is in an error state.PendingInput - The service isn't provisioned and is awaiting service confirmation.PendingActivation - The service is provisioned but requires explicit activation by an administrator (for example, Intune_O365 service plan)PendingProvisioning - Microsoft has added a new service to the product SKU and it isn't activated in the tenant.
    - `[ServicePlanId <String>]`: The unique identifier of the service plan.
    - `[ServicePlanName <String>]`: The name of the service plan.
  - `[SkuId <String>]`: The object ID of the SKU associated with this subscription.
  - `[SkuPartNumber <String>]`: The SKU associated with this subscription.
  - `[Status <String>]`: The status of this subscription.
Possible values are: Enabled, Deleted, Suspended, Warning, LockedOut.
  - `[TotalLicenses <Int32?>]`: The number of licenses included in this subscription.

SERVICESTATUS `<IMicrosoftGraphServicePlanInfo- `[]`>`: The provisioning status of each service included in this subscription.
  - `[AppliesTo <String>]`: The object the service plan can be assigned to.
The possible values are:User - service plan can be assigned to individual users.Company - service plan can be assigned to the entire tenant.
  - `[ProvisioningStatus <String>]`: The provisioning status of the service plan.
The possible values are:Success - Service is fully provisioned.Disabled - Service is disabled.Error - The service plan isn't provisioned and is in an error state.PendingInput - The service isn't provisioned and is awaiting service confirmation.PendingActivation - The service is provisioned but requires explicit activation by an administrator (for example, Intune_O365 service plan)PendingProvisioning - Microsoft has added a new service to the product SKU and it isn't activated in the tenant.
  - `[ServicePlanId <String>]`: The unique identifier of the service plan.
  - `[ServicePlanName <String>]`: The name of the service plan.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.directorymanagement/new-mgdirectorysubscription](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.directorymanagement/new-mgdirectorysubscription)
























