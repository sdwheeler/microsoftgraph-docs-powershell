---
external help file: Microsoft.Graph.Identity.Governance-help.xml
Module Name: Microsoft.Graph.Identity.Governance
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/set-mgidentitygovernanceaccessreviewdefinition
schema: 2.0.0
ms.subservice: entra-id-governance
---

# Set-MgIdentityGovernanceAccessReviewDefinition

## SYNOPSIS
Update an existing accessReviewScheduleDefinition object to change one or more of its properties.

> [!NOTE]
> To view the beta release of this cmdlet, view [Set-MgBetaIdentityGovernanceAccessReviewDefinition](/powershell/module/Microsoft.Graph.Beta.Identity.Governance/Set-MgBetaIdentityGovernanceAccessReviewDefinition?view=graph-powershell-beta)

## SYNTAX

### SetExpanded (Default)
```
Set-MgIdentityGovernanceAccessReviewDefinition -AccessReviewScheduleDefinitionId <String>
 [-ResponseHeadersVariable <String>]
 [-AdditionalNotificationRecipients <IMicrosoftGraphAccessReviewNotificationRecipientItem[]>]
 [-AdditionalProperties <Hashtable>] [-CreatedBy <IMicrosoftGraphUserIdentity>] [-CreatedDateTime <DateTime>]
 [-DescriptionForAdmins <String>] [-DescriptionForReviewers <String>] [-DisplayName <String>]
 [-FallbackReviewers <IMicrosoftGraphAccessReviewReviewerScope[]>] [-Id <String>]
 [-InstanceEnumerationScope <Hashtable>] [-Instances <IMicrosoftGraphAccessReviewInstance[]>]
 [-LastModifiedDateTime <DateTime>] [-Reviewers <IMicrosoftGraphAccessReviewReviewerScope[]>]
 [-Scope <Hashtable>] [-Settings <IMicrosoftGraphAccessReviewScheduleSettings>]
 [-StageSettings <IMicrosoftGraphAccessReviewStageSettings[]>] [-Status <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Set
```
Set-MgIdentityGovernanceAccessReviewDefinition -AccessReviewScheduleDefinitionId <String>
 -BodyParameter <IMicrosoftGraphAccessReviewScheduleDefinition> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SetViaIdentityExpanded
```
Set-MgIdentityGovernanceAccessReviewDefinition -InputObject <IIdentityGovernanceIdentity>
 [-ResponseHeadersVariable <String>]
 [-AdditionalNotificationRecipients <IMicrosoftGraphAccessReviewNotificationRecipientItem[]>]
 [-AdditionalProperties <Hashtable>] [-CreatedBy <IMicrosoftGraphUserIdentity>] [-CreatedDateTime <DateTime>]
 [-DescriptionForAdmins <String>] [-DescriptionForReviewers <String>] [-DisplayName <String>]
 [-FallbackReviewers <IMicrosoftGraphAccessReviewReviewerScope[]>] [-Id <String>]
 [-InstanceEnumerationScope <Hashtable>] [-Instances <IMicrosoftGraphAccessReviewInstance[]>]
 [-LastModifiedDateTime <DateTime>] [-Reviewers <IMicrosoftGraphAccessReviewReviewerScope[]>]
 [-Scope <Hashtable>] [-Settings <IMicrosoftGraphAccessReviewScheduleSettings>]
 [-StageSettings <IMicrosoftGraphAccessReviewStageSettings[]>] [-Status <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SetViaIdentity
```
Set-MgIdentityGovernanceAccessReviewDefinition -InputObject <IIdentityGovernanceIdentity>
 -BodyParameter <IMicrosoftGraphAccessReviewScheduleDefinition> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update an existing accessReviewScheduleDefinition object to change one or more of its properties.

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | AccessReview.ReadWrite.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | AccessReview.ReadWrite.All,  |

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	id = "60860cdd-fb4d-4054-91ba-f75e04444aa6"
	displayName = "Test world UPDATED NAME!"
	descriptionForAdmins = "Test world"
	descriptionForReviewers = "Test world"
	scope = @{
		"@odata.type" = "#microsoft.graph.accessReviewQueryScope"
		query = "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers"
		queryType = "MicrosoftGraph"
	}
	instanceEnumerationScope = @{
		"@odata.type" = "#microsoft.graph.accessReviewQueryScope"
		query = "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f"
		queryType = "MicrosoftGraph"
	}
	reviewers = @(
	)
	settings = @{
		mailNotificationsEnabled = $true
		reminderNotificationsEnabled = $true
		justificationRequiredOnApproval = $true
		defaultDecisionEnabled = $false
		defaultDecision = "None"
		instanceDurationInDays = 3
		autoApplyDecisionsEnabled = $false
		recommendationsEnabled = $true
		recurrence = @{
			pattern = @{
				type = "weekly"
				interval = 1
			}
			range = @{
				type = "noEnd"
				startDate = "2020-09-15"
			}
		}
	}
}

Set-MgIdentityGovernanceAccessReviewDefinition -AccessReviewScheduleDefinitionId $accessReviewScheduleDefinitionId -BodyParameter $params

```
This example shows how to use the Set-MgIdentityGovernanceAccessReviewDefinition Cmdlet.


## PARAMETERS

### -AccessReviewScheduleDefinitionId
The unique identifier of accessReviewScheduleDefinition

```yaml
Type: String
Parameter Sets: SetExpanded, Set
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AdditionalNotificationRecipients
Defines the list of additional users or group members to be notified of the access review progress.
To construct, see NOTES section for ADDITIONALNOTIFICATIONRECIPIENTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessReviewNotificationRecipientItem[]
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
accessReviewScheduleDefinition
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessReviewScheduleDefinition
Parameter Sets: Set, SetViaIdentity
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

### -CreatedBy
userIdentity
To construct, see NOTES section for CREATEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphUserIdentity
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreatedDateTime
Timestamp when the access review series was created.
Supports $select.
Read-only.

```yaml
Type: DateTime
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DescriptionForAdmins
Description provided by review creators to provide more context of the review to admins.
Supports $select.

```yaml
Type: String
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DescriptionForReviewers
Description provided by review creators to provide more context of the review to reviewers.
Reviewers see this description in the email sent to them requesting their review.
Email notifications support up to 256 characters.
Supports $select.

