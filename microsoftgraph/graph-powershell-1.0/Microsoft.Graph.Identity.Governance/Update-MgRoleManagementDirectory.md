---
external help file: Microsoft.Graph.Identity.Governance-help.xml
Module Name: Microsoft.Graph.Identity.Governance
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/update-mgrolemanagementdirectory
schema: 2.0.0
---

# Update-MgRoleManagementDirectory

## SYNOPSIS
Update the navigation property directory in roleManagement

> [!NOTE]
> To view the beta release of this cmdlet, view [Update-MgBetaRoleManagementDirectory](/powershell/module/Microsoft.Graph.Beta.Identity.Governance/Update-MgBetaRoleManagementDirectory?view=graph-powershell-beta)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgRoleManagementDirectory [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>]
 [-Id <String>] [-ResourceNamespaces <IMicrosoftGraphUnifiedRbacResourceNamespace[]>]
 [-RoleAssignmentScheduleInstances <IMicrosoftGraphUnifiedRoleAssignmentScheduleInstance[]>]
 [-RoleAssignmentScheduleRequests <IMicrosoftGraphUnifiedRoleAssignmentScheduleRequest[]>]
 [-RoleAssignmentSchedules <IMicrosoftGraphUnifiedRoleAssignmentSchedule[]>]
 [-RoleAssignments <IMicrosoftGraphUnifiedRoleAssignment[]>]
 [-RoleDefinitions <IMicrosoftGraphUnifiedRoleDefinition[]>]
 [-RoleEligibilityScheduleInstances <IMicrosoftGraphUnifiedRoleEligibilityScheduleInstance[]>]
 [-RoleEligibilityScheduleRequests <IMicrosoftGraphUnifiedRoleEligibilityScheduleRequest[]>]
 [-RoleEligibilitySchedules <IMicrosoftGraphUnifiedRoleEligibilitySchedule[]>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgRoleManagementDirectory -BodyParameter <IMicrosoftGraphRbacApplication>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property directory in roleManagement

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
rbacApplication
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphRbacApplication
Parameter Sets: Update
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
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceNamespaces

To construct, see NOTES section for RESOURCENAMESPACES properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRbacResourceNamespace[]
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

### -RoleAssignments
Resource to grant access to users or groups.
To construct, see NOTES section for ROLEASSIGNMENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleAssignment[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RoleAssignmentScheduleInstances
Instances for active role assignments.
To construct, see NOTES section for ROLEASSIGNMENTSCHEDULEINSTANCES properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleAssignmentScheduleInstance[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RoleAssignmentScheduleRequests
Requests for active role assignments to principals through PIM.
To construct, see NOTES section for ROLEASSIGNMENTSCHEDULEREQUESTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleAssignmentScheduleRequest[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RoleAssignmentSchedules
Schedules for active role assignment operations.
To construct, see NOTES section for ROLEASSIGNMENTSCHEDULES properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleAssignmentSchedule[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RoleDefinitions
Resource representing the roles allowed by RBAC providers and the permissions assigned to the roles.
To construct, see NOTES section for ROLEDEFINITIONS properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleDefinition[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RoleEligibilityScheduleInstances
Instances for role eligibility requests.
To construct, see NOTES section for ROLEELIGIBILITYSCHEDULEINSTANCES properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleEligibilityScheduleInstance[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RoleEligibilityScheduleRequests
Requests for role eligibilities for principals through PIM.
To construct, see NOTES section for ROLEELIGIBILITYSCHEDULEREQUESTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleEligibilityScheduleRequest[]
Parameter Sets: UpdateExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RoleEligibilitySchedules
Schedules for role eligibility operations.
To construct, see NOTES section for ROLEELIGIBILITYSCHEDULES properties and create a hash table.

```yaml
Type: IMicrosoftGraphUnifiedRoleEligibilitySchedule[]
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

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphRbacApplication
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphRbacApplication
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphRbacApplication>`: rbacApplication
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ResourceNamespaces <IMicrosoftGraphUnifiedRbacResourceNamespace- `[]`>]`:
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Name <String>]`:
    - `[ResourceActions <IMicrosoftGraphUnifiedRbacResourceAction- `[]`>]`:
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[ActionVerb <String>]`:
      - `[AuthenticationContextId <String>]`:
      - `[Description <String>]`:
      - `[IsAuthenticationContextSettable <Boolean?>]`:
      - `[Name <String>]`:
      - `[ResourceScopeId <String>]`:
  - `[RoleAssignmentScheduleInstances <IMicrosoftGraphUnifiedRoleAssignmentScheduleInstance- `[]`>]`: Instances for active role assignments.
    - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[DisplayName <String>]`: Provides the display name of the app-specific resource represented by the app scope.
Provided for display purposes since appScopeId is often an immutable, non-human-readable id.
Read-only.
      - `[Type <String>]`: Describes the type of app-specific resource represented by the app scope and is provided for display purposes, so a user interface can convey to the user the kind of app specific resource represented by the app scope.
Read-only.
    - `[AppScopeId <String>]`: Identifier of the app-specific scope when the assignment or role eligibility is scoped to an app.
The scope of an assignment or role eligibility determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
    - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment or role eligibility.
The scope of an assignment or role eligibility determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
    - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[PrincipalId <String>]`: Identifier of the principal that has been granted the role assignment or that's eligible for a role.
    - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Description <String>]`: The description for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
      - `[DisplayName <String>]`: The display name for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
Required.
Supports $filter (eq, in).
      - `[InheritsPermissionsFrom <IMicrosoftGraphUnifiedRoleDefinition- `[]`>]`: Read-only collection of role definitions that the given role definition inherits from.
Only Microsoft Entra built-in roles (isBuiltIn is true) support this attribute.
Supports $expand.
      - `[IsBuiltIn <Boolean?>]`: Flag indicating whether the role definition is part of the default set included in Microsoft Entra or a custom definition.
Read-only.
Supports $filter (eq, in).
      - `[IsEnabled <Boolean?>]`: Flag indicating whether the role is enabled for assignment.
If false the role is not available for assignment.
Read-only when isBuiltIn is true.
      - `[ResourceScopes <String- `[]`>]`: List of the scopes or permissions the role definition applies to.
Currently only / is supported.
Read-only when isBuiltIn is true.
DO NOT USE.
This will be deprecated soon.
Attach scope to role assignment.
      - `[RolePermissions <IMicrosoftGraphUnifiedRolePermission- `[]`>]`: List of permissions included in the role.
Read-only when isBuiltIn is true.
Required.
        - `[AllowedResourceActions <String- `[]`>]`: Set of tasks that can be performed on a resource.
Required.
        - `[Condition <String>]`: Optional constraints that must be met for the permission to be effective.
Not supported for custom roles.
        - `[ExcludedResourceActions <String- `[]`>]`: Set of tasks that may not be performed on a resource.
Not yet supported.
      - `[TemplateId <String>]`: Custom template identifier that can be set when isBuiltIn is false but is read-only when isBuiltIn is true.
This identifier is typically used if one needs an identifier to be the same across different directories.
      - `[Version <String>]`: Indicates version of the role definition.
Read-only when isBuiltIn is true.
    - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal or that the principal is eligible for.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ActivatedUsing <IMicrosoftGraphUnifiedRoleEligibilityScheduleInstance>]`: unifiedRoleEligibilityScheduleInstance
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
      - `[AppScopeId <String>]`: Identifier of the app-specific scope when the assignment or role eligibility is scoped to an app.
The scope of an assignment or role eligibility determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
      - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
      - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment or role eligibility.
The scope of an assignment or role eligibility determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
      - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
      - `[PrincipalId <String>]`: Identifier of the principal that has been granted the role assignment or that's eligible for a role.
      - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
      - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal or that the principal is eligible for.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[EndDateTime <DateTime?>]`: The end date of the schedule instance.
      - `[MemberType <String>]`: How the role eligibility is inherited.
It can either be Inherited, Direct, or Group.
It can further imply whether the unifiedRoleEligibilitySchedule can be managed by the caller.
Supports $filter (eq, ne).
      - `[RoleEligibilityScheduleId <String>]`: The identifier of the unifiedRoleEligibilitySchedule object from which this instance was created.
Supports $filter (eq, ne).
      - `[StartDateTime <DateTime?>]`: When this instance starts.
    - `[AssignmentType <String>]`: The type of the assignment that can either be Assigned or Activated.
Supports $filter (eq, ne).
    - `[EndDateTime <DateTime?>]`: The end date of the schedule instance.
    - `[MemberType <String>]`: How the assignment is inherited.
It can either be Inherited, Direct, or Group.
It can further imply whether the unifiedRoleAssignmentSchedule can be managed by the caller.
Supports $filter (eq, ne).
    - `[RoleAssignmentOriginId <String>]`: The identifier of the role assignment in Microsoft Entra.
Supports $filter (eq, ne).
    - `[RoleAssignmentScheduleId <String>]`: The identifier of the unifiedRoleAssignmentSchedule object from which this instance was created.
Supports $filter (eq, ne).
    - `[StartDateTime <DateTime?>]`: When this instance starts.
  - `[RoleAssignmentScheduleRequests <IMicrosoftGraphUnifiedRoleAssignmentScheduleRequest- `[]`>]`: Requests for active role assignments to principals through PIM.
    - `[ApprovalId <String>]`: The identifier of the approval of the request.
    - `[CompletedDateTime <DateTime?>]`: The request completion date time.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Application <IMicrosoftGraphIdentity>]`: identity
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
        - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
      - `[Device <IMicrosoftGraphIdentity>]`: identity
      - `[User <IMicrosoftGraphIdentity>]`: identity
    - `[CreatedDateTime <DateTime?>]`: The request creation date time.
    - `[CustomData <String>]`: Free text field to define any custom data for the request.
Not used.
    - `[Status <String>]`: The status of the request.
Not nullable.
The possible values are: Canceled, Denied, Failed, Granted, PendingAdminDecision, PendingApproval, PendingProvisioning, PendingScheduleCreation, Provisioned, Revoked, and ScheduleCreated.
Not nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Action <String>]`: unifiedRoleScheduleRequestActions
    - `[ActivatedUsing <IMicrosoftGraphUnifiedRoleEligibilitySchedule>]`: unifiedRoleEligibilitySchedule
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
      - `[AppScopeId <String>]`: Identifier of the app-specific scope when the assignment or eligibility is scoped to an app.
The scope of an assignment or eligibility determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
      - `[CreatedDateTime <DateTime?>]`: When the schedule was created.
      - `[CreatedUsing <String>]`: Identifier of the object through which this schedule was created.
      - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
      - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment or eligibility.
The scope of an assignment or eligibility determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
      - `[ModifiedDateTime <DateTime?>]`: When the schedule was last modified.
      - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
      - `[PrincipalId <String>]`: Identifier of the principal that has been granted the role assignment or eligibility.
      - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
      - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal or that a principal is eligible for.
      - `[Status <String>]`: The status of the role assignment or eligibility request.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[MemberType <String>]`: How the role eligibility is inherited.
It can either be Inherited, Direct, or Group.
It can further imply whether the unifiedRoleEligibilitySchedule can be managed by the caller.
Supports $filter (eq, ne).
      - `[ScheduleInfo <IMicrosoftGraphRequestSchedule>]`: requestSchedule
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Expiration <IMicrosoftGraphExpirationPattern>]`: expirationPattern
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Duration <TimeSpan?>]`: The requestor's desired duration of access represented in ISO 8601 format for durations.
For example, PT3H refers to three hours.
If specified in a request, endDateTime should not be present and the type property should be set to afterDuration.
          - `[EndDateTime <DateTime?>]`: Timestamp of date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
          - `[Type <String>]`: expirationPatternType
        - `[Recurrence <IMicrosoftGraphPatternedRecurrence>]`: patternedRecurrence
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Pattern <IMicrosoftGraphRecurrencePattern>]`: recurrencePattern
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
            - `[DayOfMonth <Int32?>]`: The day of the month on which the event occurs.
Required if type is absoluteMonthly or absoluteYearly.
            - `[DaysOfWeek <String- `[]`>]`: A collection of the days of the week on which the event occurs.
The possible values are: sunday, monday, tuesday, wednesday, thursday, friday, saturday.
If type is relativeMonthly or relativeYearly, and daysOfWeek specifies more than one day, the event falls on the first day that satisfies the pattern.
Required if type is weekly, relativeMonthly, or relativeYearly.
            - `[FirstDayOfWeek <String>]`: dayOfWeek
            - `[Index <String>]`: weekIndex
            - `[Interval <Int32?>]`: The number of units between occurrences, where units can be in days, weeks, months, or years, depending on the type.
Required.
            - `[Month <Int32?>]`: The month in which the event occurs.
This is a number from 1 to 12.
            - `[Type <String>]`: recurrencePatternType
          - `[Range <IMicrosoftGraphRecurrenceRange>]`: recurrenceRange
            - `[(Any) <Object>]`: This indicates any property can be added to this object.
            - `[EndDate <DateTime?>]`: The date to stop applying the recurrence pattern.
Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.
Required if type is endDate.
            - `[NumberOfOccurrences <Int32?>]`: The number of times to repeat the event.
Required and must be positive if type is numbered.
            - `[RecurrenceTimeZone <String>]`: Time zone for the startDate and endDate properties.
Optional.
If not specified, the time zone of the event is used.
            - `[StartDate <DateTime?>]`: The date to start applying the recurrence pattern.
The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.
Must be the same value as the start property of the recurring event.
Required.
            - `[Type <String>]`: recurrenceRangeType
        - `[StartDateTime <DateTime?>]`: When the  eligible or active assignment becomes active.
    - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
    - `[AppScopeId <String>]`: Identifier of the app-specific scope when the assignment is scoped to an app.
The scope of an assignment determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
Supports $filter (eq, ne, and on null values).
    - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment.
The scope of an assignment determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
Supports $filter (eq, ne, and on null values).
    - `[IsValidationOnly <Boolean?>]`: Determines whether the call is a validation or an actual call.
Only set this property if you want to check whether an activation is subject to additional rules like MFA before actually submitting the request.
    - `[Justification <String>]`: A message provided by users and administrators when create they create the unifiedRoleAssignmentScheduleRequest object.
    - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[PrincipalId <String>]`: Identifier of the principal that has been granted the assignment.
Can be a user, role-assignable group, or a service principal.
Supports $filter (eq, ne).
    - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
    - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal.
Supports $filter (eq, ne).
    - `[ScheduleInfo <IMicrosoftGraphRequestSchedule>]`: requestSchedule
    - `[TargetSchedule <IMicrosoftGraphUnifiedRoleAssignmentSchedule>]`: unifiedRoleAssignmentSchedule
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
      - `[AppScopeId <String>]`: Identifier of the app-specific scope when the assignment or eligibility is scoped to an app.
The scope of an assignment or eligibility determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
      - `[CreatedDateTime <DateTime?>]`: When the schedule was created.
      - `[CreatedUsing <String>]`: Identifier of the object through which this schedule was created.
      - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
      - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment or eligibility.
The scope of an assignment or eligibility determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
      - `[ModifiedDateTime <DateTime?>]`: When the schedule was last modified.
      - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
      - `[PrincipalId <String>]`: Identifier of the principal that has been granted the role assignment or eligibility.
      - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
      - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal or that a principal is eligible for.
      - `[Status <String>]`: The status of the role assignment or eligibility request.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[ActivatedUsing <IMicrosoftGraphUnifiedRoleEligibilitySchedule>]`: unifiedRoleEligibilitySchedule
      - `[AssignmentType <String>]`: The type of the assignment that can either be Assigned or Activated.
Supports $filter (eq, ne).
      - `[MemberType <String>]`: How the assignment is inherited.
It can either be Inherited, Direct, or Group.
It can further imply whether the unifiedRoleAssignmentSchedule can be managed by the caller.
Supports $filter (eq, ne).
      - `[ScheduleInfo <IMicrosoftGraphRequestSchedule>]`: requestSchedule
    - `[TargetScheduleId <String>]`: Identifier of the schedule object that's linked to the assignment request.
Supports $filter (eq, ne).
    - `[TicketInfo <IMicrosoftGraphTicketInfo>]`: ticketInfo
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[TicketNumber <String>]`: The ticket number.
      - `[TicketSystem <String>]`: The description of the ticket system.
  - `[RoleAssignmentSchedules <IMicrosoftGraphUnifiedRoleAssignmentSchedule- `[]`>]`: Schedules for active role assignment operations.
  - `[RoleAssignments <IMicrosoftGraphUnifiedRoleAssignment- `[]`>]`: Resource to grant access to users or groups.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
    - `[AppScopeId <String>]`: Identifier of the app specific scope when the assignment scope is app specific.
The scope of an assignment determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by a resource application only.
For the entitlement management provider, use this property to specify a catalog.
For example, /AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997.
Supports $filter (eq, in).
For example, /roleManagement/entitlementManagement/roleAssignments?$filter=appScopeId eq '/AccessPackageCatalog/{catalog id}'.
    - `[Condition <String>]`:
    - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment.
The scope of an assignment determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications, unlike app scopes that are defined and understood by a resource application only.
Supports $filter (eq, in).
    - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[PrincipalId <String>]`: Identifier of the principal to which the assignment is granted.
Supported principals are users, role-assignable groups, and service principals.
Supports $filter (eq, in).
    - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
    - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition the assignment is for.
Read-only.
Supports $filter (eq, in).
  - `[RoleDefinitions <IMicrosoftGraphUnifiedRoleDefinition- `[]`>]`: Resource representing the roles allowed by RBAC providers and the permissions assigned to the roles.
  - `[RoleEligibilityScheduleInstances <IMicrosoftGraphUnifiedRoleEligibilityScheduleInstance- `[]`>]`: Instances for role eligibility requests.
  - `[RoleEligibilityScheduleRequests <IMicrosoftGraphUnifiedRoleEligibilityScheduleRequest- `[]`>]`: Requests for role eligibilities for principals through PIM.
    - `[ApprovalId <String>]`: The identifier of the approval of the request.
    - `[CompletedDateTime <DateTime?>]`: The request completion date time.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[CreatedDateTime <DateTime?>]`: The request creation date time.
    - `[CustomData <String>]`: Free text field to define any custom data for the request.
Not used.
    - `[Status <String>]`: The status of the request.
Not nullable.
The possible values are: Canceled, Denied, Failed, Granted, PendingAdminDecision, PendingApproval, PendingProvisioning, PendingScheduleCreation, Provisioned, Revoked, and ScheduleCreated.
Not nullable.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Action <String>]`: unifiedRoleScheduleRequestActions
    - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
    - `[AppScopeId <String>]`: Identifier of the app-specific scope when the role eligibility is scoped to an app.
The scope of a role eligibility determines the set of resources for which the principal is eligible to access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
Supports $filter (eq, ne, and on null values).
    - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the role eligibility.
The scope of a role eligibility determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
Supports $filter (eq, ne, and on null values).
    - `[IsValidationOnly <Boolean?>]`: Determines whether the call is a validation or an actual call.
Only set this property if you want to check whether an activation is subject to additional rules like MFA before actually submitting the request.
    - `[Justification <String>]`: A message provided by users and administrators when create they create the unifiedRoleEligibilityScheduleRequest object.
    - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[PrincipalId <String>]`: Identifier of the principal that has been granted the role eligibility.
Can be a user or a role-assignable group.
You can grant only active assignments service principals.Supports $filter (eq, ne).
    - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
    - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal.
Supports $filter (eq, ne).
    - `[ScheduleInfo <IMicrosoftGraphRequestSchedule>]`: requestSchedule
    - `[TargetSchedule <IMicrosoftGraphUnifiedRoleEligibilitySchedule>]`: unifiedRoleEligibilitySchedule
    - `[TargetScheduleId <String>]`: Identifier of the schedule object that's linked to the eligibility request.
Supports $filter (eq, ne).
    - `[TicketInfo <IMicrosoftGraphTicketInfo>]`: ticketInfo
  - `[RoleEligibilitySchedules <IMicrosoftGraphUnifiedRoleEligibilitySchedule- `[]`>]`: Schedules for role eligibility operations.

RESOURCENAMESPACES `<IMicrosoftGraphUnifiedRbacResourceNamespace- `[]`>`: .
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Name <String>]`:
  - `[ResourceActions <IMicrosoftGraphUnifiedRbacResourceAction- `[]`>]`:
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ActionVerb <String>]`:
    - `[AuthenticationContextId <String>]`:
    - `[Description <String>]`:
    - `[IsAuthenticationContextSettable <Boolean?>]`:
    - `[Name <String>]`:
    - `[ResourceScopeId <String>]`:

ROLEASSIGNMENTS `<IMicrosoftGraphUnifiedRoleAssignment- `[]`>`: Resource to grant access to users or groups.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: Provides the display name of the app-specific resource represented by the app scope.
Provided for display purposes since appScopeId is often an immutable, non-human-readable id.
Read-only.
    - `[Type <String>]`: Describes the type of app-specific resource represented by the app scope and is provided for display purposes, so a user interface can convey to the user the kind of app specific resource represented by the app scope.
Read-only.
  - `[AppScopeId <String>]`: Identifier of the app specific scope when the assignment scope is app specific.
The scope of an assignment determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by a resource application only.
For the entitlement management provider, use this property to specify a catalog.
For example, /AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997.
Supports $filter (eq, in).
For example, /roleManagement/entitlementManagement/roleAssignments?$filter=appScopeId eq '/AccessPackageCatalog/{catalog id}'.
  - `[Condition <String>]`:
  - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment.
The scope of an assignment determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications, unlike app scopes that are defined and understood by a resource application only.
Supports $filter (eq, in).
  - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
  - `[PrincipalId <String>]`: Identifier of the principal to which the assignment is granted.
Supported principals are users, role-assignable groups, and service principals.
Supports $filter (eq, in).
  - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Description <String>]`: The description for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
    - `[DisplayName <String>]`: The display name for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
Required.
Supports $filter (eq, in).
    - `[InheritsPermissionsFrom <IMicrosoftGraphUnifiedRoleDefinition- `[]`>]`: Read-only collection of role definitions that the given role definition inherits from.
Only Microsoft Entra built-in roles (isBuiltIn is true) support this attribute.
Supports $expand.
    - `[IsBuiltIn <Boolean?>]`: Flag indicating whether the role definition is part of the default set included in Microsoft Entra or a custom definition.
Read-only.
Supports $filter (eq, in).
    - `[IsEnabled <Boolean?>]`: Flag indicating whether the role is enabled for assignment.
If false the role is not available for assignment.
Read-only when isBuiltIn is true.
    - `[ResourceScopes <String- `[]`>]`: List of the scopes or permissions the role definition applies to.
Currently only / is supported.
Read-only when isBuiltIn is true.
DO NOT USE.
This will be deprecated soon.
Attach scope to role assignment.
    - `[RolePermissions <IMicrosoftGraphUnifiedRolePermission- `[]`>]`: List of permissions included in the role.
Read-only when isBuiltIn is true.
Required.
      - `[AllowedResourceActions <String- `[]`>]`: Set of tasks that can be performed on a resource.
Required.
      - `[Condition <String>]`: Optional constraints that must be met for the permission to be effective.
Not supported for custom roles.
      - `[ExcludedResourceActions <String- `[]`>]`: Set of tasks that may not be performed on a resource.
Not yet supported.
    - `[TemplateId <String>]`: Custom template identifier that can be set when isBuiltIn is false but is read-only when isBuiltIn is true.
This identifier is typically used if one needs an identifier to be the same across different directories.
    - `[Version <String>]`: Indicates version of the role definition.
Read-only when isBuiltIn is true.
  - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition the assignment is for.
Read-only.
Supports $filter (eq, in).

ROLEASSIGNMENTSCHEDULEINSTANCES `<IMicrosoftGraphUnifiedRoleAssignmentScheduleInstance- `[]`>`: Instances for active role assignments.
  - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: Provides the display name of the app-specific resource represented by the app scope.
Provided for display purposes since appScopeId is often an immutable, non-human-readable id.
Read-only.
    - `[Type <String>]`: Describes the type of app-specific resource represented by the app scope and is provided for display purposes, so a user interface can convey to the user the kind of app specific resource represented by the app scope.
Read-only.
  - `[AppScopeId <String>]`: Identifier of the app-specific scope when the assignment or role eligibility is scoped to an app.
The scope of an assignment or role eligibility determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
  - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment or role eligibility.
The scope of an assignment or role eligibility determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
  - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
  - `[PrincipalId <String>]`: Identifier of the principal that has been granted the role assignment or that's eligible for a role.
  - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Description <String>]`: The description for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
    - `[DisplayName <String>]`: The display name for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
Required.
Supports $filter (eq, in).
    - `[InheritsPermissionsFrom <IMicrosoftGraphUnifiedRoleDefinition- `[]`>]`: Read-only collection of role definitions that the given role definition inherits from.
Only Microsoft Entra built-in roles (isBuiltIn is true) support this attribute.
Supports $expand.
    - `[IsBuiltIn <Boolean?>]`: Flag indicating whether the role definition is part of the default set included in Microsoft Entra or a custom definition.
Read-only.
Supports $filter (eq, in).
    - `[IsEnabled <Boolean?>]`: Flag indicating whether the role is enabled for assignment.
If false the role is not available for assignment.
Read-only when isBuiltIn is true.
    - `[ResourceScopes <String- `[]`>]`: List of the scopes or permissions the role definition applies to.
Currently only / is supported.
Read-only when isBuiltIn is true.
DO NOT USE.
This will be deprecated soon.
Attach scope to role assignment.
    - `[RolePermissions <IMicrosoftGraphUnifiedRolePermission- `[]`>]`: List of permissions included in the role.
Read-only when isBuiltIn is true.
Required.
      - `[AllowedResourceActions <String- `[]`>]`: Set of tasks that can be performed on a resource.
Required.
      - `[Condition <String>]`: Optional constraints that must be met for the permission to be effective.
Not supported for custom roles.
      - `[ExcludedResourceActions <String- `[]`>]`: Set of tasks that may not be performed on a resource.
Not yet supported.
    - `[TemplateId <String>]`: Custom template identifier that can be set when isBuiltIn is false but is read-only when isBuiltIn is true.
This identifier is typically used if one needs an identifier to be the same across different directories.
    - `[Version <String>]`: Indicates version of the role definition.
Read-only when isBuiltIn is true.
  - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal or that the principal is eligible for.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ActivatedUsing <IMicrosoftGraphUnifiedRoleEligibilityScheduleInstance>]`: unifiedRoleEligibilityScheduleInstance
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
    - `[AppScopeId <String>]`: Identifier of the app-specific scope when the assignment or role eligibility is scoped to an app.
The scope of an assignment or role eligibility determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
    - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment or role eligibility.
The scope of an assignment or role eligibility determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
    - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[PrincipalId <String>]`: Identifier of the principal that has been granted the role assignment or that's eligible for a role.
    - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
    - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal or that the principal is eligible for.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[EndDateTime <DateTime?>]`: The end date of the schedule instance.
    - `[MemberType <String>]`: How the role eligibility is inherited.
It can either be Inherited, Direct, or Group.
It can further imply whether the unifiedRoleEligibilitySchedule can be managed by the caller.
Supports $filter (eq, ne).
    - `[RoleEligibilityScheduleId <String>]`: The identifier of the unifiedRoleEligibilitySchedule object from which this instance was created.
Supports $filter (eq, ne).
    - `[StartDateTime <DateTime?>]`: When this instance starts.
  - `[AssignmentType <String>]`: The type of the assignment that can either be Assigned or Activated.
Supports $filter (eq, ne).
  - `[EndDateTime <DateTime?>]`: The end date of the schedule instance.
  - `[MemberType <String>]`: How the assignment is inherited.
It can either be Inherited, Direct, or Group.
It can further imply whether the unifiedRoleAssignmentSchedule can be managed by the caller.
Supports $filter (eq, ne).
  - `[RoleAssignmentOriginId <String>]`: The identifier of the role assignment in Microsoft Entra.
Supports $filter (eq, ne).
  - `[RoleAssignmentScheduleId <String>]`: The identifier of the unifiedRoleAssignmentSchedule object from which this instance was created.
Supports $filter (eq, ne).
  - `[StartDateTime <DateTime?>]`: When this instance starts.

ROLEASSIGNMENTSCHEDULEREQUESTS `<IMicrosoftGraphUnifiedRoleAssignmentScheduleRequest- `[]`>`: Requests for active role assignments to principals through PIM.
  - `[ApprovalId <String>]`: The identifier of the approval of the request.
  - `[CompletedDateTime <DateTime?>]`: The request completion date time.
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[CreatedDateTime <DateTime?>]`: The request creation date time.
  - `[CustomData <String>]`: Free text field to define any custom data for the request.
Not used.
  - `[Status <String>]`: The status of the request.
Not nullable.
The possible values are: Canceled, Denied, Failed, Granted, PendingAdminDecision, PendingApproval, PendingProvisioning, PendingScheduleCreation, Provisioned, Revoked, and ScheduleCreated.
Not nullable.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Action <String>]`: unifiedRoleScheduleRequestActions
  - `[ActivatedUsing <IMicrosoftGraphUnifiedRoleEligibilitySchedule>]`: unifiedRoleEligibilitySchedule
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[DisplayName <String>]`: Provides the display name of the app-specific resource represented by the app scope.
Provided for display purposes since appScopeId is often an immutable, non-human-readable id.
Read-only.
      - `[Type <String>]`: Describes the type of app-specific resource represented by the app scope and is provided for display purposes, so a user interface can convey to the user the kind of app specific resource represented by the app scope.
Read-only.
    - `[AppScopeId <String>]`: Identifier of the app-specific scope when the assignment or eligibility is scoped to an app.
The scope of an assignment or eligibility determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
    - `[CreatedDateTime <DateTime?>]`: When the schedule was created.
    - `[CreatedUsing <String>]`: Identifier of the object through which this schedule was created.
    - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
    - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment or eligibility.
The scope of an assignment or eligibility determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
    - `[ModifiedDateTime <DateTime?>]`: When the schedule was last modified.
    - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[PrincipalId <String>]`: Identifier of the principal that has been granted the role assignment or eligibility.
    - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Description <String>]`: The description for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
      - `[DisplayName <String>]`: The display name for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
Required.
Supports $filter (eq, in).
      - `[InheritsPermissionsFrom <IMicrosoftGraphUnifiedRoleDefinition- `[]`>]`: Read-only collection of role definitions that the given role definition inherits from.
Only Microsoft Entra built-in roles (isBuiltIn is true) support this attribute.
Supports $expand.
      - `[IsBuiltIn <Boolean?>]`: Flag indicating whether the role definition is part of the default set included in Microsoft Entra or a custom definition.
Read-only.
Supports $filter (eq, in).
      - `[IsEnabled <Boolean?>]`: Flag indicating whether the role is enabled for assignment.
If false the role is not available for assignment.
Read-only when isBuiltIn is true.
      - `[ResourceScopes <String- `[]`>]`: List of the scopes or permissions the role definition applies to.
Currently only / is supported.
Read-only when isBuiltIn is true.
DO NOT USE.
This will be deprecated soon.
Attach scope to role assignment.
      - `[RolePermissions <IMicrosoftGraphUnifiedRolePermission- `[]`>]`: List of permissions included in the role.
Read-only when isBuiltIn is true.
Required.
        - `[AllowedResourceActions <String- `[]`>]`: Set of tasks that can be performed on a resource.
Required.
        - `[Condition <String>]`: Optional constraints that must be met for the permission to be effective.
Not supported for custom roles.
        - `[ExcludedResourceActions <String- `[]`>]`: Set of tasks that may not be performed on a resource.
Not yet supported.
      - `[TemplateId <String>]`: Custom template identifier that can be set when isBuiltIn is false but is read-only when isBuiltIn is true.
This identifier is typically used if one needs an identifier to be the same across different directories.
      - `[Version <String>]`: Indicates version of the role definition.
Read-only when isBuiltIn is true.
    - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal or that a principal is eligible for.
    - `[Status <String>]`: The status of the role assignment or eligibility request.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[MemberType <String>]`: How the role eligibility is inherited.
