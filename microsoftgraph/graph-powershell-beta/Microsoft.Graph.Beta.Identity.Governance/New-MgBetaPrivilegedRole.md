---
external help file: Microsoft.Graph.Beta.Identity.Governance-help.xml
Module Name: Microsoft.Graph.Beta.Identity.Governance
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/new-mgbetaprivilegedrole
schema: 2.0.0
---

# New-MgBetaPrivilegedRole

## SYNOPSIS
Add new entity to privilegedRoles

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaPrivilegedRole [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Assignments <IMicrosoftGraphPrivilegedRoleAssignment[]>] [-Id <String>] [-Name <String>]
 [-Settings <IMicrosoftGraphPrivilegedRoleSettings>] [-Summary <IMicrosoftGraphPrivilegedRoleSummary>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaPrivilegedRole -BodyParameter <IMicrosoftGraphPrivilegedRole> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Add new entity to privilegedRoles

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

### -Assignments

To construct, see NOTES section for ASSIGNMENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphPrivilegedRoleAssignment[]
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
privilegedRole
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphPrivilegedRole
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

### -Name


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

### -Settings
privilegedRoleSettings
To construct, see NOTES section for SETTINGS properties and create a hash table.

```yaml
Type: IMicrosoftGraphPrivilegedRoleSettings
Parameter Sets: CreateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Summary
privilegedRoleSummary
To construct, see NOTES section for SUMMARY properties and create a hash table.

```yaml
Type: IMicrosoftGraphPrivilegedRoleSummary
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphPrivilegedRole
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphPrivilegedRole
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ASSIGNMENTS `<IMicrosoftGraphPrivilegedRoleAssignment- `[]`>`: .
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ExpirationDateTime <DateTime?>]`: 
  - `[IsElevated <Boolean?>]`: 
  - `[ResultMessage <String>]`: 
  - `[RoleId <String>]`: 
  - `[RoleInfo <IMicrosoftGraphPrivilegedRole>]`: privilegedRole
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Assignments <IMicrosoftGraphPrivilegedRoleAssignment- `[]`>]`: 
    - `[Name <String>]`: 
    - `[Settings <IMicrosoftGraphPrivilegedRoleSettings>]`: privilegedRoleSettings
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[ApprovalOnElevation <Boolean?>]`: 
      - `[ApproverIds <String- `[]`>]`: 
      - `[ElevationDuration <TimeSpan?>]`: 
      - `[IsMfaOnElevationConfigurable <Boolean?>]`: 
      - `[LastGlobalAdmin <Boolean?>]`: 
      - `[MaxElavationDuration <TimeSpan?>]`: 
      - `[MfaOnElevation <Boolean?>]`: 
      - `[MinElevationDuration <TimeSpan?>]`: 
      - `[NotificationToUserOnElevation <Boolean?>]`: 
      - `[TicketingInfoOnElevation <Boolean?>]`: 
    - `[Summary <IMicrosoftGraphPrivilegedRoleSummary>]`: privilegedRoleSummary
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[ElevatedCount <Int32?>]`: 
      - `[ManagedCount <Int32?>]`: 
      - `[MfaEnabled <Boolean?>]`: 
      - `[Status <String>]`: roleSummaryStatus
      - `[UsersCount <Int32?>]`: 
  - `[UserId <String>]`: 

BODYPARAMETER `<IMicrosoftGraphPrivilegedRole>`: privilegedRole
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Assignments <IMicrosoftGraphPrivilegedRoleAssignment- `[]`>]`: 
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ExpirationDateTime <DateTime?>]`: 
    - `[IsElevated <Boolean?>]`: 
    - `[ResultMessage <String>]`: 
    - `[RoleId <String>]`: 
    - `[RoleInfo <IMicrosoftGraphPrivilegedRole>]`: privilegedRole
    - `[UserId <String>]`: 
  - `[Name <String>]`: 
  - `[Settings <IMicrosoftGraphPrivilegedRoleSettings>]`: privilegedRoleSettings
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ApprovalOnElevation <Boolean?>]`: 
    - `[ApproverIds <String- `[]`>]`: 
    - `[ElevationDuration <TimeSpan?>]`: 
    - `[IsMfaOnElevationConfigurable <Boolean?>]`: 
    - `[LastGlobalAdmin <Boolean?>]`: 
    - `[MaxElavationDuration <TimeSpan?>]`: 
    - `[MfaOnElevation <Boolean?>]`: 
    - `[MinElevationDuration <TimeSpan?>]`: 
    - `[NotificationToUserOnElevation <Boolean?>]`: 
    - `[TicketingInfoOnElevation <Boolean?>]`: 
  - `[Summary <IMicrosoftGraphPrivilegedRoleSummary>]`: privilegedRoleSummary
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ElevatedCount <Int32?>]`: 
    - `[ManagedCount <Int32?>]`: 
    - `[MfaEnabled <Boolean?>]`: 
    - `[Status <String>]`: roleSummaryStatus
    - `[UsersCount <Int32?>]`: 

SETTINGS `<IMicrosoftGraphPrivilegedRoleSettings>`: privilegedRoleSettings
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ApprovalOnElevation <Boolean?>]`: 
  - `[ApproverIds <String- `[]`>]`: 
  - `[ElevationDuration <TimeSpan?>]`: 
  - `[IsMfaOnElevationConfigurable <Boolean?>]`: 
  - `[LastGlobalAdmin <Boolean?>]`: 
  - `[MaxElavationDuration <TimeSpan?>]`: 
  - `[MfaOnElevation <Boolean?>]`: 
  - `[MinElevationDuration <TimeSpan?>]`: 
  - `[NotificationToUserOnElevation <Boolean?>]`: 
  - `[TicketingInfoOnElevation <Boolean?>]`: 

SUMMARY `<IMicrosoftGraphPrivilegedRoleSummary>`: privilegedRoleSummary
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ElevatedCount <Int32?>]`: 
  - `[ManagedCount <Int32?>]`: 
  - `[MfaEnabled <Boolean?>]`: 
  - `[Status <String>]`: roleSummaryStatus
  - `[UsersCount <Int32?>]`:

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/new-mgbetaprivilegedrole](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/new-mgbetaprivilegedrole)
