```yaml
Type: String
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
Name of the access review series.
Supports $select and $orderby.
Required on create.

```yaml
Type: String
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FallbackReviewers
This collection of reviewer scopes is used to define the list of fallback reviewers.
These fallback reviewers are notified to take action if no users are found from the list of reviewers specified.
This could occur when either the group owner is specified as the reviewer but the group owner doesn't exist, or manager is specified as reviewer but a user's manager doesn't exist.
See accessReviewReviewerScope.
Replaces backupReviewers.
Supports $select.
NOTE: The value of this property will be ignored if fallback reviewers are assigned through the stageSettings property.
To construct, see NOTES section for FALLBACKREVIEWERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessReviewReviewerScope[]
Parameter Sets: SetExpanded, SetViaIdentityExpanded
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
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IIdentityGovernanceIdentity
Parameter Sets: SetViaIdentityExpanded, SetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -InstanceEnumerationScope
accessReviewScope

```yaml
Type: Hashtable
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Instances
If the accessReviewScheduleDefinition is a recurring access review, instances represent each recurrence.
A review that doesn't recur will have exactly one instance.
Instances also represent each unique resource under review in the accessReviewScheduleDefinition.
If a review has multiple resources and multiple instances, each resource has a unique instance for each recurrence.
To construct, see NOTES section for INSTANCES properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessReviewInstance[]
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedDateTime
Timestamp when the access review series was last modified.
Supports $select.
Read-only.

```yaml
Type: DateTime
Parameter Sets: SetExpanded, SetViaIdentityExpanded
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

### -Reviewers
This collection of access review scopes is used to define who are the reviewers.
The reviewers property is only updatable if individual users are assigned as reviewers.
Required on create.
Supports $select.
For examples of options for assigning reviewers, see Assign reviewers to your access review definition using the Microsoft Graph API.
NOTE: The value of this property will be ignored if reviewers are assigned through the stageSettings property.
To construct, see NOTES section for REVIEWERS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessReviewReviewerScope[]
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Scope
accessReviewScope

```yaml
Type: Hashtable
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Settings
accessReviewScheduleSettings
To construct, see NOTES section for SETTINGS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessReviewScheduleSettings
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StageSettings
Required only for a multi-stage access review to define the stages and their settings.
You can break down each review instance into up to three sequential stages, where each stage can have a different set of reviewers, fallback reviewers, and settings.
Stages are created sequentially based on the dependsOn property.
Optional.
When this property is defined, its settings are used instead of the corresponding settings in the accessReviewScheduleDefinition object and its settings, reviewers, and fallbackReviewers properties.
To construct, see NOTES section for STAGESETTINGS properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccessReviewStageSettings[]
Parameter Sets: SetExpanded, SetViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Status
This read-only field specifies the status of an access review.
The typical states include Initializing, NotStarted, Starting, InProgress, Completing, Completed, AutoReviewing, and AutoReviewed.
Supports $select, $orderby, and $filter (eq only).
Read-only.

```yaml
Type: String
Parameter Sets: SetExpanded, SetViaIdentityExpanded
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

### Microsoft.Graph.PowerShell.Models.IIdentityGovernanceIdentity
### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAccessReviewScheduleDefinition
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphAccessReviewScheduleDefinition
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ADDITIONALNOTIFICATIONRECIPIENTS `<IMicrosoftGraphAccessReviewNotificationRecipientItem- `[]`>`: Defines the list of additional users or group members to be notified of the access review progress.
  - `[NotificationRecipientScope <IMicrosoftGraphAccessReviewNotificationRecipientScope>]`: accessReviewNotificationRecipientScope
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[NotificationTemplateType <String>]`: Indicates the type of access review email to be sent.
Supported template type is CompletedAdditionalRecipients, which sends review completion notifications to the recipients.

BODYPARAMETER `<IMicrosoftGraphAccessReviewScheduleDefinition>`: accessReviewScheduleDefinition
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AdditionalNotificationRecipients <IMicrosoftGraphAccessReviewNotificationRecipientItem- `[]`>]`: Defines the list of additional users or group members to be notified of the access review progress.
    - `[NotificationRecipientScope <IMicrosoftGraphAccessReviewNotificationRecipientScope>]`: accessReviewNotificationRecipientScope
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[NotificationTemplateType <String>]`: Indicates the type of access review email to be sent.
Supported template type is CompletedAdditionalRecipients, which sends review completion notifications to the recipients.
  - `[CreatedBy <IMicrosoftGraphUserIdentity>]`: userIdentity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
    - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
    - `[IPAddress <String>]`: Indicates the client IP address associated with the user performing the activity (audit log only).
    - `[UserPrincipalName <String>]`: The userPrincipalName attribute of the user.
  - `[CreatedDateTime <DateTime?>]`: Timestamp when the access review series was created.
Supports $select.
Read-only.
  - `[DescriptionForAdmins <String>]`: Description provided by review creators to provide more context of the review to admins.
Supports $select.
  - `[DescriptionForReviewers <String>]`: Description provided  by review creators to provide more context of the review to reviewers.
Reviewers see this description in the email sent to them requesting their review.
Email notifications support up to 256 characters.
Supports $select.
  - `[DisplayName <String>]`: Name of the access review series.
Supports $select and $orderby.
Required on create.
  - `[FallbackReviewers <IMicrosoftGraphAccessReviewReviewerScope- `[]`>]`: This collection of reviewer scopes is used to define the list of fallback reviewers.
These fallback reviewers are notified to take action if no users are found from the list of reviewers specified.
This could occur when either the group owner is specified as the reviewer but the group owner doesn't exist, or manager is specified as reviewer but a user's manager doesn't exist.
See accessReviewReviewerScope.
Replaces backupReviewers.
Supports $select.
NOTE: The value of this property will be ignored if fallback reviewers are assigned through the stageSettings property.
    - `[Query <String>]`: The query specifying who will be the reviewer.
    - `[QueryRoot <String>]`: In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.
This property is only required if a relative query, for example, ./manager, is specified.
Possible value: decisions.
    - `[QueryType <String>]`: The type of query.
Examples include MicrosoftGraph and ARM.
  - `[InstanceEnumerationScope <IMicrosoftGraphAccessReviewScope>]`: accessReviewScope
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Instances <IMicrosoftGraphAccessReviewInstance- `[]`>]`: If the accessReviewScheduleDefinition is a recurring access review, instances represent each recurrence.
A review that doesn't recur will have exactly one instance.
Instances also represent each unique resource under review in the accessReviewScheduleDefinition.
If a review has multiple resources and multiple instances, each resource has a unique instance for each recurrence.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ContactedReviewers <IMicrosoftGraphAccessReviewReviewer- `[]`>]`: Returns the collection of reviewers who were contacted to complete this review.
While the reviewers and fallbackReviewers properties of the accessReviewScheduleDefinition might specify group owners or managers as reviewers, contactedReviewers returns their individual identities.
Supports $select.
Read-only.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[CreatedDateTime <DateTime?>]`: The date when the reviewer was added for the access review.
      - `[DisplayName <String>]`: Name of reviewer.
      - `[UserPrincipalName <String>]`: User principal name of the reviewer.
    - `[Decisions <IMicrosoftGraphAccessReviewInstanceDecisionItem- `[]`>]`: Each user reviewed in an accessReviewInstance has a decision item representing if they were approved, denied, or not yet reviewed.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AccessReviewId <String>]`: The identifier of the accessReviewInstance parent.
Supports $select.
Read-only.
      - `[AppliedBy <IMicrosoftGraphUserIdentity>]`: userIdentity
      - `[AppliedDateTime <DateTime?>]`: The timestamp when the approval decision was applied.00000000-0000-0000-0000-000000000000 if the assigned reviewer hasn't applied the decision or it was automatically applied.
The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Supports $select.
Read-only.
      - `[ApplyResult <String>]`: The result of applying the decision.
Possible values: New, AppliedSuccessfully, AppliedWithUnknownFailure, AppliedSuccessfullyButObjectNotFound and ApplyNotSupported.
Supports $select, $orderby, and $filter (eq only).
Read-only.
      - `[Decision <String>]`: Result of the review.
Possible values: Approve, Deny, NotReviewed, or DontKnow.
Supports $select, $orderby, and $filter (eq only).
      - `[Insights <IMicrosoftGraphGovernanceInsight- `[]`>]`: Insights are recommendations to reviewers on whether to approve or deny a decision.
There can be multiple insights associated with an accessReviewInstanceDecisionItem.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[InsightCreatedDateTime <DateTime?>]`: Indicates when the insight was created.
      - `[Justification <String>]`: Justification left by the reviewer when they made the decision.
      - `[Principal <IMicrosoftGraphIdentity>]`: identity
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
        - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
      - `[PrincipalLink <String>]`: A link to the principal object.