It can either be Inherited, Direct, or Group.
It can further imply whether the unifiedRoleEligibilitySchedule can be managed by the caller.
Supports $filter (eq, ne).
    - `[ScheduleInfo <IMicrosoftGraphRequestSchedule>]`: requestSchedule
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Expiration <IMicrosoftGraphExpirationPattern>]`: expirationPattern
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Duration <TimeSpan?>]`: The requestor's desired duration of access represented in ISO 8601 format for durations.
For example, PT3H refers to three hours.
If specified in a request, endDateTime should not be present and the type property should be set to afterDuration.
        - `[EndDateTime <DateTime?>]`: Timestamp of date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
        - `[Type <String>]`: expirationPatternType
      - `[Recurrence <IMicrosoftGraphPatternedRecurrence>]`: patternedRecurrence
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Pattern <IMicrosoftGraphRecurrencePattern>]`: recurrencePattern
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[DayOfMonth <Int32?>]`: The day of the month on which the event occurs.
Required if type is absoluteMonthly or absoluteYearly.
          - `[DaysOfWeek <String- `[]`>]`: A collection of the days of the week on which the event occurs.
The possible values are: sunday, monday, tuesday, wednesday, thursday, friday, saturday.
If type is relativeMonthly or relativeYearly, and daysOfWeek specifies more than one day, the event falls on the first day that satisfies the pattern.
Required if type is weekly, relativeMonthly, or relativeYearly.
          - `[FirstDayOfWeek <String>]`: dayOfWeek
          - `[Index <String>]`: weekIndex
          - `[Interval <Int32?>]`: The number of units between occurrences, where units can be in days, weeks, months, or years, depending on the type.
