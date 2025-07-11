---
external help file: Microsoft.Graph.Planner-help.xml
Module Name: Microsoft.Graph.Planner
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.planner/update-mgplanner
schema: 2.0.0
---

# Update-MgPlanner

## SYNOPSIS
Update planner

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaPlanner](/powershell/module/Microsoft.Graph.Beta.Planner/Update-MgBetaPlanner?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgPlanner [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Buckets <IMicrosoftGraphPlannerBucket[]>] [-Id <String>] [-Plans <IMicrosoftGraphPlannerPlan[]>]
 [-Tasks <IMicrosoftGraphPlannerTask[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgPlanner -BodyParameter <IMicrosoftGraphPlanner> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update planner

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
planner
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphPlanner
Parameter Sets: Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Buckets
Read-only.
Nullable.
Returns a collection of the specified buckets
To construct, see NOTES section for BUCKETS properties and create a hash table.

```yaml
Type: IMicrosoftGraphPlannerBucket[]
Parameter Sets: UpdateExpanded
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
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Plans
Read-only.
Nullable.
Returns a collection of the specified plans
To construct, see NOTES section for PLANS properties and create a hash table.

```yaml
Type: IMicrosoftGraphPlannerPlan[]
Parameter Sets: UpdateExpanded
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

### -Tasks
Read-only.
Nullable.
Returns a collection of the specified tasks
To construct, see NOTES section for TASKS properties and create a hash table.

```yaml
Type: IMicrosoftGraphPlannerTask[]
Parameter Sets: UpdateExpanded
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphPlanner
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphPlanner
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphPlanner>`: planner
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Buckets <IMicrosoftGraphPlannerBucket- `[]`>]`: Read-only.
Nullable.
Returns a collection of the specified buckets
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Name <String>]`: Name of the bucket.
    - `[OrderHint <String>]`: Hint used to order items of this type in a list view.
For details about the supported format, see Using order hints in Planner.
    - `[PlanId <String>]`: Plan ID to which the bucket belongs.
    - `[Tasks <IMicrosoftGraphPlannerTask- `[]`>]`: Read-only.
Nullable.
The collection of tasks in the bucket.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[ActiveChecklistItemCount <Int32?>]`: Number of checklist items with value set to false, representing incomplete items.
      - `[AppliedCategories <IMicrosoftGraphPlannerAppliedCategories>]`: plannerAppliedCategories
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[AssignedToTaskBoardFormat <IMicrosoftGraphPlannerAssignedToTaskBoardTaskFormat>]`: plannerAssignedToTaskBoardTaskFormat
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[OrderHintsByAssignee <IMicrosoftGraphPlannerOrderHintsByAssignee>]`: plannerOrderHintsByAssignee
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[UnassignedOrderHint <String>]`: Hint value used to order the task on the AssignedTo view of the Task Board when the task isn't assigned to anyone, or if the orderHintsByAssignee dictionary doesn't provide an order hint for the user the task is assigned to.
The format is defined as outlined here.
      - `[AssigneePriority <String>]`: Hint used to order items of this type in a list view.
The format is defined as outlined here.
      - `[Assignments <IMicrosoftGraphPlannerAssignments>]`: plannerAssignments
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[BucketId <String>]`: Bucket ID to which the task belongs.
The bucket needs to be in the plan that the task is in.
It's 28 characters long and case-sensitive.
Format validation is done on the service.
      - `[BucketTaskBoardFormat <IMicrosoftGraphPlannerBucketTaskBoardTaskFormat>]`: plannerBucketTaskBoardTaskFormat
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[OrderHint <String>]`: Hint used to order tasks in the bucket view of the task board.
For details about the supported format, see Using order hints in Planner.
      - `[ChecklistItemCount <Int32?>]`: Number of checklist items that are present on the task.
      - `[CompletedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Application <IMicrosoftGraphIdentity>]`: identity
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
          - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
        - `[Device <IMicrosoftGraphIdentity>]`: identity
        - `[User <IMicrosoftGraphIdentity>]`: identity
      - `[CompletedDateTime <DateTime?>]`: Read-only.
Date and time at which the 'percentComplete' of the task is set to '100'.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      - `[ConversationThreadId <String>]`: Thread ID of the conversation on the task.
This is the ID of the conversation thread object created in the group.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[CreatedDateTime <DateTime?>]`: Read-only.
Date and time at which the task is created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      - `[Details <IMicrosoftGraphPlannerTaskDetails>]`: plannerTaskDetails
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[Checklist <IMicrosoftGraphPlannerChecklistItems>]`: plannerChecklistItems
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Description <String>]`: Description of the task.
        - `[PreviewType <String>]`: plannerPreviewType
        - `[References <IMicrosoftGraphPlannerExternalReferences>]`: plannerExternalReferences
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DueDateTime <DateTime?>]`: Date and time at which the task is due.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      - `[HasDescription <Boolean?>]`: Read-only.
Value is true if the details object of the task has a nonempty description and false otherwise.
      - `[OrderHint <String>]`: Hint used to order items of this type in a list view.
The format is defined as outlined here.
      - `[PercentComplete <Int32?>]`: Percentage of task completion.
When set to 100, the task is considered completed.
      - `[PlanId <String>]`: Plan ID to which the task belongs.
      - `[PreviewType <String>]`: plannerPreviewType
      - `[Priority <Int32?>]`: Priority of the task.
The valid range of values is between 0 and 10, with the increasing value being lower priority (0 has the highest priority and 10 has the lowest priority).
Currently, Planner interprets values 0 and 1 as 'urgent', 2, 3 and 4 as 'important', 5, 6, and 7 as 'medium', and 8, 9, and 10 as 'low'.
Additionally, Planner sets the value 1 for 'urgent', 3 for 'important', 5 for 'medium', and 9 for 'low'.
      - `[ProgressTaskBoardFormat <IMicrosoftGraphPlannerProgressTaskBoardTaskFormat>]`: plannerProgressTaskBoardTaskFormat
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[OrderHint <String>]`: Hint value used to order the task on the progress view of the task board.
For details about the supported format, see Using order hints in Planner.
      - `[ReferenceCount <Int32?>]`: Number of external references that exist on the task.
      - `[StartDateTime <DateTime?>]`: Date and time at which the task starts.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      - `[Title <String>]`: Title of the task.
  - `[Plans <IMicrosoftGraphPlannerPlan- `[]`>]`: Read-only.
Nullable.
Returns a collection of the specified plans
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Buckets <IMicrosoftGraphPlannerBucket- `[]`>]`: Read-only.
Nullable.
Collection of buckets in the plan.
    - `[Container <IMicrosoftGraphPlannerPlanContainer>]`: plannerPlanContainer
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[ContainerId <String>]`: The identifier of the resource that contains the plan.
Optional.
      - `[Type <String>]`: plannerContainerType
      - `[Url <String>]`: The full canonical URL of the container.
Optional.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[CreatedDateTime <DateTime?>]`: Read-only.
Date and time at which the plan is created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[Details <IMicrosoftGraphPlannerPlanDetails>]`: plannerPlanDetails
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[CategoryDescriptions <IMicrosoftGraphPlannerCategoryDescriptions>]`: plannerCategoryDescriptions
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Category1 <String>]`: The label associated with Category 1
        - `[Category10 <String>]`: The label associated with Category 10
        - `[Category11 <String>]`: The label associated with Category 11
        - `[Category12 <String>]`: The label associated with Category 12
        - `[Category13 <String>]`: The label associated with Category 13
        - `[Category14 <String>]`: The label associated with Category 14
        - `[Category15 <String>]`: The label associated with Category 15
        - `[Category16 <String>]`: The label associated with Category 16
        - `[Category17 <String>]`: The label associated with Category 17
        - `[Category18 <String>]`: The label associated with Category 18
        - `[Category19 <String>]`: The label associated with Category 19
        - `[Category2 <String>]`: The label associated with Category 2
        - `[Category20 <String>]`: The label associated with Category 20
        - `[Category21 <String>]`: The label associated with Category 21
        - `[Category22 <String>]`: The label associated with Category 22
        - `[Category23 <String>]`: The label associated with Category 23
        - `[Category24 <String>]`: The label associated with Category 24
        - `[Category25 <String>]`: The label associated with Category 25
        - `[Category3 <String>]`: The label associated with Category 3
        - `[Category4 <String>]`: The label associated with Category 4
        - `[Category5 <String>]`: The label associated with Category 5
        - `[Category6 <String>]`: The label associated with Category 6
        - `[Category7 <String>]`: The label associated with Category 7
        - `[Category8 <String>]`: The label associated with Category 8
        - `[Category9 <String>]`: The label associated with Category 9
      - `[SharedWith <IMicrosoftGraphPlannerUserIds>]`: plannerUserIds
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Owner <String>]`: Use the container property instead.
ID of the group that owns the plan.
After it's set, this property can't be updated.
This property won't return a valid group ID if the container of the plan isn't a group.
    - `[Tasks <IMicrosoftGraphPlannerTask- `[]`>]`: Read-only.
