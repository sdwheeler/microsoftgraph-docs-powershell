---
external help file: Microsoft.Graph.Beta.ManagedTenants-help.xml
Module Name: Microsoft.Graph.Beta.ManagedTenants
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.managedtenants/new-mgbetatenantrelationshipmanagedtenantcloudpcoverview
schema: 2.0.0
---

# New-MgBetaTenantRelationshipManagedTenantCloudPcOverview

## SYNOPSIS
Create new navigation property to cloudPcsOverview for tenantRelationships

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaTenantRelationshipManagedTenantCloudPcOverview [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-FrontlineLicensesCount <Int32>] [-Id <String>]
 [-LastRefreshedDateTime <DateTime>] [-NumberOfCloudPcConnectionStatusFailed <Int32>]
 [-NumberOfCloudPcConnectionStatusPassed <Int32>] [-NumberOfCloudPcConnectionStatusPending <Int32>]
 [-NumberOfCloudPcConnectionStatusRunning <Int32>] [-NumberOfCloudPcConnectionStatusUnkownFutureValue <Int32>]
 [-NumberOfCloudPcStatusDeprovisioning <Int32>] [-NumberOfCloudPcStatusFailed <Int32>]
 [-NumberOfCloudPcStatusInGracePeriod <Int32>] [-NumberOfCloudPcStatusNotProvisioned <Int32>]
 [-NumberOfCloudPcStatusProvisioned <Int32>] [-NumberOfCloudPcStatusProvisioning <Int32>]
 [-NumberOfCloudPcStatusUnknown <Int32>] [-NumberOfCloudPcStatusUpgrading <Int32>]
 [-TenantDisplayName <String>] [-TenantId <String>] [-TotalBusinessLicenses <Int32>]
 [-TotalCloudPcConnectionStatus <Int32>] [-TotalCloudPcStatus <Int32>] [-TotalEnterpriseLicenses <Int32>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaTenantRelationshipManagedTenantCloudPcOverview
 -BodyParameter <IMicrosoftGraphManagedTenantsCloudPcOverview> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to cloudPcsOverview for tenantRelationships

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
cloudPcOverview
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphManagedTenantsCloudPcOverview
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

### -FrontlineLicensesCount
The total number of cloud PC devices that have the Frontline SKU.
Optional.
Read-only.

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

### -LastRefreshedDateTime
Date and time the entity was last updated in the multi-tenant management platform.
Optional.
Read-only.

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

### -NumberOfCloudPcConnectionStatusFailed
The number of cloud PC connections that have a status of failed.
Optional.
Read-only.

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

### -NumberOfCloudPcConnectionStatusPassed
The number of cloud PC connections that have a status of passed.
Optional.
Read-only.

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

### -NumberOfCloudPcConnectionStatusPending
The number of cloud PC connections that have a status of pending.
Optional.
Read-only.

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

### -NumberOfCloudPcConnectionStatusRunning
The number of cloud PC connections that have a status of running.
Optional.
Read-only.

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

### -NumberOfCloudPcConnectionStatusUnkownFutureValue
The number of cloud PC connections that have a status of unknownFutureValue.
Optional.
Read-only.

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

### -NumberOfCloudPcStatusDeprovisioning
The number of cloud PCs that have a status of deprovisioning.
Optional.
Read-only.

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

### -NumberOfCloudPcStatusFailed
The number of cloud PCs that have a status of failed.
Optional.
Read-only.

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

### -NumberOfCloudPcStatusInGracePeriod
The number of cloud PCs that have a status of inGracePeriod.
Optional.
Read-only.

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

### -NumberOfCloudPcStatusNotProvisioned
The number of cloud PCs that have a status of notProvisioned.
Optional.
Read-only.

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

### -NumberOfCloudPcStatusProvisioned
The number of cloud PCs that have a status of provisioned.
Optional.
Read-only.

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

### -NumberOfCloudPcStatusProvisioning
The number of cloud PCs that have a status of provisioning.
Optional.
Read-only.

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

### -NumberOfCloudPcStatusUnknown
The number of cloud PCs that have a status of unknown.
Optional.
Read-only.

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

### -NumberOfCloudPcStatusUpgrading
The number of cloud PCs that have a status of upgrading.
Optional.
Read-only.

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

### -TenantDisplayName
The display name for the managed tenant.
Optional.
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

### -TenantId


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

### -TotalBusinessLicenses
The total number of cloud PC devices that have the Business SKU.
Optional.
Read-only.

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

### -TotalCloudPcConnectionStatus
The total number of cloud PC connection statuses for the given managed tenant.
Optional.
Read-only.

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

### -TotalCloudPcStatus
The total number of cloud PC statues for the given managed tenant.
Optional.
Read-only.

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

### -TotalEnterpriseLicenses
The total number of cloud PC devices that have the Enterprise SKU.
Optional.
Read-only.

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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphManagedTenantsCloudPcOverview
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphManagedTenantsCloudPcOverview
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphManagedTenantsCloudPcOverview>`: cloudPcOverview
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[FrontlineLicensesCount <Int32?>]`: The total number of cloud PC devices that have the Frontline SKU.
Optional.
Read-only.
  - `[LastRefreshedDateTime <DateTime?>]`: Date and time the entity was last updated in the multi-tenant management platform.
Optional.
Read-only.
  - `[NumberOfCloudPcConnectionStatusFailed <Int32?>]`: The number of cloud PC connections that have a status of failed.
Optional.
Read-only.
  - `[NumberOfCloudPcConnectionStatusPassed <Int32?>]`: The number of cloud PC connections that have a status of passed.
Optional.
Read-only.
  - `[NumberOfCloudPcConnectionStatusPending <Int32?>]`: The number of cloud PC connections that have a status of pending.
Optional.
Read-only.
  - `[NumberOfCloudPcConnectionStatusRunning <Int32?>]`: The number of cloud PC connections that have a status of running.
Optional.
Read-only.
  - `[NumberOfCloudPcConnectionStatusUnkownFutureValue <Int32?>]`: The number of cloud PC connections that have a status of unknownFutureValue.
Optional.
Read-only.
  - `[NumberOfCloudPcStatusDeprovisioning <Int32?>]`: The number of cloud PCs that have a status of deprovisioning.
Optional.
Read-only.
  - `[NumberOfCloudPcStatusFailed <Int32?>]`: The number of cloud PCs that have a status of failed.
Optional.
Read-only.
  - `[NumberOfCloudPcStatusInGracePeriod <Int32?>]`: The number of cloud PCs that have a status of inGracePeriod.
Optional.
Read-only.
  - `[NumberOfCloudPcStatusNotProvisioned <Int32?>]`: The number of cloud PCs that have a status of notProvisioned.
Optional.
Read-only.
  - `[NumberOfCloudPcStatusProvisioned <Int32?>]`: The number of cloud PCs that have a status of provisioned.
Optional.
Read-only.
  - `[NumberOfCloudPcStatusProvisioning <Int32?>]`: The number of cloud PCs that have a status of provisioning.
Optional.
Read-only.
  - `[NumberOfCloudPcStatusUnknown <Int32?>]`: The number of cloud PCs that have a status of unknown.
Optional.
Read-only.
  - `[NumberOfCloudPcStatusUpgrading <Int32?>]`: The number of cloud PCs that have a status of upgrading.
Optional.
Read-only.
  - `[TenantDisplayName <String>]`: The display name for the managed tenant.
Optional.
Read-only.
  - `[TenantId <String>]`: 
  - `[TotalBusinessLicenses <Int32?>]`: The total number of cloud PC devices that have the Business SKU.
Optional.
Read-only.
  - `[TotalCloudPcConnectionStatus <Int32?>]`: The total number of cloud PC connection statuses for the given managed tenant.
Optional.
Read-only.
  - `[TotalCloudPcStatus <Int32?>]`: The total number of cloud PC statues for the given managed tenant.
Optional.
Read-only.
  - `[TotalEnterpriseLicenses <Int32?>]`: The total number of cloud PC devices that have the Enterprise SKU.
Optional.
Read-only.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.managedtenants/new-mgbetatenantrelationshipmanagedtenantcloudpcoverview](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.managedtenants/new-mgbetatenantrelationshipmanagedtenantcloudpcoverview)
