Required.
          - `[Month <Int32?>]`: The month in which the event occurs.
This is a number from 1 to 12.
          - `[Type <String>]`: recurrencePatternType
        - `[Range <IMicrosoftGraphRecurrenceRange>]`: recurrenceRange
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[EndDate <DateTime?>]`: The date to stop applying the recurrence pattern.
Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.
Required if type is endDate.
          - `[NumberOfOccurrences <Int32?>]`: The number of times to repeat the event.
Required and must be positive if type is numbered.
          - `[RecurrenceTimeZone <String>]`: Time zone for the startDate and endDate properties.
Optional.
If not specified, the time zone of the event is used.
          - `[StartDate <DateTime?>]`: The date to start applying the recurrence pattern.
The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.
Must be the same value as the start property of the recurring event.
Required.
          - `[Type <String>]`: recurrenceRangeType
      - `[StartDateTime <DateTime?>]`: When the  eligible or active assignment becomes active.
  - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
  - `[AppScopeId <String>]`: Identifier of the app-specific scope when the assignment is scoped to an app.
The scope of an assignment determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
Supports $filter (eq, ne, and on null values).
  - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
  - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment.
The scope of an assignment determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
Supports $filter (eq, ne, and on null values).
  - `[IsValidationOnly <Boolean?>]`: Determines whether the call is a validation or an actual call.
Only set this property if you want to check whether an activation is subject to additional rules like MFA before actually submitting the request.
  - `[Justification <String>]`: A message provided by users and administrators when create they create the unifiedRoleAssignmentScheduleRequest object.
  - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
  - `[PrincipalId <String>]`: Identifier of the principal that has been granted the assignment.
Can be a user, role-assignable group, or a service principal.
Supports $filter (eq, ne).
  - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
  - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal.
Supports $filter (eq, ne).
  - `[ScheduleInfo <IMicrosoftGraphRequestSchedule>]`: requestSchedule
  - `[TargetSchedule <IMicrosoftGraphUnifiedRoleAssignmentSchedule>]`: unifiedRoleAssignmentSchedule
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
    - `[AppScopeId <String>]`: Identifier of the app-specific scope when the assignment or eligibility is scoped to an app.
The scope of an assignment or eligibility determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
    - `[CreatedDateTime <DateTime?>]`: When the schedule was created.
    - `[CreatedUsing <String>]`: Identifier of the object through which this schedule was created.
    - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment or eligibility.
The scope of an assignment or eligibility determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
    - `[ModifiedDateTime <DateTime?>]`: When the schedule was last modified.
    - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[PrincipalId <String>]`: Identifier of the principal that has been granted the role assignment or eligibility.
    - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
    - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal or that a principal is eligible for.
    - `[Status <String>]`: The status of the role assignment or eligibility request.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ActivatedUsing <IMicrosoftGraphUnifiedRoleEligibilitySchedule>]`: unifiedRoleEligibilitySchedule
    - `[AssignmentType <String>]`: The type of the assignment that can either be Assigned or Activated.
Supports $filter (eq, ne).
    - `[MemberType <String>]`: How the assignment is inherited.
It can either be Inherited, Direct, or Group.
It can further imply whether the unifiedRoleAssignmentSchedule can be managed by the caller.
Supports $filter (eq, ne).
    - `[ScheduleInfo <IMicrosoftGraphRequestSchedule>]`: requestSchedule
  - `[TargetScheduleId <String>]`: Identifier of the schedule object that's linked to the assignment request.
Supports $filter (eq, ne).
  - `[TicketInfo <IMicrosoftGraphTicketInfo>]`: ticketInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[TicketNumber <String>]`: The ticket number.
    - `[TicketSystem <String>]`: The description of the ticket system.