Nullable.
Collection of tasks in the plan.
    - `[Title <String>]`: Required.
Title of the plan.
  - `[Tasks <IMicrosoftGraphPlannerTask- `[]`>]`: Read-only.
Nullable.
Returns a collection of the specified tasks

BUCKETS `<IMicrosoftGraphPlannerBucket- `[]`>`: Read-only.
Nullable.
Returns a collection of the specified buckets
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Name <String>]`: Name of the bucket.
  - `[OrderHint <String>]`: Hint used to order items of this type in a list view.
For details about the supported format, see Using order hints in Planner.
  - `[PlanId <String>]`: Plan ID to which the bucket belongs.
  - `[Tasks <IMicrosoftGraphPlannerTask- `[]`>]`: Read-only.
Nullable.
The collection of tasks in the bucket.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ActiveChecklistItemCount <Int32?>]`: Number of checklist items with value set to false, representing incomplete items.
    - `[AppliedCategories <IMicrosoftGraphPlannerAppliedCategories>]`: plannerAppliedCategories
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AssignedToTaskBoardFormat <IMicrosoftGraphPlannerAssignedToTaskBoardTaskFormat>]`: plannerAssignedToTaskBoardTaskFormat
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[OrderHintsByAssignee <IMicrosoftGraphPlannerOrderHintsByAssignee>]`: plannerOrderHintsByAssignee
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[UnassignedOrderHint <String>]`: Hint value used to order the task on the AssignedTo view of the Task Board when the task isn't assigned to anyone, or if the orderHintsByAssignee dictionary doesn't provide an order hint for the user the task is assigned to.
The format is defined as outlined here.
    - `[AssigneePriority <String>]`: Hint used to order items of this type in a list view.
The format is defined as outlined here.
    - `[Assignments <IMicrosoftGraphPlannerAssignments>]`: plannerAssignments
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[BucketId <String>]`: Bucket ID to which the task belongs.
The bucket needs to be in the plan that the task is in.
It's 28 characters long and case-sensitive.
Format validation is done on the service.
    - `[BucketTaskBoardFormat <IMicrosoftGraphPlannerBucketTaskBoardTaskFormat>]`: plannerBucketTaskBoardTaskFormat
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[OrderHint <String>]`: Hint used to order tasks in the bucket view of the task board.
For details about the supported format, see Using order hints in Planner.
    - `[ChecklistItemCount <Int32?>]`: Number of checklist items that are present on the task.
    - `[CompletedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Application <IMicrosoftGraphIdentity>]`: identity
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
        - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
      - `[Device <IMicrosoftGraphIdentity>]`: identity
      - `[User <IMicrosoftGraphIdentity>]`: identity
    - `[CompletedDateTime <DateTime?>]`: Read-only.
Date and time at which the 'percentComplete' of the task is set to '100'.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[ConversationThreadId <String>]`: Thread ID of the conversation on the task.
This is the ID of the conversation thread object created in the group.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[CreatedDateTime <DateTime?>]`: Read-only.
Date and time at which the task is created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[Details <IMicrosoftGraphPlannerTaskDetails>]`: plannerTaskDetails
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Checklist <IMicrosoftGraphPlannerChecklistItems>]`: plannerChecklistItems
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Description <String>]`: Description of the task.
      - `[PreviewType <String>]`: plannerPreviewType
      - `[References <IMicrosoftGraphPlannerExternalReferences>]`: plannerExternalReferences
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DueDateTime <DateTime?>]`: Date and time at which the task is due.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[HasDescription <Boolean?>]`: Read-only.
Value is true if the details object of the task has a nonempty description and false otherwise.
    - `[OrderHint <String>]`: Hint used to order items of this type in a list view.