For example, https://graph.microsoft.com/v1.0/users/a6c7aecb-cbfd-4763-87ef-e91b4bd509d9.
Read-only.
      - `[Recommendation <String>]`: A system-generated recommendation for the approval decision based off last interactive sign-in to tenant.
The value is Approve if the sign-in is fewer than 30 days after the start of review, Deny if the sign-in is greater than 30 days after, or NoInfoAvailable.
Possible values: Approve, Deny, or NoInfoAvailable.
Supports $select, $orderby, and $filter (eq only).
Read-only.
      - `[Resource <IMicrosoftGraphAccessReviewInstanceDecisionItemResource>]`: accessReviewInstanceDecisionItemResource
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[DisplayName <String>]`: Display name of the resource
        - `[Id <String>]`: Identifier of the resource
        - `[Type <String>]`: Type of resource.
Types include: Group, ServicePrincipal, DirectoryRole, AzureRole, AccessPackageAssignmentPolicy.
      - `[ResourceLink <String>]`: A link to the resource.
For example, https://graph.microsoft.com/v1.0/servicePrincipals/c86300f3-8695-4320-9f6e-32a2555f5ff8.
Supports $select.
Read-only.
      - `[ReviewedBy <IMicrosoftGraphUserIdentity>]`: userIdentity
      - `[ReviewedDateTime <DateTime?>]`: The timestamp when the review decision occurred.
Supports $select.
Read-only.
    - `[EndDateTime <DateTime?>]`: DateTime when review instance is scheduled to end.The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Supports $select.
Read-only.
    - `[FallbackReviewers <IMicrosoftGraphAccessReviewReviewerScope- `[]`>]`: This collection of reviewer scopes is used to define the list of fallback reviewers.
These fallback reviewers will be notified to take action if no users are found from the list of reviewers specified.
This could occur when either the group owner is specified as the reviewer but the group owner does not exist, or manager is specified as reviewer but a user's manager does not exist.
Supports $select.
    - `[Reviewers <IMicrosoftGraphAccessReviewReviewerScope- `[]`>]`: This collection of access review scopes is used to define who the reviewers are.
Supports $select.
For examples of options for assigning reviewers, see Assign reviewers to your access review definition using the Microsoft Graph API.
    - `[Scope <IMicrosoftGraphAccessReviewScope>]`: accessReviewScope
    - `[Stages <IMicrosoftGraphAccessReviewStage- `[]`>]`: If the instance has multiple stages, this returns the collection of stages.
A new stage will only be created when the previous stage ends.
The existence, number, and settings of stages on a review instance are created based on the accessReviewStageSettings on the parent accessReviewScheduleDefinition.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[Decisions <IMicrosoftGraphAccessReviewInstanceDecisionItem- `[]`>]`: Each user reviewed in an accessReviewStage has a decision item representing if they were approved, denied, or not yet reviewed.
      - `[EndDateTime <DateTime?>]`: The date and time in ISO 8601 format and UTC time when the review stage is scheduled to end.
This property is the cumulative total of the durationInDays for all stages.
Read-only.
      - `[FallbackReviewers <IMicrosoftGraphAccessReviewReviewerScope- `[]`>]`: This collection of reviewer scopes is used to define the list of fallback reviewers.
These fallback reviewers are notified to take action if no users are found from the list of reviewers specified.
This could occur when either the group owner is specified as the reviewer but the group owner doesn't exist, or manager is specified as reviewer but a user's manager doesn't exist.
      - `[Reviewers <IMicrosoftGraphAccessReviewReviewerScope- `[]`>]`: This collection of access review scopes is used to define who the reviewers are.
