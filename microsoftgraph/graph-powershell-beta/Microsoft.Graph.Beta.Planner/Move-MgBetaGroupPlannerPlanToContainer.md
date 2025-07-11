---
external help file: Microsoft.Graph.Beta.Planner-help.xml
Module Name: Microsoft.Graph.Beta.Planner
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.planner/move-mgbetagroupplannerplantocontainer
schema: 2.0.0
ms.subservice: planner
---

# Move-MgBetaGroupPlannerPlanToContainer

## SYNOPSIS
Move a planner plan object from one planner plan container to another.
Planner plans can only be moved from a user container to a group container.

## SYNTAX

### MoveExpanded (Default)
```
Move-MgBetaGroupPlannerPlanToContainer -GroupId <String> -PlannerPlanId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Container <IMicrosoftGraphPlannerPlanContainer>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Move
```
Move-MgBetaGroupPlannerPlanToContainer -GroupId <String> -PlannerPlanId <String>
 -BodyParameter <IPaths1N253R0GroupsGroupIdPlannerPlansPlannerplanIdMicrosoftGraphMovetocontainerPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### MoveViaIdentityExpanded
```
Move-MgBetaGroupPlannerPlanToContainer -InputObject <IPlannerIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-Container <IMicrosoftGraphPlannerPlanContainer>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### MoveViaIdentity
```
Move-MgBetaGroupPlannerPlanToContainer -InputObject <IPlannerIdentity>
 -BodyParameter <IPaths1N253R0GroupsGroupIdPlannerPlansPlannerplanIdMicrosoftGraphMovetocontainerPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Move a planner plan object from one planner plan container to another.
Planner plans can only be moved from a user container to a group container.

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: MoveExpanded, MoveViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter

To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPaths1N253R0GroupsGroupIdPlannerPlansPlannerplanIdMicrosoftGraphMovetocontainerPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Move, MoveViaIdentity
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

### -Container
plannerPlanContainer
To construct, see NOTES section for CONTAINER properties and create a hash table.

```yaml
Type: IMicrosoftGraphPlannerPlanContainer
Parameter Sets: MoveExpanded, MoveViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GroupId
The unique identifier of group

```yaml
Type: String
Parameter Sets: MoveExpanded, Move
Aliases:

Required: True
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
Type: IPlannerIdentity
Parameter Sets: MoveViaIdentityExpanded, MoveViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -PlannerPlanId
The unique identifier of plannerPlan

```yaml
Type: String
Parameter Sets: MoveExpanded, Move
Aliases:

Required: True
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

### Microsoft.Graph.Beta.PowerShell.Models.IPaths1N253R0GroupsGroupIdPlannerPlansPlannerplanIdMicrosoftGraphMovetocontainerPostRequestbodyContentApplicationJsonSchema
### Microsoft.Graph.Beta.PowerShell.Models.IPlannerIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphPlannerPlan
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPaths1N253R0GroupsGroupIdPlannerPlansPlannerplanIdMicrosoftGraphMovetocontainerPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Container <IMicrosoftGraphPlannerPlanContainer>]`: plannerPlanContainer
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ContainerId <String>]`: The identifier of the resource that contains the plan.
Optional.
    - `[Type <String>]`: plannerContainerType
    - `[Url <String>]`: The full canonical URL of the container.
Optional.

CONTAINER `<IMicrosoftGraphPlannerPlanContainer>`: plannerPlanContainer
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ContainerId <String>]`: The identifier of the resource that contains the plan.
Optional.
  - `[Type <String>]`: plannerContainerType
  - `[Url <String>]`: The full canonical URL of the container.
Optional.

INPUTOBJECT `<IPlannerIdentity>`: Identity Parameter
  - `[GroupId <String>]`: The unique identifier of group
  - `[PlannerBucketId <String>]`: The unique identifier of plannerBucket
  - `[PlannerDeltaId <String>]`: The unique identifier of plannerDelta
  - `[PlannerPlanId <String>]`: The unique identifier of plannerPlan
  - `[PlannerRosterId <String>]`: The unique identifier of plannerRoster
  - `[PlannerRosterMemberId <String>]`: The unique identifier of plannerRosterMember
  - `[PlannerTaskId <String>]`: The unique identifier of plannerTask
  - `[UserId <String>]`: The unique identifier of user

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.planner/move-mgbetagroupplannerplantocontainer](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.planner/move-mgbetagroupplannerplantocontainer)

[https://learn.microsoft.com/graph/api/plannerplan-movetocontainer?view=graph-rest-beta](https://learn.microsoft.com/graph/api/plannerplan-movetocontainer?view=graph-rest-beta)
