ROLEASSIGNMENTSCHEDULES `<IMicrosoftGraphUnifiedRoleAssignmentSchedule- `[]`>`: Schedules for active role assignment operations.
  - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: Provides the display name of the app-specific resource represented by the app scope.
Provided for display purposes since appScopeId is often an immutable, non-human-readable id.
Read-only.
    - `[Type <String>]`: Describes the type of app-specific resource represented by the app scope and is provided for display purposes, so a user interface can convey to the user the kind of app specific resource represented by the app scope.
Read-only.
  - `[AppScopeId <String>]`: Identifier of the app-specific scope when the assignment or eligibility is scoped to an app.
The scope of an assignment or eligibility determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
  - `[CreatedDateTime <DateTime?>]`: When the schedule was created.
  - `[CreatedUsing <String>]`: Identifier of the object through which this schedule was created.
  - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment or eligibility.
The scope of an assignment or eligibility determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
  - `[ModifiedDateTime <DateTime?>]`: When the schedule was last modified.
  - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
  - `[PrincipalId <String>]`: Identifier of the principal that has been granted the role assignment or eligibility.
  - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Description <String>]`: The description for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
    - `[DisplayName <String>]`: The display name for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
Required.
Supports $filter (eq, in).
    - `[InheritsPermissionsFrom <IMicrosoftGraphUnifiedRoleDefinition- `[]`>]`: Read-only collection of role definitions that the given role definition inherits from.
Only Microsoft Entra built-in roles (isBuiltIn is true) support this attribute.
Supports $expand.
    - `[IsBuiltIn <Boolean?>]`: Flag indicating whether the role definition is part of the default set included in Microsoft Entra or a custom definition.
Read-only.
Supports $filter (eq, in).
    - `[IsEnabled <Boolean?>]`: Flag indicating whether the role is enabled for assignment.
If false the role is not available for assignment.
Read-only when isBuiltIn is true.
    - `[ResourceScopes <String- `[]`>]`: List of the scopes or permissions the role definition applies to.
Currently only / is supported.
Read-only when isBuiltIn is true.
DO NOT USE.
This will be deprecated soon.
Attach scope to role assignment.
    - `[RolePermissions <IMicrosoftGraphUnifiedRolePermission- `[]`>]`: List of permissions included in the role.
Read-only when isBuiltIn is true.
Required.
      - `[AllowedResourceActions <String- `[]`>]`: Set of tasks that can be performed on a resource.
Required.
      - `[Condition <String>]`: Optional constraints that must be met for the permission to be effective.
Not supported for custom roles.
      - `[ExcludedResourceActions <String- `[]`>]`: Set of tasks that may not be performed on a resource.
Not yet supported.
    - `[TemplateId <String>]`: Custom template identifier that can be set when isBuiltIn is false but is read-only when isBuiltIn is true.
This identifier is typically used if one needs an identifier to be the same across different directories.
    - `[Version <String>]`: Indicates version of the role definition.
Read-only when isBuiltIn is true.
  - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal or that a principal is eligible for.
  - `[Status <String>]`: The status of the role assignment or eligibility request.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ActivatedUsing <IMicrosoftGraphUnifiedRoleEligibilitySchedule>]`: unifiedRoleEligibilitySchedule
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
    - `[AppScopeId <String>]`: Identifier of the app-specific scope when the assignment or eligibility is scoped to an app.