For examples of options for assigning reviewers, see Assign reviewers to your access review definition using the Microsoft Graph API.
      - `[StartDateTime <DateTime?>]`: The date and time in ISO 8601 format and UTC time when the review stage is scheduled to start.
Read-only.
      - `[Status <String>]`: Specifies the status of an accessReviewStage.
Possible values: Initializing, NotStarted, Starting, InProgress, Completing, Completed, AutoReviewing, and AutoReviewed.
Supports $orderby, and $filter (eq only).
Read-only.
    - `[StartDateTime <DateTime?>]`: DateTime when review instance is scheduled to start.
May be in the future.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Supports $select.
Read-only.
    - `[Status <String>]`: Specifies the status of an accessReview.
Possible values: Initializing, NotStarted, Starting, InProgress, Completing, Completed, AutoReviewing, and AutoReviewed.
Supports $select, $orderby, and $filter (eq only).
Read-only.
  - `[LastModifiedDateTime <DateTime?>]`: Timestamp when the access review series was last modified.
Supports $select.
Read-only.
  - `[Reviewers <IMicrosoftGraphAccessReviewReviewerScope- `[]`>]`: This collection of access review scopes is used to define who are the reviewers.
The reviewers property is only updatable if individual users are assigned as reviewers.
Required on create.
Supports $select.
For examples of options for assigning reviewers, see Assign reviewers to your access review definition using the Microsoft Graph API.
NOTE: The value of this property will be ignored if reviewers are assigned through the stageSettings property.
  - `[Scope <IMicrosoftGraphAccessReviewScope>]`: accessReviewScope
  - `[Settings <IMicrosoftGraphAccessReviewScheduleSettings>]`: accessReviewScheduleSettings
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[ApplyActions <IMicrosoftGraphAccessReviewApplyAction- `[]`>]`: Optional field.
Describes the  actions to take once a review is complete.
There are two types that are currently supported: removeAccessApplyAction (default) and disableAndDeleteUserApplyAction.
Field only needs to be specified in the case of disableAndDeleteUserApplyAction.
    - `[AutoApplyDecisionsEnabled <Boolean?>]`: Indicates whether decisions are automatically applied.
When set to false, an admin must apply the decisions manually once the reviewer completes the access review.
When set to true, decisions are applied automatically after the access review instance duration ends, whether or not the reviewers have responded.
Default value is false.
CAUTION: If both autoApplyDecisionsEnabled and defaultDecisionEnabled are true, all access for the principals to the resource risks being revoked if the reviewers fail to respond.
    - `[DecisionHistoriesForReviewersEnabled <Boolean?>]`: Indicates whether decisions on previous access review stages are available for reviewers on an accessReviewInstance with multiple subsequent stages.
If not provided, the default is disabled (false).
    - `[DefaultDecision <String>]`: Decision chosen if defaultDecisionEnabled is enabled.
Can be one of Approve, Deny, or Recommendation.
    - `[DefaultDecisionEnabled <Boolean?>]`: Indicates whether the default decision is enabled or disabled when reviewers do not respond.
Default value is false.
CAUTION: If both autoApplyDecisionsEnabled and defaultDecisionEnabled are true, all access for the principals to the resource risks being revoked if the reviewers fail to respond.
    - `[InstanceDurationInDays <Int32?>]`: Duration of an access review instance in days.
NOTE: If the stageSettings of the accessReviewScheduleDefinition object is defined, its durationInDays setting will be used instead of the value of this property.
    - `[JustificationRequiredOnApproval <Boolean?>]`: Indicates whether reviewers are required to provide justification with their decision.
Default value is false.
    - `[MailNotificationsEnabled <Boolean?>]`: Indicates whether emails are enabled or disabled.
Default value is false.
    - `[RecommendationInsightSettings <IMicrosoftGraphAccessReviewRecommendationInsightSetting- `[]`>]`: Optional.
Describes the types of insights that aid reviewers to make access review decisions.
NOTE: If the stageSettings of the accessReviewScheduleDefinition object is defined, its recommendationInsightSettings setting will be used instead of the value of this property.
    - `[RecommendationLookBackDuration <TimeSpan?>]`: Optional field.
Indicates the period of inactivity (with respect to the start date of the review instance) that recommendations will be configured from.
The recommendation will be to deny if the user is inactive during the look-back duration.
For reviews of groups and Microsoft Entra roles, any duration is accepted.
For reviews of applications, 30 days is the maximum duration.
If not specified, the duration is 30 days.
NOTE: If the stageSettings of the accessReviewScheduleDefinition object is defined, its recommendationLookBackDuration setting will be used instead of the value of this property.
    - `[RecommendationsEnabled <Boolean?>]`: Indicates whether decision recommendations are enabled or disabled.
NOTE: If the stageSettings of the accessReviewScheduleDefinition object is defined, its recommendationsEnabled setting will be used instead of the value of this property.
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
    - `[ReminderNotificationsEnabled <Boolean?>]`: Indicates whether reminders are enabled or disabled.
Default value is false.
  - `[StageSettings <IMicrosoftGraphAccessReviewStageSettings- `[]`>]`: Required only for a multi-stage access review to define the stages and their settings.
You can break down each review instance into up to three sequential stages, where each stage can have a different set of reviewers, fallback reviewers, and settings.
Stages are created sequentially based on the dependsOn property.
Optional.
When this property is defined, its settings are used instead of the corresponding settings in the accessReviewScheduleDefinition object and its settings, reviewers, and fallbackReviewers properties.
    - `[DecisionsThatWillMoveToNextStage <String- `[]`>]`: Indicate which decisions will go to the next stage.
Can be a subset of Approve, Deny, Recommendation, or NotReviewed.
If not provided, all decisions will go to the next stage.
Optional.
    - `[DependsOn <String- `[]`>]`: Defines the sequential or parallel order of the stages and depends on the stageId.
Only sequential stages are currently supported.
For example, if stageId is 2, then dependsOn must be 1.
If stageId is 1, don't specify dependsOn.
Required if stageId isn't 1.
    - `[DurationInDays <Int32?>]`: The duration of the stage.
Required.
NOTE: The cumulative value of this property across all stages  1.
Will override the instanceDurationInDays setting on the accessReviewScheduleDefinition object.
2.
Can't exceed the length of one recurrence.
That is, if the review recurs weekly, the cumulative durationInDays can't exceed 7.
    - `[FallbackReviewers <IMicrosoftGraphAccessReviewReviewerScope- `[]`>]`: If provided, the fallback reviewers are asked to complete a review if the primary reviewers don't exist.
For example, if managers are selected as reviewers and a principal under review doesn't have a manager in Microsoft Entra ID, the fallback reviewers are asked to review that principal.
NOTE: The value of this property overrides the corresponding setting on the accessReviewScheduleDefinition object.
    - `[RecommendationInsightSettings <IMicrosoftGraphAccessReviewRecommendationInsightSetting- `[]`>]`:
    - `[RecommendationsEnabled <Boolean?>]`: Indicates whether showing recommendations to reviewers is enabled.
Required.
NOTE: The value of this property overrides override the corresponding setting on the accessReviewScheduleDefinition object.
    - `[Reviewers <IMicrosoftGraphAccessReviewReviewerScope- `[]`>]`: Defines who the reviewers are.
If none is specified, the review is a self-review (users review their own access).
For examples of options for assigning reviewers, see Assign reviewers to your access review definition using the Microsoft Graph API.
NOTE: The value of this property overrides the corresponding setting on the accessReviewScheduleDefinition.
    - `[StageId <String>]`: Unique identifier of the accessReviewStageSettings object.
The stageId is used by the dependsOn property to indicate the order of the stages.
Required.
  - `[Status <String>]`: This read-only field specifies the status of an access review.
The typical states include Initializing, NotStarted, Starting, InProgress, Completing, Completed, AutoReviewing, and AutoReviewed.
Supports $select, $orderby, and $filter (eq only).
Read-only.

CREATEDBY `<IMicrosoftGraphUserIdentity>`: userIdentity
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
  - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
  - `[IPAddress <String>]`: Indicates the client IP address associated with the user performing the activity (audit log only).
  - `[UserPrincipalName <String>]`: The userPrincipalName attribute of the user.

FALLBACKREVIEWERS `<IMicrosoftGraphAccessReviewReviewerScope- `[]`>`: This collection of reviewer scopes is used to define the list of fallback reviewers.
These fallback reviewers are notified to take action if no users are found from the list of reviewers specified.
This could occur when either the group owner is specified as the reviewer but the group owner doesn't exist, or manager is specified as reviewer but a user's manager doesn't exist.
See accessReviewReviewerScope.
Replaces backupReviewers.
Supports $select.
NOTE: The value of this property will be ignored if fallback reviewers are assigned through the stageSettings property.
  - `[Query <String>]`: The query specifying who will be the reviewer.
  - `[QueryRoot <String>]`: In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.
This property is only required if a relative query, for example, ./manager, is specified.
Possible value: decisions.
  - `[QueryType <String>]`: The type of query.
Examples include MicrosoftGraph and ARM.

INPUTOBJECT `<IIdentityGovernanceIdentity>`: Identity Parameter
  - `[AccessPackageAssignmentId <String>]`: The unique identifier of accessPackageAssignment
  - `[AccessPackageAssignmentPolicyId <String>]`: The unique identifier of accessPackageAssignmentPolicy
  - `[AccessPackageAssignmentRequestId <String>]`: The unique identifier of accessPackageAssignmentRequest
  - `[AccessPackageCatalogId <String>]`: The unique identifier of accessPackageCatalog
  - `[AccessPackageId <String>]`: The unique identifier of accessPackage
  - `[AccessPackageId1 <String>]`: The unique identifier of accessPackage
  - `[AccessPackageQuestionId <String>]`: The unique identifier of accessPackageQuestion
  - `[AccessPackageResourceEnvironmentId <String>]`: The unique identifier of accessPackageResourceEnvironment
  - `[AccessPackageResourceId <String>]`: The unique identifier of accessPackageResource
  - `[AccessPackageResourceRequestId <String>]`: The unique identifier of accessPackageResourceRequest
  - `[AccessPackageResourceRoleId <String>]`: The unique identifier of accessPackageResourceRole
  - `[AccessPackageResourceRoleId1 <String>]`: The unique identifier of accessPackageResourceRole
  - `[AccessPackageResourceRoleScopeId <String>]`: The unique identifier of accessPackageResourceRoleScope
  - `[AccessPackageResourceScopeId <String>]`: The unique identifier of accessPackageResourceScope
  - `[AccessPackageResourceScopeId1 <String>]`: The unique identifier of accessPackageResourceScope
  - `[AccessReviewHistoryDefinitionId <String>]`: The unique identifier of accessReviewHistoryDefinition
  - `[AccessReviewHistoryInstanceId <String>]`: The unique identifier of accessReviewHistoryInstance
  - `[AccessReviewInstanceDecisionItemId <String>]`: The unique identifier of accessReviewInstanceDecisionItem
  - `[AccessReviewInstanceId <String>]`: The unique identifier of accessReviewInstance
  - `[AccessReviewReviewerId <String>]`: The unique identifier of accessReviewReviewer
  - `[AccessReviewScheduleDefinitionId <String>]`: The unique identifier of accessReviewScheduleDefinition
  - `[AccessReviewStageId <String>]`: The unique identifier of accessReviewStage
  - `[AgreementAcceptanceId <String>]`: The unique identifier of agreementAcceptance
  - `[AgreementFileLocalizationId <String>]`: The unique identifier of agreementFileLocalization
  - `[AgreementFileVersionId <String>]`: The unique identifier of agreementFileVersion
  - `[AgreementId <String>]`: The unique identifier of agreement
  - `[AppConsentRequestId <String>]`: The unique identifier of appConsentRequest
  - `[ApprovalId <String>]`: The unique identifier of approval
  - `[ApprovalStageId <String>]`: The unique identifier of approvalStage
  - `[ConnectedOrganizationId <String>]`: The unique identifier of connectedOrganization
  - `[CustomCalloutExtensionId <String>]`: The unique identifier of customCalloutExtension
  - `[CustomExtensionStageSettingId <String>]`: The unique identifier of customExtensionStageSetting
  - `[CustomTaskExtensionId <String>]`: The unique identifier of customTaskExtension
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[EndDateTime <DateTime?>]`: Usage: endDateTime={endDateTime}
  - `[GovernanceInsightId <String>]`: The unique identifier of governanceInsight
  - `[IncompatibleAccessPackageId <String>]`: Usage: incompatibleAccessPackageId='{incompatibleAccessPackageId}'
  - `[On <String>]`: Usage: on='{on}'
  - `[PrivilegedAccessGroupAssignmentScheduleId <String>]`: The unique identifier of privilegedAccessGroupAssignmentSchedule
  - `[PrivilegedAccessGroupAssignmentScheduleInstanceId <String>]`: The unique identifier of privilegedAccessGroupAssignmentScheduleInstance
  - `[PrivilegedAccessGroupAssignmentScheduleRequestId <String>]`: The unique identifier of privilegedAccessGroupAssignmentScheduleRequest
  - `[PrivilegedAccessGroupEligibilityScheduleId <String>]`: The unique identifier of privilegedAccessGroupEligibilitySchedule
  - `[PrivilegedAccessGroupEligibilityScheduleInstanceId <String>]`: The unique identifier of privilegedAccessGroupEligibilityScheduleInstance
  - `[PrivilegedAccessGroupEligibilityScheduleRequestId <String>]`: The unique identifier of privilegedAccessGroupEligibilityScheduleRequest
  - `[RunId <String>]`: The unique identifier of run
  - `[StartDateTime <DateTime?>]`: Usage: startDateTime={startDateTime}
  - `[TaskDefinitionId <String>]`: The unique identifier of taskDefinition
  - `[TaskId <String>]`: The unique identifier of task
  - `[TaskProcessingResultId <String>]`: The unique identifier of taskProcessingResult
  - `[TaskReportId <String>]`: The unique identifier of taskReport
  - `[UnifiedRbacResourceActionId <String>]`: The unique identifier of unifiedRbacResourceAction
  - `[UnifiedRbacResourceNamespaceId <String>]`: The unique identifier of unifiedRbacResourceNamespace
  - `[UnifiedRoleAssignmentId <String>]`: The unique identifier of unifiedRoleAssignment
  - `[UnifiedRoleAssignmentScheduleId <String>]`: The unique identifier of unifiedRoleAssignmentSchedule
  - `[UnifiedRoleAssignmentScheduleInstanceId <String>]`: The unique identifier of unifiedRoleAssignmentScheduleInstance
  - `[UnifiedRoleAssignmentScheduleRequestId <String>]`: The unique identifier of unifiedRoleAssignmentScheduleRequest
  - `[UnifiedRoleDefinitionId <String>]`: The unique identifier of unifiedRoleDefinition
  - `[UnifiedRoleDefinitionId1 <String>]`: The unique identifier of unifiedRoleDefinition
  - `[UnifiedRoleEligibilityScheduleId <String>]`: The unique identifier of unifiedRoleEligibilitySchedule
  - `[UnifiedRoleEligibilityScheduleInstanceId <String>]`: The unique identifier of unifiedRoleEligibilityScheduleInstance
  - `[UnifiedRoleEligibilityScheduleRequestId <String>]`: The unique identifier of unifiedRoleEligibilityScheduleRequest
  - `[UserConsentRequestId <String>]`: The unique identifier of userConsentRequest
  - `[UserId <String>]`: The unique identifier of user
  - `[UserProcessingResultId <String>]`: The unique identifier of userProcessingResult
  - `[WorkflowId <String>]`: The unique identifier of workflow
  - `[WorkflowTemplateId <String>]`: The unique identifier of workflowTemplate
  - `[WorkflowVersionNumber <Int32?>]`: The unique identifier of workflowVersion