The format is defined as outlined here.
    - `[PercentComplete <Int32?>]`: Percentage of task completion.
When set to 100, the task is considered completed.
    - `[PlanId <String>]`: Plan ID to which the task belongs.
    - `[PreviewType <String>]`: plannerPreviewType
    - `[Priority <Int32?>]`: Priority of the task.
The valid range of values is between 0 and 10, with the increasing value being lower priority (0 has the highest priority and 10 has the lowest priority).
Currently, Planner interprets values 0 and 1 as 'urgent', 2, 3 and 4 as 'important', 5, 6, and 7 as 'medium', and 8, 9, and 10 as 'low'.
Additionally, Planner sets the value 1 for 'urgent', 3 for 'important', 5 for 'medium', and 9 for 'low'.
    - `[ProgressTaskBoardFormat <IMicrosoftGraphPlannerProgressTaskBoardTaskFormat>]`: plannerProgressTaskBoardTaskFormat
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[OrderHint <String>]`: Hint value used to order the task on the progress view of the task board.
For details about the supported format, see Using order hints in Planner.
    - `[ReferenceCount <Int32?>]`: Number of external references that exist on the task.
    - `[StartDateTime <DateTime?>]`: Date and time at which the task starts.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[Title <String>]`: Title of the task.

PLANS `<IMicrosoftGraphPlannerPlan- `[]`>`: Read-only.
Nullable.
Returns a collection of the specified plans
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Buckets <IMicrosoftGraphPlannerBucket- `[]`>]`: Read-only.
Nullable.
Collection of buckets in the plan.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Name <String>]`: Name of the bucket.
    - `[OrderHint <String>]`: Hint used to order items of this type in a list view.