The scope of an assignment or eligibility determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
    - `[CreatedDateTime <DateTime?>]`: When the schedule was created.
    - `[CreatedUsing <String>]`: Identifier of the object through which this schedule was created.
    - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment or eligibility.
The scope of an assignment or eligibility determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
    - `[ModifiedDateTime <DateTime?>]`: When the schedule was last modified.
    - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[PrincipalId <String>]`: Identifier of the principal that has been granted the role assignment or eligibility.
    - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
    - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal or that a principal is eligible for.
    - `[Status <String>]`: The status of the role assignment or eligibility request.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[MemberType <String>]`: How the role eligibility is inherited.
It can either be Inherited, Direct, or Group.
It can further imply whether the unifiedRoleEligibilitySchedule can be managed by the caller.
Supports $filter (eq, ne).
    - `[ScheduleInfo <IMicrosoftGraphRequestSchedule>]`: requestSchedule
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Expiration <IMicrosoftGraphExpirationPattern>]`: expirationPattern
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Duration <TimeSpan?>]`: The requestor's desired duration of access represented in ISO 8601 format for durations.
For example, PT3H refers to three hours.
If specified in a request, endDateTime should not be present and the type property should be set to afterDuration.
        - `[EndDateTime <DateTime?>]`: Timestamp of date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
        - `[Type <String>]`: expirationPatternType
      - `[Recurrence <IMicrosoftGraphPatternedRecurrence>]`: patternedRecurrence
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Pattern <IMicrosoftGraphRecurrencePattern>]`: recurrencePattern
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[DayOfMonth <Int32?>]`: The day of the month on which the event occurs.
Required if type is absoluteMonthly or absoluteYearly.
          - `[DaysOfWeek <String- `[]`>]`: A collection of the days of the week on which the event occurs.