INSTANCES `<IMicrosoftGraphAccessReviewInstance- `[]`>`: If the accessReviewScheduleDefinition is a recurring access review, instances represent each recurrence.
A review that doesn't recur will have exactly one instance.
Instances also represent each unique resource under review in the accessReviewScheduleDefinition.
If a review has multiple resources and multiple instances, each resource has a unique instance for each recurrence.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ContactedReviewers <IMicrosoftGraphAccessReviewReviewer- `[]`>]`: Returns the collection of reviewers who were contacted to complete this review.
While the reviewers and fallbackReviewers properties of the accessReviewScheduleDefinition might specify group owners or managers as reviewers, contactedReviewers returns their individual identities.
Supports $select.
Read-only.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[CreatedDateTime <DateTime?>]`: The date when the reviewer was added for the access review.
    - `[DisplayName <String>]`: Name of reviewer.
    - `[UserPrincipalName <String>]`: User principal name of the reviewer.
  - `[Decisions <IMicrosoftGraphAccessReviewInstanceDecisionItem- `[]`>]`: Each user reviewed in an accessReviewInstance has a decision item representing if they were approved, denied, or not yet reviewed.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AccessReviewId <String>]`: The identifier of the accessReviewInstance parent.
Supports $select.
Read-only.
    - `[AppliedBy <IMicrosoftGraphUserIdentity>]`: userIdentity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
      - `[IPAddress <String>]`: Indicates the client IP address associated with the user performing the activity (audit log only).
      - `[UserPrincipalName <String>]`: The userPrincipalName attribute of the user.
    - `[AppliedDateTime <DateTime?>]`: The timestamp when the approval decision was applied.00000000-0000-0000-0000-000000000000 if the assigned reviewer hasn't applied the decision or it was automatically applied.
The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Supports $select.
Read-only.
    - `[ApplyResult <String>]`: The result of applying the decision.
Possible values: New, AppliedSuccessfully, AppliedWithUnknownFailure, AppliedSuccessfullyButObjectNotFound and ApplyNotSupported.
Supports $select, $orderby, and $filter (eq only).
Read-only.
    - `[Decision <String>]`: Result of the review.
Possible values: Approve, Deny, NotReviewed, or DontKnow.
Supports $select, $orderby, and $filter (eq only).
    - `[Insights <IMicrosoftGraphGovernanceInsight- `[]`>]`: Insights are recommendations to reviewers on whether to approve or deny a decision.
There can be multiple insights associated with an accessReviewInstanceDecisionItem.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[InsightCreatedDateTime <DateTime?>]`: Indicates when the insight was created.
    - `[Justification <String>]`: Justification left by the reviewer when they made the decision.
    - `[Principal <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.For drive items, the display name might not always be available or up to date.
For example, if a user changes their display name the API might show the new value in a future response, but the items associated with the user don't show up as changed when using delta.
      - `[Id <String>]`: Unique identifier for the identity or actor.
For example, in the access reviews decisions API, this property might record the id of the principal, that is, the group, user, or application that's subject to review.
    - `[PrincipalLink <String>]`: A link to the principal object.
For example, https://graph.microsoft.com/v1.0/users/a6c7aecb-cbfd-4763-87ef-e91b4bd509d9.
Read-only.
    - `[Recommendation <String>]`: A system-generated recommendation for the approval decision based off last interactive sign-in to tenant.
The value is Approve if the sign-in is fewer than 30 days after the start of review, Deny if the sign-in is greater than 30 days after, or NoInfoAvailable.
Possible values: Approve, Deny, or NoInfoAvailable.
Supports $select, $orderby, and $filter (eq only).
Read-only.
    - `[Resource <IMicrosoftGraphAccessReviewInstanceDecisionItemResource>]`: accessReviewInstanceDecisionItemResource
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: Display name of the resource
      - `[Id <String>]`: Identifier of the resource
      - `[Type <String>]`: Type of resource.
Types include: Group, ServicePrincipal, DirectoryRole, AzureRole, AccessPackageAssignmentPolicy.
    - `[ResourceLink <String>]`: A link to the resource.
For example, https://graph.microsoft.com/v1.0/servicePrincipals/c86300f3-8695-4320-9f6e-32a2555f5ff8.
Supports $select.
Read-only.
    - `[ReviewedBy <IMicrosoftGraphUserIdentity>]`: userIdentity
    - `[ReviewedDateTime <DateTime?>]`: The timestamp when the review decision occurred.
Supports $select.
Read-only.
  - `[EndDateTime <DateTime?>]`: DateTime when review instance is scheduled to end.The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Supports $select.
Read-only.
  - `[FallbackReviewers <IMicrosoftGraphAccessReviewReviewerScope- `[]`>]`: This collection of reviewer scopes is used to define the list of fallback reviewers.
These fallback reviewers will be notified to take action if no users are found from the list of reviewers specified.
This could occur when either the group owner is specified as the reviewer but the group owner does not exist, or manager is specified as reviewer but a user's manager does not exist.
Supports $select.
    - `[Query <String>]`: The query specifying who will be the reviewer.
    - `[QueryRoot <String>]`: In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.
This property is only required if a relative query, for example, ./manager, is specified.
Possible value: decisions.
    - `[QueryType <String>]`: The type of query.
Examples include MicrosoftGraph and ARM.
  - `[Reviewers <IMicrosoftGraphAccessReviewReviewerScope- `[]`>]`: This collection of access review scopes is used to define who the reviewers are.
Supports $select.
For examples of options for assigning reviewers, see Assign reviewers to your access review definition using the Microsoft Graph API.
  - `[Scope <IMicrosoftGraphAccessReviewScope>]`: accessReviewScope
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Stages <IMicrosoftGraphAccessReviewStage- `[]`>]`: If the instance has multiple stages, this returns the collection of stages.
A new stage will only be created when the previous stage ends.
The existence, number, and settings of stages on a review instance are created based on the accessReviewStageSettings on the parent accessReviewScheduleDefinition.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[Decisions <IMicrosoftGraphAccessReviewInstanceDecisionItem- `[]`>]`: Each user reviewed in an accessReviewStage has a decision item representing if they were approved, denied, or not yet reviewed.
    - `[EndDateTime <DateTime?>]`: The date and time in ISO 8601 format and UTC time when the review stage is scheduled to end.
This property is the cumulative total of the durationInDays for all stages.
Read-only.
    - `[FallbackReviewers <IMicrosoftGraphAccessReviewReviewerScope- `[]`>]`: This collection of reviewer scopes is used to define the list of fallback reviewers.
These fallback reviewers are notified to take action if no users are found from the list of reviewers specified.
This could occur when either the group owner is specified as the reviewer but the group owner doesn't exist, or manager is specified as reviewer but a user's manager doesn't exist.
    - `[Reviewers <IMicrosoftGraphAccessReviewReviewerScope- `[]`>]`: This collection of access review scopes is used to define who the reviewers are.
For examples of options for assigning reviewers, see Assign reviewers to your access review definition using the Microsoft Graph API.
    - `[StartDateTime <DateTime?>]`: The date and time in ISO 8601 format and UTC time when the review stage is scheduled to start.
Read-only.
    - `[Status <String>]`: Specifies the status of an accessReviewStage.
Possible values: Initializing, NotStarted, Starting, InProgress, Completing, Completed, AutoReviewing, and AutoReviewed.
Supports $orderby, and $filter (eq only).
Read-only.
  - `[StartDateTime <DateTime?>]`: DateTime when review instance is scheduled to start.
May be in the future.
The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Supports $select.
Read-only.
  - `[Status <String>]`: Specifies the status of an accessReview.
Possible values: Initializing, NotStarted, Starting, InProgress, Completing, Completed, AutoReviewing, and AutoReviewed.
Supports $select, $orderby, and $filter (eq only).
Read-only.

REVIEWERS `<IMicrosoftGraphAccessReviewReviewerScope- `[]`>`: This collection of access review scopes is used to define who are the reviewers.
The reviewers property is only updatable if individual users are assigned as reviewers.
Required on create.
Supports $select.
For examples of options for assigning reviewers, see Assign reviewers to your access review definition using the Microsoft Graph API.
NOTE: The value of this property will be ignored if reviewers are assigned through the stageSettings property.
  - `[Query <String>]`: The query specifying who will be the reviewer.
  - `[QueryRoot <String>]`: In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.
This property is only required if a relative query, for example, ./manager, is specified.
Possible value: decisions.
  - `[QueryType <String>]`: The type of query.
Examples include MicrosoftGraph and ARM.

SETTINGS `<IMicrosoftGraphAccessReviewScheduleSettings>`: accessReviewScheduleSettings
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ApplyActions <IMicrosoftGraphAccessReviewApplyAction- `[]`>]`: Optional field.
Describes the  actions to take once a review is complete.
There are two types that are currently supported: removeAccessApplyAction (default) and disableAndDeleteUserApplyAction.
Field only needs to be specified in the case of disableAndDeleteUserApplyAction.
  - `[AutoApplyDecisionsEnabled <Boolean?>]`: Indicates whether decisions are automatically applied.