For details about the supported format, see Using order hints in Planner.
    - `[PlanId <String>]`: Plan ID to which the bucket belongs.
    - `[Tasks <IMicrosoftGraphPlannerTask- `[]`>]`: Read-only.
Nullable.
The collection of tasks in the bucket.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[ActiveChecklistItemCount <Int32?>]`: Number of checklist items with value set to false, representing incomplete items.
      - `[AppliedCategories <IMicrosoftGraphPlannerAppliedCategories>]`: plannerAppliedCategories
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[AssignedToTaskBoardFormat <IMicrosoftGraphPlannerAssignedToTaskBoardTaskFormat>]`: plannerAssignedToTaskBoardTaskFormat
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[OrderHintsByAssignee <IMicrosoftGraphPlannerOrderHintsByAssignee>]`: plannerOrderHintsByAssignee
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[UnassignedOrderHint <String>]`: Hint value used to order the task on the AssignedTo view of the Task Board when the task isn't assigned to anyone, or if the orderHintsByAssignee dictionary doesn't provide an order hint for the user the task is assigned to.
The format is defined as outlined here.
      - `[AssigneePriority <String>]`: Hint used to order items of this type in a list view.
The format is defined as outlined here.
      - `[Assignments <IMicrosoftGraphPlannerAssignments>]`: plannerAssignments
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[BucketId <String>]`: Bucket ID to which the task belongs.
The bucket needs to be in the plan that the task is in.
It's 28 characters long and case-sensitive.
Format validation is done on the service.
      - `[BucketTaskBoardFormat <IMicrosoftGraphPlannerBucketTaskBoardTaskFormat>]`: plannerBucketTaskBoardTaskFormat
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[OrderHint <String>]`: Hint used to order tasks in the bucket view of the task board.
For details about the supported format, see Using order hints in Planner.
      - `[ChecklistItemCount <Int32?>]`: Number of checklist items that are present on the task.
      - `[CompletedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Application <IMicrosoftGraphIdentity>]`: identity
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
          - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
        - `[Device <IMicrosoftGraphIdentity>]`: identity
        - `[User <IMicrosoftGraphIdentity>]`: identity
      - `[CompletedDateTime <DateTime?>]`: Read-only.
Date and time at which the 'percentComplete' of the task is set to '100'.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      - `[ConversationThreadId <String>]`: Thread ID of the conversation on the task.
This is the ID of the conversation thread object created in the group.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[CreatedDateTime <DateTime?>]`: Read-only.
Date and time at which the task is created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      - `[Details <IMicrosoftGraphPlannerTaskDetails>]`: plannerTaskDetails
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[Checklist <IMicrosoftGraphPlannerChecklistItems>]`: plannerChecklistItems
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Description <String>]`: Description of the task.
        - `[PreviewType <String>]`: plannerPreviewType
        - `[References <IMicrosoftGraphPlannerExternalReferences>]`: plannerExternalReferences
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DueDateTime <DateTime?>]`: Date and time at which the task is due.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      - `[HasDescription <Boolean?>]`: Read-only.
Value is true if the details object of the task has a nonempty description and false otherwise.
      - `[OrderHint <String>]`: Hint used to order items of this type in a list view.