The possible values are: sunday, monday, tuesday, wednesday, thursday, friday, saturday.
If type is relativeMonthly or relativeYearly, and daysOfWeek specifies more than one day, the event falls on the first day that satisfies the pattern.
Required if type is weekly, relativeMonthly, or relativeYearly.
          - `[FirstDayOfWeek <String>]`: dayOfWeek
          - `[Index <String>]`: weekIndex
          - `[Interval <Int32?>]`: The number of units between occurrences, where units can be in days, weeks, months, or years, depending on the type.
Required.
          - `[Month <Int32?>]`: The month in which the event occurs.
This is a number from 1 to 12.
          - `[Type <String>]`: recurrencePatternType
        - `[Range <IMicrosoftGraphRecurrenceRange>]`: recurrenceRange
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[EndDate <DateTime?>]`: The date to stop applying the recurrence pattern.
Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.
Required if type is endDate.
          - `[NumberOfOccurrences <Int32?>]`: The number of times to repeat the event.
Required and must be positive if type is numbered.
          - `[RecurrenceTimeZone <String>]`: Time zone for the startDate and endDate properties.
Optional.
If not specified, the time zone of the event is used.
          - `[StartDate <DateTime?>]`: The date to start applying the recurrence pattern.
The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.
Must be the same value as the start property of the recurring event.
Required.
          - `[Type <String>]`: recurrenceRangeType
      - `[StartDateTime <DateTime?>]`: When the  eligible or active assignment becomes active.
  - `[AssignmentType <String>]`: The type of the assignment that can either be Assigned or Activated.
Supports $filter (eq, ne).
  - `[MemberType <String>]`: How the assignment is inherited.
It can either be Inherited, Direct, or Group.
It can further imply whether the unifiedRoleAssignmentSchedule can be managed by the caller.
Supports $filter (eq, ne).
  - `[ScheduleInfo <IMicrosoftGraphRequestSchedule>]`: requestSchedule

ROLEDEFINITIONS `<IMicrosoftGraphUnifiedRoleDefinition- `[]`>`: Resource representing the roles allowed by RBAC providers and the permissions assigned to the roles.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Description <String>]`: The description for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
  - `[DisplayName <String>]`: The display name for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
Required.
Supports $filter (eq, in).
  - `[InheritsPermissionsFrom <IMicrosoftGraphUnifiedRoleDefinition- `[]`>]`: Read-only collection of role definitions that the given role definition inherits from.
Only Microsoft Entra built-in roles (isBuiltIn is true) support this attribute.
Supports $expand.
  - `[IsBuiltIn <Boolean?>]`: Flag indicating whether the role definition is part of the default set included in Microsoft Entra or a custom definition.
Read-only.
Supports $filter (eq, in).
  - `[IsEnabled <Boolean?>]`: Flag indicating whether the role is enabled for assignment.
If false the role is not available for assignment.
Read-only when isBuiltIn is true.
  - `[ResourceScopes <String- `[]`>]`: List of the scopes or permissions the role definition applies to.
Currently only / is supported.
Read-only when isBuiltIn is true.
DO NOT USE.
This will be deprecated soon.
Attach scope to role assignment.
  - `[RolePermissions <IMicrosoftGraphUnifiedRolePermission- `[]`>]`: List of permissions included in the role.
Read-only when isBuiltIn is true.
Required.
    - `[AllowedResourceActions <String- `[]`>]`: Set of tasks that can be performed on a resource.
Required.
    - `[Condition <String>]`: Optional constraints that must be met for the permission to be effective.
Not supported for custom roles.
    - `[ExcludedResourceActions <String- `[]`>]`: Set of tasks that may not be performed on a resource.
Not yet supported.
  - `[TemplateId <String>]`: Custom template identifier that can be set when isBuiltIn is false but is read-only when isBuiltIn is true.
This identifier is typically used if one needs an identifier to be the same across different directories.
  - `[Version <String>]`: Indicates version of the role definition.
Read-only when isBuiltIn is true.

ROLEELIGIBILITYSCHEDULEINSTANCES `<IMicrosoftGraphUnifiedRoleEligibilityScheduleInstance- `[]`>`: Instances for role eligibility requests.
  - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: Provides the display name of the app-specific resource represented by the app scope.
Provided for display purposes since appScopeId is often an immutable, non-human-readable id.
Read-only.
    - `[Type <String>]`: Describes the type of app-specific resource represented by the app scope and is provided for display purposes, so a user interface can convey to the user the kind of app specific resource represented by the app scope.
Read-only.
  - `[AppScopeId <String>]`: Identifier of the app-specific scope when the assignment or role eligibility is scoped to an app.
The scope of an assignment or role eligibility determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
  - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment or role eligibility.