When set to false, an admin must apply the decisions manually once the reviewer completes the access review.
When set to true, decisions are applied automatically after the access review instance duration ends, whether or not the reviewers have responded.
Default value is false.
CAUTION: If both autoApplyDecisionsEnabled and defaultDecisionEnabled are true, all access for the principals to the resource risks being revoked if the reviewers fail to respond.
  - `[DecisionHistoriesForReviewersEnabled <Boolean?>]`: Indicates whether decisions on previous access review stages are available for reviewers on an accessReviewInstance with multiple subsequent stages.
If not provided, the default is disabled (false).
  - `[DefaultDecision <String>]`: Decision chosen if defaultDecisionEnabled is enabled.
Can be one of Approve, Deny, or Recommendation.
  - `[DefaultDecisionEnabled <Boolean?>]`: Indicates whether the default decision is enabled or disabled when reviewers do not respond.
Default value is false.
CAUTION: If both autoApplyDecisionsEnabled and defaultDecisionEnabled are true, all access for the principals to the resource risks being revoked if the reviewers fail to respond.
  - `[InstanceDurationInDays <Int32?>]`: Duration of an access review instance in days.
NOTE: If the stageSettings of the accessReviewScheduleDefinition object is defined, its durationInDays setting will be used instead of the value of this property.
  - `[JustificationRequiredOnApproval <Boolean?>]`: Indicates whether reviewers are required to provide justification with their decision.