The format is defined as outlined here.
      - `[PercentComplete <Int32?>]`: Percentage of task completion.
When set to 100, the task is considered completed.
      - `[PlanId <String>]`: Plan ID to which the task belongs.
      - `[PreviewType <String>]`: plannerPreviewType
      - `[Priority <Int32?>]`: Priority of the task.
The valid range of values is between 0 and 10, with the increasing value being lower priority (0 has the highest priority and 10 has the lowest priority).
Currently, Planner interprets values 0 and 1 as 'urgent', 2, 3 and 4 as 'important', 5, 6, and 7 as 'medium', and 8, 9, and 10 as 'low'.
Additionally, Planner sets the value 1 for 'urgent', 3 for 'important', 5 for 'medium', and 9 for 'low'.
      - `[ProgressTaskBoardFormat <IMicrosoftGraphPlannerProgressTaskBoardTaskFormat>]`: plannerProgressTaskBoardTaskFormat
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[OrderHint <String>]`: Hint value used to order the task on the progress view of the task board.
For details about the supported format, see Using order hints in Planner.
      - `[ReferenceCount <Int32?>]`: Number of external references that exist on the task.
      - `[StartDateTime <DateTime?>]`: Date and time at which the task starts.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      - `[Title <String>]`: Title of the task.
  - `[Container <IMicrosoftGraphPlannerPlanContainer>]`: plannerPlanContainer
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ContainerId <String>]`: The identifier of the resource that contains the plan.
Optional.
    - `[Type <String>]`: plannerContainerType
    - `[Url <String>]`: The full canonical URL of the container.