The scope of an assignment or role eligibility determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
  - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
  - `[PrincipalId <String>]`: Identifier of the principal that has been granted the role assignment or that's eligible for a role.
  - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Description <String>]`: The description for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
    - `[DisplayName <String>]`: The display name for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
Required.
Supports $filter (eq, in).
    - `[InheritsPermissionsFrom <IMicrosoftGraphUnifiedRoleDefinition- `[]`>]`: Read-only collection of role definitions that the given role definition inherits from.
Only Microsoft Entra built-in roles (isBuiltIn is true) support this attribute.
Supports $expand.
    - `[IsBuiltIn <Boolean?>]`: Flag indicating whether the role definition is part of the default set included in Microsoft Entra or a custom definition.
Read-only.
Supports $filter (eq, in).
    - `[IsEnabled <Boolean?>]`: Flag indicating whether the role is enabled for assignment.
If false the role is not available for assignment.
Read-only when isBuiltIn is true.
    - `[ResourceScopes <String- `[]`>]`: List of the scopes or permissions the role definition applies to.
Currently only / is supported.
Read-only when isBuiltIn is true.
DO NOT USE.
This will be deprecated soon.
Attach scope to role assignment.
    - `[RolePermissions <IMicrosoftGraphUnifiedRolePermission- `[]`>]`: List of permissions included in the role.
Read-only when isBuiltIn is true.
Required.
      - `[AllowedResourceActions <String- `[]`>]`: Set of tasks that can be performed on a resource.
Required.
      - `[Condition <String>]`: Optional constraints that must be met for the permission to be effective.
Not supported for custom roles.
      - `[ExcludedResourceActions <String- `[]`>]`: Set of tasks that may not be performed on a resource.
Not yet supported.
    - `[TemplateId <String>]`: Custom template identifier that can be set when isBuiltIn is false but is read-only when isBuiltIn is true.
This identifier is typically used if one needs an identifier to be the same across different directories.
    - `[Version <String>]`: Indicates version of the role definition.
Read-only when isBuiltIn is true.
  - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal or that the principal is eligible for.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[EndDateTime <DateTime?>]`: The end date of the schedule instance.
  - `[MemberType <String>]`: How the role eligibility is inherited.
It can either be Inherited, Direct, or Group.
It can further imply whether the unifiedRoleEligibilitySchedule can be managed by the caller.
Supports $filter (eq, ne).
  - `[RoleEligibilityScheduleId <String>]`: The identifier of the unifiedRoleEligibilitySchedule object from which this instance was created.
Supports $filter (eq, ne).
  - `[StartDateTime <DateTime?>]`: When this instance starts.

ROLEELIGIBILITYSCHEDULEREQUESTS `<IMicrosoftGraphUnifiedRoleEligibilityScheduleRequest- `[]`>`: Requests for role eligibilities for principals through PIM.
  - `[ApprovalId <String>]`: The identifier of the approval of the request.
  - `[CompletedDateTime <DateTime?>]`: The request completion date time.
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[CreatedDateTime <DateTime?>]`: The request creation date time.
  - `[CustomData <String>]`: Free text field to define any custom data for the request.
Not used.
  - `[Status <String>]`: The status of the request.
Not nullable.
The possible values are: Canceled, Denied, Failed, Granted, PendingAdminDecision, PendingApproval, PendingProvisioning, PendingScheduleCreation, Provisioned, Revoked, and ScheduleCreated.
Not nullable.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[Action <String>]`: unifiedRoleScheduleRequestActions
  - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: Provides the display name of the app-specific resource represented by the app scope.
Provided for display purposes since appScopeId is often an immutable, non-human-readable id.
Read-only.
    - `[Type <String>]`: Describes the type of app-specific resource represented by the app scope and is provided for display purposes, so a user interface can convey to the user the kind of app specific resource represented by the app scope.
Read-only.
  - `[AppScopeId <String>]`: Identifier of the app-specific scope when the role eligibility is scoped to an app.
The scope of a role eligibility determines the set of resources for which the principal is eligible to access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
Supports $filter (eq, ne, and on null values).
  - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the role eligibility.
The scope of a role eligibility determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
Supports $filter (eq, ne, and on null values).
  - `[IsValidationOnly <Boolean?>]`: Determines whether the call is a validation or an actual call.
Only set this property if you want to check whether an activation is subject to additional rules like MFA before actually submitting the request.
  - `[Justification <String>]`: A message provided by users and administrators when create they create the unifiedRoleEligibilityScheduleRequest object.
  - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
  - `[PrincipalId <String>]`: Identifier of the principal that has been granted the role eligibility.
Can be a user or a role-assignable group.
You can grant only active assignments service principals.Supports $filter (eq, ne).
  - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Description <String>]`: The description for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
    - `[DisplayName <String>]`: The display name for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
Required.
Supports $filter (eq, in).
    - `[InheritsPermissionsFrom <IMicrosoftGraphUnifiedRoleDefinition- `[]`>]`: Read-only collection of role definitions that the given role definition inherits from.
Only Microsoft Entra built-in roles (isBuiltIn is true) support this attribute.
Supports $expand.
    - `[IsBuiltIn <Boolean?>]`: Flag indicating whether the role definition is part of the default set included in Microsoft Entra or a custom definition.
Read-only.
Supports $filter (eq, in).
    - `[IsEnabled <Boolean?>]`: Flag indicating whether the role is enabled for assignment.
If false the role is not available for assignment.
Read-only when isBuiltIn is true.
    - `[ResourceScopes <String- `[]`>]`: List of the scopes or permissions the role definition applies to.
Currently only / is supported.
Read-only when isBuiltIn is true.
DO NOT USE.
This will be deprecated soon.
Attach scope to role assignment.
    - `[RolePermissions <IMicrosoftGraphUnifiedRolePermission- `[]`>]`: List of permissions included in the role.
Read-only when isBuiltIn is true.
Required.
      - `[AllowedResourceActions <String- `[]`>]`: Set of tasks that can be performed on a resource.
Required.
      - `[Condition <String>]`: Optional constraints that must be met for the permission to be effective.
Not supported for custom roles.
      - `[ExcludedResourceActions <String- `[]`>]`: Set of tasks that may not be performed on a resource.
Not yet supported.
    - `[TemplateId <String>]`: Custom template identifier that can be set when isBuiltIn is false but is read-only when isBuiltIn is true.
This identifier is typically used if one needs an identifier to be the same across different directories.
    - `[Version <String>]`: Indicates version of the role definition.
Read-only when isBuiltIn is true.
  - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal.
Supports $filter (eq, ne).
  - `[ScheduleInfo <IMicrosoftGraphRequestSchedule>]`: requestSchedule
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Expiration <IMicrosoftGraphExpirationPattern>]`: expirationPattern
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Duration <TimeSpan?>]`: The requestor's desired duration of access represented in ISO 8601 format for durations.
For example, PT3H refers to three hours.
If specified in a request, endDateTime should not be present and the type property should be set to afterDuration.
      - `[EndDateTime <DateTime?>]`: Timestamp of date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
      - `[Type <String>]`: expirationPatternType
    - `[Recurrence <IMicrosoftGraphPatternedRecurrence>]`: patternedRecurrence
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Pattern <IMicrosoftGraphRecurrencePattern>]`: recurrencePattern
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DayOfMonth <Int32?>]`: The day of the month on which the event occurs.
Required if type is absoluteMonthly or absoluteYearly.
        - `[DaysOfWeek <String- `[]`>]`: A collection of the days of the week on which the event occurs.
The possible values are: sunday, monday, tuesday, wednesday, thursday, friday, saturday.
If type is relativeMonthly or relativeYearly, and daysOfWeek specifies more than one day, the event falls on the first day that satisfies the pattern.
Required if type is weekly, relativeMonthly, or relativeYearly.
        - `[FirstDayOfWeek <String>]`: dayOfWeek
        - `[Index <String>]`: weekIndex
        - `[Interval <Int32?>]`: The number of units between occurrences, where units can be in days, weeks, months, or years, depending on the type.
Required.
        - `[Month <Int32?>]`: The month in which the event occurs.
This is a number from 1 to 12.
        - `[Type <String>]`: recurrencePatternType
      - `[Range <IMicrosoftGraphRecurrenceRange>]`: recurrenceRange
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[EndDate <DateTime?>]`: The date to stop applying the recurrence pattern.
Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.
Required if type is endDate.
        - `[NumberOfOccurrences <Int32?>]`: The number of times to repeat the event.
Required and must be positive if type is numbered.
        - `[RecurrenceTimeZone <String>]`: Time zone for the startDate and endDate properties.
Optional.
If not specified, the time zone of the event is used.
        - `[StartDate <DateTime?>]`: The date to start applying the recurrence pattern.
The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.
Must be the same value as the start property of the recurring event.
Required.
        - `[Type <String>]`: recurrenceRangeType
    - `[StartDateTime <DateTime?>]`: When the  eligible or active assignment becomes active.
  - `[TargetSchedule <IMicrosoftGraphUnifiedRoleEligibilitySchedule>]`: unifiedRoleEligibilitySchedule
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
    - `[AppScopeId <String>]`: Identifier of the app-specific scope when the assignment or eligibility is scoped to an app.