Default value is false.
  - `[MailNotificationsEnabled <Boolean?>]`: Indicates whether emails are enabled or disabled.
Default value is false.
  - `[RecommendationInsightSettings <IMicrosoftGraphAccessReviewRecommendationInsightSetting- `[]`>]`: Optional.
Describes the types of insights that aid reviewers to make access review decisions.
NOTE: If the stageSettings of the accessReviewScheduleDefinition object is defined, its recommendationInsightSettings setting will be used instead of the value of this property.
  - `[RecommendationLookBackDuration <TimeSpan?>]`: Optional field.
Indicates the period of inactivity (with respect to the start date of the review instance) that recommendations will be configured from.
The recommendation will be to deny if the user is inactive during the look-back duration.
For reviews of groups and Microsoft Entra roles, any duration is accepted.
For reviews of applications, 30 days is the maximum duration.
If not specified, the duration is 30 days.
NOTE: If the stageSettings of the accessReviewScheduleDefinition object is defined, its recommendationLookBackDuration setting will be used instead of the value of this property.
  - `[RecommendationsEnabled <Boolean?>]`: Indicates whether decision recommendations are enabled or disabled.
NOTE: If the stageSettings of the accessReviewScheduleDefinition object is defined, its recommendationsEnabled setting will be used instead of the value of this property.
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
  - `[ReminderNotificationsEnabled <Boolean?>]`: Indicates whether reminders are enabled or disabled.