Optional.
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[CreatedDateTime <DateTime?>]`: Read-only.
Date and time at which the plan is created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[Details <IMicrosoftGraphPlannerPlanDetails>]`: plannerPlanDetails
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[CategoryDescriptions <IMicrosoftGraphPlannerCategoryDescriptions>]`: plannerCategoryDescriptions
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Category1 <String>]`: The label associated with Category 1
      - `[Category10 <String>]`: The label associated with Category 10
      - `[Category11 <String>]`: The label associated with Category 11
      - `[Category12 <String>]`: The label associated with Category 12
      - `[Category13 <String>]`: The label associated with Category 13
      - `[Category14 <String>]`: The label associated with Category 14
      - `[Category15 <String>]`: The label associated with Category 15
      - `[Category16 <String>]`: The label associated with Category 16
      - `[Category17 <String>]`: The label associated with Category 17
      - `[Category18 <String>]`: The label associated with Category 18
      - `[Category19 <String>]`: The label associated with Category 19
      - `[Category2 <String>]`: The label associated with Category 2
      - `[Category20 <String>]`: The label associated with Category 20
      - `[Category21 <String>]`: The label associated with Category 21
      - `[Category22 <String>]`: The label associated with Category 22
      - `[Category23 <String>]`: The label associated with Category 23
      - `[Category24 <String>]`: The label associated with Category 24
      - `[Category25 <String>]`: The label associated with Category 25
      - `[Category3 <String>]`: The label associated with Category 3
      - `[Category4 <String>]`: The label associated with Category 4
      - `[Category5 <String>]`: The label associated with Category 5
      - `[Category6 <String>]`: The label associated with Category 6
      - `[Category7 <String>]`: The label associated with Category 7
      - `[Category8 <String>]`: The label associated with Category 8
      - `[Category9 <String>]`: The label associated with Category 9
    - `[SharedWith <IMicrosoftGraphPlannerUserIds>]`: plannerUserIds
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Owner <String>]`: Use the container property instead.
ID of the group that owns the plan.
After it's set, this property can't be updated.
This property won't return a valid group ID if the container of the plan isn't a group.
  - `[Tasks <IMicrosoftGraphPlannerTask- `[]`>]`: Read-only.
Nullable.
Collection of tasks in the plan.
  - `[Title <String>]`: Required.
Title of the plan.

TASKS `<IMicrosoftGraphPlannerTask- `[]`>`: Read-only.
Nullable.
Returns a collection of the specified tasks
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ActiveChecklistItemCount <Int32?>]`: Number of checklist items with value set to false, representing incomplete items.
  - `[AppliedCategories <IMicrosoftGraphPlannerAppliedCategories>]`: plannerAppliedCategories
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[AssignedToTaskBoardFormat <IMicrosoftGraphPlannerAssignedToTaskBoardTaskFormat>]`: plannerAssignedToTaskBoardTaskFormat
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[OrderHintsByAssignee <IMicrosoftGraphPlannerOrderHintsByAssignee>]`: plannerOrderHintsByAssignee
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[UnassignedOrderHint <String>]`: Hint value used to order the task on the AssignedTo view of the Task Board when the task isn't assigned to anyone, or if the orderHintsByAssignee dictionary doesn't provide an order hint for the user the task is assigned to.
The format is defined as outlined here.
  - `[AssigneePriority <String>]`: Hint used to order items of this type in a list view.
The format is defined as outlined here.
  - `[Assignments <IMicrosoftGraphPlannerAssignments>]`: plannerAssignments
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[BucketId <String>]`: Bucket ID to which the task belongs.
The bucket needs to be in the plan that the task is in.
It's 28 characters long and case-sensitive.
Format validation is done on the service.
  - `[BucketTaskBoardFormat <IMicrosoftGraphPlannerBucketTaskBoardTaskFormat>]`: plannerBucketTaskBoardTaskFormat
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[OrderHint <String>]`: Hint used to order tasks in the bucket view of the task board.
For details about the supported format, see Using order hints in Planner.
  - `[ChecklistItemCount <Int32?>]`: Number of checklist items that are present on the task.
  - `[CompletedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[CompletedDateTime <DateTime?>]`: Read-only.
Date and time at which the 'percentComplete' of the task is set to '100'.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[ConversationThreadId <String>]`: Thread ID of the conversation on the task.
This is the ID of the conversation thread object created in the group.
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[CreatedDateTime <DateTime?>]`: Read-only.
Date and time at which the task is created.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[Details <IMicrosoftGraphPlannerTaskDetails>]`: plannerTaskDetails
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Checklist <IMicrosoftGraphPlannerChecklistItems>]`: plannerChecklistItems
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Description <String>]`: Description of the task.
    - `[PreviewType <String>]`: plannerPreviewType
    - `[References <IMicrosoftGraphPlannerExternalReferences>]`: plannerExternalReferences
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DueDateTime <DateTime?>]`: Date and time at which the task is due.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[HasDescription <Boolean?>]`: Read-only.
Value is true if the details object of the task has a nonempty description and false otherwise.
  - `[OrderHint <String>]`: Hint used to order items of this type in a list view.
The format is defined as outlined here.
  - `[PercentComplete <Int32?>]`: Percentage of task completion.
When set to 100, the task is considered completed.
  - `[PlanId <String>]`: Plan ID to which the task belongs.
  - `[PreviewType <String>]`: plannerPreviewType
  - `[Priority <Int32?>]`: Priority of the task.
The valid range of values is between 0 and 10, with the increasing value being lower priority (0 has the highest priority and 10 has the lowest priority).
Currently, Planner interprets values 0 and 1 as 'urgent', 2, 3 and 4 as 'important', 5, 6, and 7 as 'medium', and 8, 9, and 10 as 'low'.
Additionally, Planner sets the value 1 for 'urgent', 3 for 'important', 5 for 'medium', and 9 for 'low'.
  - `[ProgressTaskBoardFormat <IMicrosoftGraphPlannerProgressTaskBoardTaskFormat>]`: plannerProgressTaskBoardTaskFormat
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[OrderHint <String>]`: Hint value used to order the task on the progress view of the task board.
For details about the supported format, see Using order hints in Planner.
  - `[ReferenceCount <Int32?>]`: Number of external references that exist on the task.
  - `[StartDateTime <DateTime?>]`: Date and time at which the task starts.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[Title <String>]`: Title of the task.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.planner/update-mgplanner](https://learn.microsoft.com/powershell/module/microsoft.graph.planner/update-mgplanner)
