The scope of an assignment or eligibility determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
    - `[CreatedDateTime <DateTime?>]`: When the schedule was created.
    - `[CreatedUsing <String>]`: Identifier of the object through which this schedule was created.
    - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment or eligibility.
The scope of an assignment or eligibility determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
    - `[ModifiedDateTime <DateTime?>]`: When the schedule was last modified.
    - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[PrincipalId <String>]`: Identifier of the principal that has been granted the role assignment or eligibility.
    - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
    - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal or that a principal is eligible for.
    - `[Status <String>]`: The status of the role assignment or eligibility request.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[MemberType <String>]`: How the role eligibility is inherited.
It can either be Inherited, Direct, or Group.
It can further imply whether the unifiedRoleEligibilitySchedule can be managed by the caller.
Supports $filter (eq, ne).
    - `[ScheduleInfo <IMicrosoftGraphRequestSchedule>]`: requestSchedule
  - `[TargetScheduleId <String>]`: Identifier of the schedule object that's linked to the eligibility request.
Supports $filter (eq, ne).
  - `[TicketInfo <IMicrosoftGraphTicketInfo>]`: ticketInfo
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[TicketNumber <String>]`: The ticket number.
    - `[TicketSystem <String>]`: The description of the ticket system.

ROLEELIGIBILITYSCHEDULES `<IMicrosoftGraphUnifiedRoleEligibilitySchedule- `[]`>`: Schedules for role eligibility operations.
  - `[AppScope <IMicrosoftGraphAppScope>]`: appScope
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: Provides the display name of the app-specific resource represented by the app scope.
Provided for display purposes since appScopeId is often an immutable, non-human-readable id.
Read-only.
    - `[Type <String>]`: Describes the type of app-specific resource represented by the app scope and is provided for display purposes, so a user interface can convey to the user the kind of app specific resource represented by the app scope.
Read-only.
  - `[AppScopeId <String>]`: Identifier of the app-specific scope when the assignment or eligibility is scoped to an app.
The scope of an assignment or eligibility determines the set of resources for which the principal has been granted access.
App scopes are scopes that are defined and understood by this application only.
Use / for tenant-wide app scopes.
Use directoryScopeId to limit the scope to particular directory objects, for example, administrative units.
  - `[CreatedDateTime <DateTime?>]`: When the schedule was created.
  - `[CreatedUsing <String>]`: Identifier of the object through which this schedule was created.
  - `[DirectoryScope <IMicrosoftGraphDirectoryObject>]`: directoryObject
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DeletedDateTime <DateTime?>]`: Date and time when this object was deleted.
Always null when the object hasn't been deleted.
  - `[DirectoryScopeId <String>]`: Identifier of the directory object representing the scope of the assignment or eligibility.
The scope of an assignment or eligibility determines the set of resources for which the principal has been granted access.
Directory scopes are shared scopes stored in the directory that are understood by multiple applications.
Use / for tenant-wide scope.
Use appScopeId to limit the scope to an application only.
  - `[ModifiedDateTime <DateTime?>]`: When the schedule was last modified.
  - `[Principal <IMicrosoftGraphDirectoryObject>]`: directoryObject
  - `[PrincipalId <String>]`: Identifier of the principal that has been granted the role assignment or eligibility.
  - `[RoleDefinition <IMicrosoftGraphUnifiedRoleDefinition>]`: unifiedRoleDefinition
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Description <String>]`: The description for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
    - `[DisplayName <String>]`: The display name for the unifiedRoleDefinition.
Read-only when isBuiltIn is true.
Required.
Supports $filter (eq, in).
    - `[InheritsPermissionsFrom <IMicrosoftGraphUnifiedRoleDefinition- `[]`>]`: Read-only collection of role definitions that the given role definition inherits from.
Only Microsoft Entra built-in roles (isBuiltIn is true) support this attribute.
Supports $expand.
    - `[IsBuiltIn <Boolean?>]`: Flag indicating whether the role definition is part of the default set included in Microsoft Entra or a custom definition.
Read-only.
Supports $filter (eq, in).
    - `[IsEnabled <Boolean?>]`: Flag indicating whether the role is enabled for assignment.
If false the role is not available for assignment.
Read-only when isBuiltIn is true.
    - `[ResourceScopes <String- `[]`>]`: List of the scopes or permissions the role definition applies to.
Currently only / is supported.
Read-only when isBuiltIn is true.
DO NOT USE.
This will be deprecated soon.
Attach scope to role assignment.
    - `[RolePermissions <IMicrosoftGraphUnifiedRolePermission- `[]`>]`: List of permissions included in the role.
Read-only when isBuiltIn is true.
Required.
      - `[AllowedResourceActions <String- `[]`>]`: Set of tasks that can be performed on a resource.
Required.
      - `[Condition <String>]`: Optional constraints that must be met for the permission to be effective.
Not supported for custom roles.
      - `[ExcludedResourceActions <String- `[]`>]`: Set of tasks that may not be performed on a resource.
Not yet supported.
    - `[TemplateId <String>]`: Custom template identifier that can be set when isBuiltIn is false but is read-only when isBuiltIn is true.
This identifier is typically used if one needs an identifier to be the same across different directories.
    - `[Version <String>]`: Indicates version of the role definition.
Read-only when isBuiltIn is true.
  - `[RoleDefinitionId <String>]`: Identifier of the unifiedRoleDefinition object that is being assigned to the principal or that a principal is eligible for.
  - `[Status <String>]`: The status of the role assignment or eligibility request.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[MemberType <String>]`: How the role eligibility is inherited.
It can either be Inherited, Direct, or Group.
It can further imply whether the unifiedRoleEligibilitySchedule can be managed by the caller.
Supports $filter (eq, ne).
  - `[ScheduleInfo <IMicrosoftGraphRequestSchedule>]`: requestSchedule
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Expiration <IMicrosoftGraphExpirationPattern>]`: expirationPattern
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Duration <TimeSpan?>]`: The requestor's desired duration of access represented in ISO 8601 format for durations.
For example, PT3H refers to three hours.
If specified in a request, endDateTime should not be present and the type property should be set to afterDuration.
      - `[EndDateTime <DateTime?>]`: Timestamp of date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
      - `[Type <String>]`: expirationPatternType
    - `[Recurrence <IMicrosoftGraphPatternedRecurrence>]`: patternedRecurrence
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Pattern <IMicrosoftGraphRecurrencePattern>]`: recurrencePattern
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DayOfMonth <Int32?>]`: The day of the month on which the event occurs.
Required if type is absoluteMonthly or absoluteYearly.
        - `[DaysOfWeek <String- `[]`>]`: A collection of the days of the week on which the event occurs.
The possible values are: sunday, monday, tuesday, wednesday, thursday, friday, saturday.
If type is relativeMonthly or relativeYearly, and daysOfWeek specifies more than one day, the event falls on the first day that satisfies the pattern.
Required if type is weekly, relativeMonthly, or relativeYearly.
        - `[FirstDayOfWeek <String>]`: dayOfWeek
        - `[Index <String>]`: weekIndex
        - `[Interval <Int32?>]`: The number of units between occurrences, where units can be in days, weeks, months, or years, depending on the type.
Required.
        - `[Month <Int32?>]`: The month in which the event occurs.
This is a number from 1 to 12.
        - `[Type <String>]`: recurrencePatternType
      - `[Range <IMicrosoftGraphRecurrenceRange>]`: recurrenceRange
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[EndDate <DateTime?>]`: The date to stop applying the recurrence pattern.
Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.
Required if type is endDate.
        - `[NumberOfOccurrences <Int32?>]`: The number of times to repeat the event.
Required and must be positive if type is numbered.
        - `[RecurrenceTimeZone <String>]`: Time zone for the startDate and endDate properties.
Optional.
If not specified, the time zone of the event is used.
        - `[StartDate <DateTime?>]`: The date to start applying the recurrence pattern.
The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.
Must be the same value as the start property of the recurring event.
Required.
        - `[Type <String>]`: recurrenceRangeType
    - `[StartDateTime <DateTime?>]`: When the  eligible or active assignment becomes active.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/update-mgrolemanagementdirectory](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/update-mgrolemanagementdirectory)
