Default value is false.

STAGESETTINGS `<IMicrosoftGraphAccessReviewStageSettings- `[]`>`: Required only for a multi-stage access review to define the stages and their settings.
You can break down each review instance into up to three sequential stages, where each stage can have a different set of reviewers, fallback reviewers, and settings.
Stages are created sequentially based on the dependsOn property.
Optional.
When this property is defined, its settings are used instead of the corresponding settings in the accessReviewScheduleDefinition object and its settings, reviewers, and fallbackReviewers properties.
  - `[DecisionsThatWillMoveToNextStage <String- `[]`>]`: Indicate which decisions will go to the next stage.
Can be a subset of Approve, Deny, Recommendation, or NotReviewed.
If not provided, all decisions will go to the next stage.
Optional.
  - `[DependsOn <String- `[]`>]`: Defines the sequential or parallel order of the stages and depends on the stageId.
Only sequential stages are currently supported.
For example, if stageId is 2, then dependsOn must be 1.
If stageId is 1, don't specify dependsOn.
Required if stageId isn't 1.
  - `[DurationInDays <Int32?>]`: The duration of the stage.
Required.
NOTE: The cumulative value of this property across all stages  1.
Will override the instanceDurationInDays setting on the accessReviewScheduleDefinition object.
2.
Can't exceed the length of one recurrence.
That is, if the review recurs weekly, the cumulative durationInDays can't exceed 7.
  - `[FallbackReviewers <IMicrosoftGraphAccessReviewReviewerScope- `[]`>]`: If provided, the fallback reviewers are asked to complete a review if the primary reviewers don't exist.
For example, if managers are selected as reviewers and a principal under review doesn't have a manager in Microsoft Entra ID, the fallback reviewers are asked to review that principal.
NOTE: The value of this property overrides the corresponding setting on the accessReviewScheduleDefinition object.
    - `[Query <String>]`: The query specifying who will be the reviewer.
    - `[QueryRoot <String>]`: In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.
This property is only required if a relative query, for example, ./manager, is specified.
Possible value: decisions.
    - `[QueryType <String>]`: The type of query.
Examples include MicrosoftGraph and ARM.
  - `[RecommendationInsightSettings <IMicrosoftGraphAccessReviewRecommendationInsightSetting- `[]`>]`:
  - `[RecommendationsEnabled <Boolean?>]`: Indicates whether showing recommendations to reviewers is enabled.
Required.
NOTE: The value of this property overrides override the corresponding setting on the accessReviewScheduleDefinition object.
  - `[Reviewers <IMicrosoftGraphAccessReviewReviewerScope- `[]`>]`: Defines who the reviewers are.
If none is specified, the review is a self-review (users review their own access).
For examples of options for assigning reviewers, see Assign reviewers to your access review definition using the Microsoft Graph API.
NOTE: The value of this property overrides the corresponding setting on the accessReviewScheduleDefinition.
  - `[StageId <String>]`: Unique identifier of the accessReviewStageSettings object.
The stageId is used by the dependsOn property to indicate the order of the stages.
Required.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/set-mgidentitygovernanceaccessreviewdefinition](https://learn.microsoft.com/powershell/module/microsoft.graph.identity.governance/set-mgidentitygovernanceaccessreviewdefinition)

[https://learn.microsoft.com/graph/api/accessreviewscheduledefinition-update?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/accessreviewscheduledefinition-update?view=graph-rest-1.0)























