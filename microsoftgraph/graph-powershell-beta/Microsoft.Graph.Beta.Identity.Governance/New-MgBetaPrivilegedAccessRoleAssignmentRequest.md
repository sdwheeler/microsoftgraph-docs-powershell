---
external help file: Microsoft.Graph.Beta.Identity.Governance-help.xml
Module Name: Microsoft.Graph.Beta.Identity.Governance
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/new-mgbetaprivilegedaccessroleassignmentrequest
schema: 2.0.0
---

# New-MgBetaPrivilegedAccessRoleAssignmentRequest

## SYNOPSIS
Create new navigation property to roleAssignmentRequests for privilegedAccess

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaPrivilegedAccessRoleAssignmentRequest -PrivilegedAccessId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-AssignmentState <String>]
 [-Id <String>] [-LinkedEligibleRoleAssignmentId <String>] [-Reason <String>] [-RequestedDateTime <DateTime>]
 [-Resource <IMicrosoftGraphGovernanceResource>] [-ResourceId <String>]
 [-RoleDefinition <IMicrosoftGraphGovernanceRoleDefinition>] [-RoleDefinitionId <String>]
 [-Schedule <IMicrosoftGraphGovernanceSchedule>]
 [-Status <IMicrosoftGraphGovernanceRoleAssignmentRequestStatus>] [-Subject <IMicrosoftGraphGovernanceSubject>]
 [-SubjectId <String>] [-Type <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaPrivilegedAccessRoleAssignmentRequest -PrivilegedAccessId <String>
 -BodyParameter <IMicrosoftGraphGovernanceRoleAssignmentRequest> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgBetaPrivilegedAccessRoleAssignmentRequest -InputObject <IIdentityGovernanceIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-AssignmentState <String>]
 [-Id <String>] [-LinkedEligibleRoleAssignmentId <String>] [-Reason <String>] [-RequestedDateTime <DateTime>]
 [-Resource <IMicrosoftGraphGovernanceResource>] [-ResourceId <String>]
 [-RoleDefinition <IMicrosoftGraphGovernanceRoleDefinition>] [-RoleDefinitionId <String>]
 [-Schedule <IMicrosoftGraphGovernanceSchedule>]
 [-Status <IMicrosoftGraphGovernanceRoleAssignmentRequestStatus>] [-Subject <IMicrosoftGraphGovernanceSubject>]
 [-SubjectId <String>] [-Type <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgBetaPrivilegedAccessRoleAssignmentRequest -InputObject <IIdentityGovernanceIdentity>
 -BodyParameter <IMicrosoftGraphGovernanceRoleAssignmentRequest> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to roleAssignmentRequests for privilegedAccess

## EXAMPLES
### Example 1: Using the New-MgBetaPrivilegedAccessRoleAssignmentRequest Cmdlet
```powershell
Import-Module Microsoft.Graph.Beta.Identity.Governance
$params = @{
	RoleDefinitionId = "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d"
	ResourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5"
	SubjectId = "918e54be-12c4-4f4c-a6d3-2ee0e3661c51"
	AssignmentState = "Eligible"
	Type = "AdminAdd"
	Reason = "Assign an eligible role"
	Schedule = @{
		StartDateTime = [System.DateTime]::Parse("2018-05-12T23:37:43.356Z")
		EndDateTime = [System.DateTime]::Parse("2018-11-08T23:37:43.356Z")
		Type = "Once"
	}
}
New-MgBetaPrivilegedAccessRoleAssignmentRequest -PrivilegedAccessId $privilegedAccessId -BodyParameter $params
```
This example shows how to use the New-MgBetaPrivilegedAccessRoleAssignmentRequest Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).
### Example 2: Using the New-MgBetaPrivilegedAccessRoleAssignmentRequest Cmdlet
```powershell
Import-Module Microsoft.Graph.Beta.Identity.Governance
$params = @{
	RoleDefinitionId = "8b4d1d51-08e9-4254-b0a6-b16177aae376"
	ResourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5"
	SubjectId = "918e54be-12c4-4f4c-a6d3-2ee0e3661c51"
	AssignmentState = "Active"
	Type = "UserAdd"
	Reason = "Activate the owner role"
	Schedule = @{
		Type = "Once"
		StartDateTime = [System.DateTime]::Parse("2018-05-12T23:28:43.537Z")
		Duration = "PT9H"
	}
	LinkedEligibleRoleAssignmentId = "e327f4be-42a0-47a2-8579-0a39b025b394"
}
New-MgBetaPrivilegedAccessRoleAssignmentRequest -PrivilegedAccessId $privilegedAccessId -BodyParameter $params
```
This example shows how to use the New-MgBetaPrivilegedAccessRoleAssignmentRequest Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).
### Example 3: Using the New-MgBetaPrivilegedAccessRoleAssignmentRequest Cmdlet
```powershell
Import-Module Microsoft.Graph.Beta.Identity.Governance
$params = @{
	RoleDefinitionId = "bc75b4e6-7403-4243-bf2f-d1f6990be122"
	ResourceId = "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735"
	SubjectId = "918e54be-12c4-4f4c-a6d3-2ee0e3661c51"
	AssignmentState = "Active"
	Type = "UserRemove"
	Reason = "Deactivate the role"
	LinkedEligibleRoleAssignmentId = "cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
New-MgBetaPrivilegedAccessRoleAssignmentRequest -PrivilegedAccessId $privilegedAccessId -BodyParameter $params
```
This example shows how to use the New-MgBetaPrivilegedAccessRoleAssignmentRequest Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).
### Example 4: Using the New-MgBetaPrivilegedAccessRoleAssignmentRequest Cmdlet
```powershell
Import-Module Microsoft.Graph.Beta.Identity.Governance
$params = @{
	RoleDefinitionId = "65bb4622-61f5-4f25-9d75-d0e20cf92019"
	ResourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5"
	SubjectId = "74765671-9ca4-40d7-9e36-2f4a570608a6"
	AssignmentState = "Eligible"
	Type = "AdminRemove"
}
New-MgBetaPrivilegedAccessRoleAssignmentRequest -PrivilegedAccessId $privilegedAccessId -BodyParameter $params
```
This example shows how to use the New-MgBetaPrivilegedAccessRoleAssignmentRequest Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).
### Example 5: Using the New-MgBetaPrivilegedAccessRoleAssignmentRequest Cmdlet
```powershell
Import-Module Microsoft.Graph.Beta.Identity.Governance
$params = @{
	RoleDefinitionId = "70521f3e-3b95-4e51-b4d2-a2f485b02103"
	ResourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5"
	SubjectId = "1566d11d-d2b6-444a-a8de-28698682c445"
	AssignmentState = "Eligible"
	Type = "AdminUpdate"
	Schedule = @{
		Type = "Once"
		StartDateTime = [System.DateTime]::Parse("2018-03-08T05:42:45.317Z")
		EndDateTime = [System.DateTime]::Parse("2018-06-05T05:42:31.000Z")
	}
}
New-MgBetaPrivilegedAccessRoleAssignmentRequest -PrivilegedAccessId $privilegedAccessId -BodyParameter $params
```
This example shows how to use the New-MgBetaPrivilegedAccessRoleAssignmentRequest Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).
### Example 6: Using the New-MgBetaPrivilegedAccessRoleAssignmentRequest Cmdlet
```powershell
Import-Module Microsoft.Graph.Beta.Identity.Governance
$params = @{
	RoleDefinitionId = "0e88fd18-50f5-4ee1-9104-01c3ed910065"
	ResourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5"
	SubjectId = "74765671-9ca4-40d7-9e36-2f4a570608a6"
	AssignmentState = "Eligible"
	Type = "AdminExtend"
	Reason = "extend role assignment"
	Schedule = @{
		Type = "Once"
		StartDateTime = [System.DateTime]::Parse("2018-05-12T23:53:55.327Z")
		EndDateTime = [System.DateTime]::Parse("2018-08-10T23:53:55.327Z")
	}
}
New-MgBetaPrivilegedAccessRoleAssignmentRequest -PrivilegedAccessId $privilegedAccessId -BodyParameter $params
```
This example shows how to use the New-MgBetaPrivilegedAccessRoleAssignmentRequest Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AssignmentState
Required.
The state of the assignment.
The possible values are: Eligible (for eligible assignment), Active (if it is directly assigned), Active (by administrators, or activated on an eligible assignment by the users).

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
governanceRoleAssignmentRequest
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphGovernanceRoleAssignmentRequest
Parameter Sets: Create, CreateViaIdentity
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
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -LinkedEligibleRoleAssignmentId
If this is a request for role activation, it represents the id of the eligible assignment being referred; Otherwise, the value is null.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PrivilegedAccessId
The unique identifier of privilegedAccess

```yaml
Type: String
Parameter Sets: CreateExpanded, Create
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Reason
A message provided by users and administrators when create the request about why it is needed.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RequestedDateTime
Read-only.
The request create time.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z

```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Resource
governanceResource
To construct, see NOTES section for RESOURCE properties and create a hash table.

```yaml
Type: IMicrosoftGraphGovernanceResource
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceId
Required.
The unique identifier of the Azure resource that is associated with the role assignment request.
Azure resources can include subscriptions, resource groups, virtual machines, and SQL databases.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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

### -RoleDefinition
governanceRoleDefinition
To construct, see NOTES section for ROLEDEFINITION properties and create a hash table.

```yaml
Type: IMicrosoftGraphGovernanceRoleDefinition
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RoleDefinitionId
Required.
The identifier of the Azure role definition that the role assignment request is associated with.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Schedule
governanceSchedule
To construct, see NOTES section for SCHEDULE properties and create a hash table.

```yaml
Type: IMicrosoftGraphGovernanceSchedule
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Status
governanceRoleAssignmentRequestStatus
To construct, see NOTES section for STATUS properties and create a hash table.

```yaml
Type: IMicrosoftGraphGovernanceRoleAssignmentRequestStatus
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Subject
governanceSubject
To construct, see NOTES section for SUBJECT properties and create a hash table.

```yaml
Type: IMicrosoftGraphGovernanceSubject
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubjectId
Required.
The unique identifier of the principal or subject that the role assignment request is associated with.
Principals can be users, groups, or service principals.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Type
Required.
Representing the type of the operation on the role assignment.
The possible values are: AdminAdd , UserAdd , AdminUpdate , AdminRemove , UserRemove , UserExtend , AdminExtend , UserRenew , AdminRenew.

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IIdentityGovernanceIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphGovernanceRoleAssignmentRequest
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphGovernanceRoleAssignmentRequest
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphGovernanceRoleAssignmentRequest>`: governanceRoleAssignmentRequest
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[AssignmentState <String>]`: Required.
The state of the assignment.
The possible values are: Eligible (for eligible assignment),  Active (if it is directly assigned), Active (by administrators, or activated on an eligible assignment by the users).
  - `[LinkedEligibleRoleAssignmentId <String>]`: If this is a request for role activation, it represents the id of the eligible assignment being referred; Otherwise, the value is null.
  - `[Reason <String>]`: A message provided by users and administrators when create the request about why it is needed.
  - `[RequestedDateTime <DateTime?>]`: Read-only.
The request create time.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[Resource <IMicrosoftGraphGovernanceResource>]`: governanceResource
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: The display name of the resource.
    - `[ExternalId <String>]`: The external id of the resource, representing its original id in the external system.
For example, a subscription resource's external id can be '/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac'.
    - `[Parent <IMicrosoftGraphGovernanceResource>]`: governanceResource
    - `[RegisteredDateTime <DateTime?>]`: Represents the date time when the resource is registered in PIM.
    - `[RegisteredRoot <String>]`: The externalId of the resource's root scope that is registered in PIM.
The root scope can be the parent, grandparent, or higher ancestor resources.
    - `[RoleAssignmentRequests <IMicrosoftGraphGovernanceRoleAssignmentRequest- `[]`>]`: The collection of role assignment requests for the resource.
    - `[RoleAssignments <IMicrosoftGraphGovernanceRoleAssignment- `[]`>]`: The collection of role assignments for the resource.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AssignmentState <String>]`: The state of the assignment.
The value can be Eligible for eligible assignment or Active if it's directly assigned Active by administrators, or activated on an eligible assignment by the users.
      - `[EndDateTime <DateTime?>]`: For a non-permanent role assignment, this is the time when the role assignment is expired.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      - `[ExternalId <String>]`: The external ID the resource that is used to identify the role assignment in the provider.
      - `[LinkedEligibleRoleAssignment <IMicrosoftGraphGovernanceRoleAssignment>]`: governanceRoleAssignment
      - `[LinkedEligibleRoleAssignmentId <String>]`: If this is an active assignment and created due to activation on an eligible assignment, it represents the ID of that eligible assignment; Otherwise, the value is null.
      - `[MemberType <String>]`: The type of member.
The value can be: Inherited (if the role assignment is inherited from a parent resource scope), Group (if the role assignment isn't inherited, but comes from the membership of a group assignment), or User (if the role assignment isn't inherited or from a group assignment).
      - `[Resource <IMicrosoftGraphGovernanceResource>]`: governanceResource
      - `[ResourceId <String>]`: Required.
The ID of the resource that the role assignment is associated with.
      - `[RoleDefinition <IMicrosoftGraphGovernanceRoleDefinition>]`: governanceRoleDefinition
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[DisplayName <String>]`: The display name of the role definition.
        - `[ExternalId <String>]`: The external ID of the role definition.
        - `[Resource <IMicrosoftGraphGovernanceResource>]`: governanceResource
        - `[ResourceId <String>]`: Required.
The ID of the resource associated with the role definition.
        - `[RoleSetting <IMicrosoftGraphGovernanceRoleSetting>]`: governanceRoleSetting
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[Id <String>]`: The unique identifier for an entity.
Read-only.
          - `[AdminEligibleSettings <IMicrosoftGraphGovernanceRuleSetting- `[]`>]`: The rule settings that are evaluated when an administrator tries to add an eligible role assignment.
            - `[RuleIdentifier <String>]`: The id of the rule.
For example, ExpirationRule and MfaRule.
            - `[Setting <String>]`: The settings of the rule.
The value is a JSON string with a list of pairs in the format of ParameterName:ParameterValue.
For example, {'permanentAssignment':false,'maximumGrantPeriodInMinutes':129600}
          - `[AdminMemberSettings <IMicrosoftGraphGovernanceRuleSetting- `[]`>]`: The rule settings that are evaluated when an administrator tries to add a direct member role assignment.
          - `[IsDefault <Boolean?>]`: Read-only.
Indicate if the roleSetting is a default roleSetting
          - `[LastUpdatedBy <String>]`: Read-only.
The display name of the administrator who last updated the roleSetting.
          - `[LastUpdatedDateTime <DateTime?>]`: Read-only.
The time when the role setting was last updated.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
          - `[Resource <IMicrosoftGraphGovernanceResource>]`: governanceResource
          - `[ResourceId <String>]`: Required.
The id of the resource that the role setting is associated with.
          - `[RoleDefinition <IMicrosoftGraphGovernanceRoleDefinition>]`: governanceRoleDefinition
          - `[RoleDefinitionId <String>]`: Required.
The id of the role definition that the role setting is associated with.
          - `[UserEligibleSettings <IMicrosoftGraphGovernanceRuleSetting- `[]`>]`: The rule settings that are evaluated when a user tries to add an eligible role assignment.
The setting is not supported for now.
          - `[UserMemberSettings <IMicrosoftGraphGovernanceRuleSetting- `[]`>]`: The rule settings that are evaluated when a user tries to activate his role assignment.
        - `[TemplateId <String>]`: The unique identifier for the template.
      - `[RoleDefinitionId <String>]`: Required.
The ID of the role definition that the role assignment is associated with.
      - `[StartDateTime <DateTime?>]`: The start time of the role assignment.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      - `[Status <String>]`: 
      - `[Subject <IMicrosoftGraphGovernanceSubject>]`: governanceSubject
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[DisplayName <String>]`: The display name of the subject.
        - `[Email <String>]`: The email address of the user subject.
If the subject is in other types, it's empty.
        - `[PrincipalName <String>]`: The principal name of the user subject.
If the subject is in other types, it's empty.
        - `[Type <String>]`: The type of the subject.
The value can be User, Group, and ServicePrincipal.
      - `[SubjectId <String>]`: Required.
The ID of the subject that the role assignment is associated with.
    - `[RoleDefinitions <IMicrosoftGraphGovernanceRoleDefinition- `[]`>]`: The collection of role definitions for the resource.
    - `[RoleSettings <IMicrosoftGraphGovernanceRoleSetting- `[]`>]`: The collection of role settings for the resource.
    - `[Status <String>]`: The status of a given resource.
For example, it could represent whether the resource is locked or not (values: Active/Locked).
Note: This property may be extended in the future to support more scenarios.
    - `[Type <String>]`: Required.
Resource type.
For example, for Azure resources, the type could be 'Subscription', 'ResourceGroup', 'Microsoft.Sql/server', etc.
  - `[ResourceId <String>]`: Required.
The unique identifier of the Azure resource that is associated with the role assignment request.
Azure resources can include subscriptions, resource groups, virtual machines, and SQL databases.
  - `[RoleDefinition <IMicrosoftGraphGovernanceRoleDefinition>]`: governanceRoleDefinition
  - `[RoleDefinitionId <String>]`: Required.
The identifier of the Azure role definition that the role assignment request is associated with.
  - `[Schedule <IMicrosoftGraphGovernanceSchedule>]`: governanceSchedule
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Duration <TimeSpan?>]`: The duration of a role assignment.
It is in format of a TimeSpan.
    - `[EndDateTime <DateTime?>]`: The end time of the role assignment.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Note: if the value is null, it indicates a permanent assignment.
    - `[StartDateTime <DateTime?>]`: The start time of the role assignment.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[Type <String>]`: The role assignment schedule type.
Only Once is supported for now.
  - `[Status <IMicrosoftGraphGovernanceRoleAssignmentRequestStatus>]`: governanceRoleAssignmentRequestStatus
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Status <String>]`: The status of the role assignment request.
The value can be InProgress or Closed.
    - `[StatusDetails <IMicrosoftGraphKeyValue- `[]`>]`: The details of the status of the role assignment request.
It represents the evaluation results of different rules.
      - `[Key <String>]`: Key.
      - `[Value <String>]`: Value.
    - `[SubStatus <String>]`: The sub status of the role assignment request.
The values can be Accepted, PendingEvaluation, Granted, Denied, PendingProvisioning, Provisioned, PendingRevocation, Revoked, Canceled, Failed, PendingApprovalProvisioning, PendingApproval, FailedAsResourceIsLocked, PendingAdminDecision, AdminApproved, AdminDenied, TimedOut, and ProvisioningStarted.
  - `[Subject <IMicrosoftGraphGovernanceSubject>]`: governanceSubject
  - `[SubjectId <String>]`: Required.
The unique identifier of the principal or subject that the role assignment request is associated with.
Principals can be users, groups, or service principals.
  - `[Type <String>]`: Required.
Representing the type of the operation on the role assignment.
The possible values are: AdminAdd , UserAdd , AdminUpdate , AdminRemove , UserRemove , UserExtend , AdminExtend , UserRenew , AdminRenew.

INPUTOBJECT `<IIdentityGovernanceIdentity>`: Identity Parameter
  - `[AccessPackageAssignmentId <String>]`: The unique identifier of accessPackageAssignment
  - `[AccessPackageAssignmentPolicyId <String>]`: The unique identifier of accessPackageAssignmentPolicy
  - `[AccessPackageAssignmentRequestId <String>]`: The unique identifier of accessPackageAssignmentRequest
  - `[AccessPackageAssignmentResourceRoleId <String>]`: The unique identifier of accessPackageAssignmentResourceRole
  - `[AccessPackageCatalogId <String>]`: The unique identifier of accessPackageCatalog
  - `[AccessPackageId <String>]`: The unique identifier of accessPackage
  - `[AccessPackageId1 <String>]`: The unique identifier of accessPackage
  - `[AccessPackageResourceEnvironmentId <String>]`: The unique identifier of accessPackageResourceEnvironment
  - `[AccessPackageResourceId <String>]`: The unique identifier of accessPackageResource
  - `[AccessPackageResourceRequestId <String>]`: The unique identifier of accessPackageResourceRequest
  - `[AccessPackageResourceRoleId <String>]`: The unique identifier of accessPackageResourceRole
  - `[AccessPackageResourceRoleScopeId <String>]`: The unique identifier of accessPackageResourceRoleScope
  - `[AccessPackageResourceScopeId <String>]`: The unique identifier of accessPackageResourceScope
  - `[AccessPackageSubjectId <String>]`: The unique identifier of accessPackageSubject
  - `[AccessReviewDecisionId <String>]`: The unique identifier of accessReviewDecision
  - `[AccessReviewHistoryDefinitionId <String>]`: The unique identifier of accessReviewHistoryDefinition
  - `[AccessReviewHistoryInstanceId <String>]`: The unique identifier of accessReviewHistoryInstance
  - `[AccessReviewId <String>]`: The unique identifier of accessReview
  - `[AccessReviewId1 <String>]`: The unique identifier of accessReview
  - `[AccessReviewInstanceDecisionItemId <String>]`: The unique identifier of accessReviewInstanceDecisionItem
  - `[AccessReviewInstanceDecisionItemId1 <String>]`: The unique identifier of accessReviewInstanceDecisionItem
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
  - `[ApprovalStepId <String>]`: The unique identifier of approvalStep
  - `[BusinessFlowTemplateId <String>]`: The unique identifier of businessFlowTemplate
  - `[ConnectedOrganizationId <String>]`: The unique identifier of connectedOrganization
  - `[CustomAccessPackageWorkflowExtensionId <String>]`: The unique identifier of customAccessPackageWorkflowExtension
  - `[CustomCalloutExtensionId <String>]`: The unique identifier of customCalloutExtension
  - `[CustomExtensionHandlerId <String>]`: The unique identifier of customExtensionHandler
  - `[CustomExtensionStageSettingId <String>]`: The unique identifier of customExtensionStageSetting
  - `[CustomTaskExtensionId <String>]`: The unique identifier of customTaskExtension
  - `[DirectoryObjectId <String>]`: The unique identifier of directoryObject
  - `[EndDateTime <DateTime?>]`: Usage: endDateTime={endDateTime}
  - `[FindingId <String>]`: The unique identifier of finding
  - `[GovernanceInsightId <String>]`: The unique identifier of governanceInsight
  - `[GovernanceResourceId <String>]`: The unique identifier of governanceResource
  - `[GovernanceRoleAssignmentId <String>]`: The unique identifier of governanceRoleAssignment
  - `[GovernanceRoleAssignmentRequestId <String>]`: The unique identifier of governanceRoleAssignmentRequest
  - `[GovernanceRoleDefinitionId <String>]`: The unique identifier of governanceRoleDefinition
  - `[GovernanceRoleSettingId <String>]`: The unique identifier of governanceRoleSetting
  - `[IncompatibleAccessPackageId <String>]`: Usage: incompatibleAccessPackageId='{incompatibleAccessPackageId}'
  - `[LongRunningOperationId <String>]`: The unique identifier of longRunningOperation
  - `[ObjectId <String>]`: Alternate key of accessPackageSubject
  - `[On <String>]`: Usage: on='{on}'
  - `[PermissionsCreepIndexDistributionId <String>]`: The unique identifier of permissionsCreepIndexDistribution
  - `[PermissionsRequestChangeId <String>]`: The unique identifier of permissionsRequestChange
  - `[PrivilegedAccessGroupAssignmentScheduleId <String>]`: The unique identifier of privilegedAccessGroupAssignmentSchedule
  - `[PrivilegedAccessGroupAssignmentScheduleInstanceId <String>]`: The unique identifier of privilegedAccessGroupAssignmentScheduleInstance
  - `[PrivilegedAccessGroupAssignmentScheduleRequestId <String>]`: The unique identifier of privilegedAccessGroupAssignmentScheduleRequest
  - `[PrivilegedAccessGroupEligibilityScheduleId <String>]`: The unique identifier of privilegedAccessGroupEligibilitySchedule
  - `[PrivilegedAccessGroupEligibilityScheduleInstanceId <String>]`: The unique identifier of privilegedAccessGroupEligibilityScheduleInstance
  - `[PrivilegedAccessGroupEligibilityScheduleRequestId <String>]`: The unique identifier of privilegedAccessGroupEligibilityScheduleRequest
  - `[PrivilegedAccessId <String>]`: The unique identifier of privilegedAccess
  - `[PrivilegedApprovalId <String>]`: The unique identifier of privilegedApproval
  - `[PrivilegedOperationEventId <String>]`: The unique identifier of privilegedOperationEvent
  - `[PrivilegedRoleAssignmentId <String>]`: The unique identifier of privilegedRoleAssignment
  - `[PrivilegedRoleAssignmentId1 <String>]`: The unique identifier of privilegedRoleAssignment
  - `[PrivilegedRoleAssignmentRequestId <String>]`: The unique identifier of privilegedRoleAssignmentRequest
  - `[PrivilegedRoleId <String>]`: The unique identifier of privilegedRole
  - `[ProgramControlId <String>]`: The unique identifier of programControl
  - `[ProgramControlId1 <String>]`: The unique identifier of programControl
  - `[ProgramControlTypeId <String>]`: The unique identifier of programControlType
  - `[ProgramId <String>]`: The unique identifier of program
  - `[RbacApplicationId <String>]`: The unique identifier of rbacApplication
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
  - `[UnifiedRoleManagementAlertConfigurationId <String>]`: The unique identifier of unifiedRoleManagementAlertConfiguration
  - `[UnifiedRoleManagementAlertDefinitionId <String>]`: The unique identifier of unifiedRoleManagementAlertDefinition
  - `[UnifiedRoleManagementAlertId <String>]`: The unique identifier of unifiedRoleManagementAlert
  - `[UnifiedRoleManagementAlertIncidentId <String>]`: The unique identifier of unifiedRoleManagementAlertIncident
  - `[UniqueName <String>]`: Alternate key of accessPackageCatalog
  - `[UserConsentRequestId <String>]`: The unique identifier of userConsentRequest
  - `[UserId <String>]`: The unique identifier of user
  - `[UserProcessingResultId <String>]`: The unique identifier of userProcessingResult
  - `[WorkflowId <String>]`: The unique identifier of workflow
  - `[WorkflowTemplateId <String>]`: The unique identifier of workflowTemplate
  - `[WorkflowVersionNumber <Int32?>]`: The unique identifier of workflowVersion

RESOURCE `<IMicrosoftGraphGovernanceResource>`: governanceResource
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DisplayName <String>]`: The display name of the resource.
  - `[ExternalId <String>]`: The external id of the resource, representing its original id in the external system.
For example, a subscription resource's external id can be '/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac'.
  - `[Parent <IMicrosoftGraphGovernanceResource>]`: governanceResource
  - `[RegisteredDateTime <DateTime?>]`: Represents the date time when the resource is registered in PIM.
  - `[RegisteredRoot <String>]`: The externalId of the resource's root scope that is registered in PIM.
The root scope can be the parent, grandparent, or higher ancestor resources.
  - `[RoleAssignmentRequests <IMicrosoftGraphGovernanceRoleAssignmentRequest- `[]`>]`: The collection of role assignment requests for the resource.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AssignmentState <String>]`: Required.
The state of the assignment.
The possible values are: Eligible (for eligible assignment),  Active (if it is directly assigned), Active (by administrators, or activated on an eligible assignment by the users).
    - `[LinkedEligibleRoleAssignmentId <String>]`: If this is a request for role activation, it represents the id of the eligible assignment being referred; Otherwise, the value is null.
    - `[Reason <String>]`: A message provided by users and administrators when create the request about why it is needed.
    - `[RequestedDateTime <DateTime?>]`: Read-only.
The request create time.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[Resource <IMicrosoftGraphGovernanceResource>]`: governanceResource
    - `[ResourceId <String>]`: Required.
The unique identifier of the Azure resource that is associated with the role assignment request.
Azure resources can include subscriptions, resource groups, virtual machines, and SQL databases.
    - `[RoleDefinition <IMicrosoftGraphGovernanceRoleDefinition>]`: governanceRoleDefinition
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[DisplayName <String>]`: The display name of the role definition.
      - `[ExternalId <String>]`: The external ID of the role definition.
      - `[Resource <IMicrosoftGraphGovernanceResource>]`: governanceResource
      - `[ResourceId <String>]`: Required.
The ID of the resource associated with the role definition.
      - `[RoleSetting <IMicrosoftGraphGovernanceRoleSetting>]`: governanceRoleSetting
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[AdminEligibleSettings <IMicrosoftGraphGovernanceRuleSetting- `[]`>]`: The rule settings that are evaluated when an administrator tries to add an eligible role assignment.
          - `[RuleIdentifier <String>]`: The id of the rule.
For example, ExpirationRule and MfaRule.
          - `[Setting <String>]`: The settings of the rule.
The value is a JSON string with a list of pairs in the format of ParameterName:ParameterValue.
For example, {'permanentAssignment':false,'maximumGrantPeriodInMinutes':129600}
        - `[AdminMemberSettings <IMicrosoftGraphGovernanceRuleSetting- `[]`>]`: The rule settings that are evaluated when an administrator tries to add a direct member role assignment.
        - `[IsDefault <Boolean?>]`: Read-only.
Indicate if the roleSetting is a default roleSetting
        - `[LastUpdatedBy <String>]`: Read-only.
The display name of the administrator who last updated the roleSetting.
        - `[LastUpdatedDateTime <DateTime?>]`: Read-only.
The time when the role setting was last updated.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
        - `[Resource <IMicrosoftGraphGovernanceResource>]`: governanceResource
        - `[ResourceId <String>]`: Required.
The id of the resource that the role setting is associated with.
        - `[RoleDefinition <IMicrosoftGraphGovernanceRoleDefinition>]`: governanceRoleDefinition
        - `[RoleDefinitionId <String>]`: Required.
The id of the role definition that the role setting is associated with.
        - `[UserEligibleSettings <IMicrosoftGraphGovernanceRuleSetting- `[]`>]`: The rule settings that are evaluated when a user tries to add an eligible role assignment.
The setting is not supported for now.
        - `[UserMemberSettings <IMicrosoftGraphGovernanceRuleSetting- `[]`>]`: The rule settings that are evaluated when a user tries to activate his role assignment.
      - `[TemplateId <String>]`: The unique identifier for the template.
    - `[RoleDefinitionId <String>]`: Required.
The identifier of the Azure role definition that the role assignment request is associated with.
    - `[Schedule <IMicrosoftGraphGovernanceSchedule>]`: governanceSchedule
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Duration <TimeSpan?>]`: The duration of a role assignment.
It is in format of a TimeSpan.
      - `[EndDateTime <DateTime?>]`: The end time of the role assignment.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Note: if the value is null, it indicates a permanent assignment.
      - `[StartDateTime <DateTime?>]`: The start time of the role assignment.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      - `[Type <String>]`: The role assignment schedule type.
Only Once is supported for now.
    - `[Status <IMicrosoftGraphGovernanceRoleAssignmentRequestStatus>]`: governanceRoleAssignmentRequestStatus
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Status <String>]`: The status of the role assignment request.
The value can be InProgress or Closed.
      - `[StatusDetails <IMicrosoftGraphKeyValue- `[]`>]`: The details of the status of the role assignment request.
It represents the evaluation results of different rules.
        - `[Key <String>]`: Key.
        - `[Value <String>]`: Value.
      - `[SubStatus <String>]`: The sub status of the role assignment request.
The values can be Accepted, PendingEvaluation, Granted, Denied, PendingProvisioning, Provisioned, PendingRevocation, Revoked, Canceled, Failed, PendingApprovalProvisioning, PendingApproval, FailedAsResourceIsLocked, PendingAdminDecision, AdminApproved, AdminDenied, TimedOut, and ProvisioningStarted.
    - `[Subject <IMicrosoftGraphGovernanceSubject>]`: governanceSubject
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[DisplayName <String>]`: The display name of the subject.
      - `[Email <String>]`: The email address of the user subject.
If the subject is in other types, it's empty.
      - `[PrincipalName <String>]`: The principal name of the user subject.
If the subject is in other types, it's empty.
      - `[Type <String>]`: The type of the subject.
The value can be User, Group, and ServicePrincipal.
    - `[SubjectId <String>]`: Required.
The unique identifier of the principal or subject that the role assignment request is associated with.
Principals can be users, groups, or service principals.
    - `[Type <String>]`: Required.
Representing the type of the operation on the role assignment.
The possible values are: AdminAdd , UserAdd , AdminUpdate , AdminRemove , UserRemove , UserExtend , AdminExtend , UserRenew , AdminRenew.
  - `[RoleAssignments <IMicrosoftGraphGovernanceRoleAssignment- `[]`>]`: The collection of role assignments for the resource.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[AssignmentState <String>]`: The state of the assignment.
The value can be Eligible for eligible assignment or Active if it's directly assigned Active by administrators, or activated on an eligible assignment by the users.
    - `[EndDateTime <DateTime?>]`: For a non-permanent role assignment, this is the time when the role assignment is expired.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[ExternalId <String>]`: The external ID the resource that is used to identify the role assignment in the provider.
    - `[LinkedEligibleRoleAssignment <IMicrosoftGraphGovernanceRoleAssignment>]`: governanceRoleAssignment
    - `[LinkedEligibleRoleAssignmentId <String>]`: If this is an active assignment and created due to activation on an eligible assignment, it represents the ID of that eligible assignment; Otherwise, the value is null.
    - `[MemberType <String>]`: The type of member.
The value can be: Inherited (if the role assignment is inherited from a parent resource scope), Group (if the role assignment isn't inherited, but comes from the membership of a group assignment), or User (if the role assignment isn't inherited or from a group assignment).
    - `[Resource <IMicrosoftGraphGovernanceResource>]`: governanceResource
    - `[ResourceId <String>]`: Required.
The ID of the resource that the role assignment is associated with.
    - `[RoleDefinition <IMicrosoftGraphGovernanceRoleDefinition>]`: governanceRoleDefinition
    - `[RoleDefinitionId <String>]`: Required.
The ID of the role definition that the role assignment is associated with.
    - `[StartDateTime <DateTime?>]`: The start time of the role assignment.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
    - `[Status <String>]`: 
    - `[Subject <IMicrosoftGraphGovernanceSubject>]`: governanceSubject
    - `[SubjectId <String>]`: Required.
The ID of the subject that the role assignment is associated with.
  - `[RoleDefinitions <IMicrosoftGraphGovernanceRoleDefinition- `[]`>]`: The collection of role definitions for the resource.
  - `[RoleSettings <IMicrosoftGraphGovernanceRoleSetting- `[]`>]`: The collection of role settings for the resource.
  - `[Status <String>]`: The status of a given resource.
For example, it could represent whether the resource is locked or not (values: Active/Locked).
Note: This property may be extended in the future to support more scenarios.
  - `[Type <String>]`: Required.
Resource type.
For example, for Azure resources, the type could be 'Subscription', 'ResourceGroup', 'Microsoft.Sql/server', etc.

ROLEDEFINITION `<IMicrosoftGraphGovernanceRoleDefinition>`: governanceRoleDefinition
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DisplayName <String>]`: The display name of the role definition.
  - `[ExternalId <String>]`: The external ID of the role definition.
  - `[Resource <IMicrosoftGraphGovernanceResource>]`: governanceResource
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[DisplayName <String>]`: The display name of the resource.
    - `[ExternalId <String>]`: The external id of the resource, representing its original id in the external system.
For example, a subscription resource's external id can be '/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac'.
    - `[Parent <IMicrosoftGraphGovernanceResource>]`: governanceResource
    - `[RegisteredDateTime <DateTime?>]`: Represents the date time when the resource is registered in PIM.
    - `[RegisteredRoot <String>]`: The externalId of the resource's root scope that is registered in PIM.
The root scope can be the parent, grandparent, or higher ancestor resources.
    - `[RoleAssignmentRequests <IMicrosoftGraphGovernanceRoleAssignmentRequest- `[]`>]`: The collection of role assignment requests for the resource.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AssignmentState <String>]`: Required.
The state of the assignment.
The possible values are: Eligible (for eligible assignment),  Active (if it is directly assigned), Active (by administrators, or activated on an eligible assignment by the users).
      - `[LinkedEligibleRoleAssignmentId <String>]`: If this is a request for role activation, it represents the id of the eligible assignment being referred; Otherwise, the value is null.
      - `[Reason <String>]`: A message provided by users and administrators when create the request about why it is needed.
      - `[RequestedDateTime <DateTime?>]`: Read-only.
The request create time.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      - `[Resource <IMicrosoftGraphGovernanceResource>]`: governanceResource
      - `[ResourceId <String>]`: Required.
The unique identifier of the Azure resource that is associated with the role assignment request.
Azure resources can include subscriptions, resource groups, virtual machines, and SQL databases.
      - `[RoleDefinition <IMicrosoftGraphGovernanceRoleDefinition>]`: governanceRoleDefinition
      - `[RoleDefinitionId <String>]`: Required.
The identifier of the Azure role definition that the role assignment request is associated with.
      - `[Schedule <IMicrosoftGraphGovernanceSchedule>]`: governanceSchedule
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Duration <TimeSpan?>]`: The duration of a role assignment.
It is in format of a TimeSpan.
        - `[EndDateTime <DateTime?>]`: The end time of the role assignment.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Note: if the value is null, it indicates a permanent assignment.
        - `[StartDateTime <DateTime?>]`: The start time of the role assignment.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
        - `[Type <String>]`: The role assignment schedule type.
Only Once is supported for now.
      - `[Status <IMicrosoftGraphGovernanceRoleAssignmentRequestStatus>]`: governanceRoleAssignmentRequestStatus
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Status <String>]`: The status of the role assignment request.
The value can be InProgress or Closed.
        - `[StatusDetails <IMicrosoftGraphKeyValue- `[]`>]`: The details of the status of the role assignment request.
It represents the evaluation results of different rules.
          - `[Key <String>]`: Key.
          - `[Value <String>]`: Value.
        - `[SubStatus <String>]`: The sub status of the role assignment request.
The values can be Accepted, PendingEvaluation, Granted, Denied, PendingProvisioning, Provisioned, PendingRevocation, Revoked, Canceled, Failed, PendingApprovalProvisioning, PendingApproval, FailedAsResourceIsLocked, PendingAdminDecision, AdminApproved, AdminDenied, TimedOut, and ProvisioningStarted.
      - `[Subject <IMicrosoftGraphGovernanceSubject>]`: governanceSubject
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[DisplayName <String>]`: The display name of the subject.
        - `[Email <String>]`: The email address of the user subject.
If the subject is in other types, it's empty.
        - `[PrincipalName <String>]`: The principal name of the user subject.
If the subject is in other types, it's empty.
        - `[Type <String>]`: The type of the subject.
The value can be User, Group, and ServicePrincipal.
      - `[SubjectId <String>]`: Required.
The unique identifier of the principal or subject that the role assignment request is associated with.
Principals can be users, groups, or service principals.
      - `[Type <String>]`: Required.
Representing the type of the operation on the role assignment.
The possible values are: AdminAdd , UserAdd , AdminUpdate , AdminRemove , UserRemove , UserExtend , AdminExtend , UserRenew , AdminRenew.
    - `[RoleAssignments <IMicrosoftGraphGovernanceRoleAssignment- `[]`>]`: The collection of role assignments for the resource.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AssignmentState <String>]`: The state of the assignment.
The value can be Eligible for eligible assignment or Active if it's directly assigned Active by administrators, or activated on an eligible assignment by the users.
      - `[EndDateTime <DateTime?>]`: For a non-permanent role assignment, this is the time when the role assignment is expired.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      - `[ExternalId <String>]`: The external ID the resource that is used to identify the role assignment in the provider.
      - `[LinkedEligibleRoleAssignment <IMicrosoftGraphGovernanceRoleAssignment>]`: governanceRoleAssignment
      - `[LinkedEligibleRoleAssignmentId <String>]`: If this is an active assignment and created due to activation on an eligible assignment, it represents the ID of that eligible assignment; Otherwise, the value is null.
      - `[MemberType <String>]`: The type of member.
The value can be: Inherited (if the role assignment is inherited from a parent resource scope), Group (if the role assignment isn't inherited, but comes from the membership of a group assignment), or User (if the role assignment isn't inherited or from a group assignment).
      - `[Resource <IMicrosoftGraphGovernanceResource>]`: governanceResource
      - `[ResourceId <String>]`: Required.
The ID of the resource that the role assignment is associated with.
      - `[RoleDefinition <IMicrosoftGraphGovernanceRoleDefinition>]`: governanceRoleDefinition
      - `[RoleDefinitionId <String>]`: Required.
The ID of the role definition that the role assignment is associated with.
      - `[StartDateTime <DateTime?>]`: The start time of the role assignment.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      - `[Status <String>]`: 
      - `[Subject <IMicrosoftGraphGovernanceSubject>]`: governanceSubject
      - `[SubjectId <String>]`: Required.
The ID of the subject that the role assignment is associated with.
    - `[RoleDefinitions <IMicrosoftGraphGovernanceRoleDefinition- `[]`>]`: The collection of role definitions for the resource.
    - `[RoleSettings <IMicrosoftGraphGovernanceRoleSetting- `[]`>]`: The collection of role settings for the resource.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[AdminEligibleSettings <IMicrosoftGraphGovernanceRuleSetting- `[]`>]`: The rule settings that are evaluated when an administrator tries to add an eligible role assignment.
        - `[RuleIdentifier <String>]`: The id of the rule.
For example, ExpirationRule and MfaRule.
        - `[Setting <String>]`: The settings of the rule.
The value is a JSON string with a list of pairs in the format of ParameterName:ParameterValue.
For example, {'permanentAssignment':false,'maximumGrantPeriodInMinutes':129600}
      - `[AdminMemberSettings <IMicrosoftGraphGovernanceRuleSetting- `[]`>]`: The rule settings that are evaluated when an administrator tries to add a direct member role assignment.
      - `[IsDefault <Boolean?>]`: Read-only.
Indicate if the roleSetting is a default roleSetting
      - `[LastUpdatedBy <String>]`: Read-only.
The display name of the administrator who last updated the roleSetting.
      - `[LastUpdatedDateTime <DateTime?>]`: Read-only.
The time when the role setting was last updated.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
      - `[Resource <IMicrosoftGraphGovernanceResource>]`: governanceResource
      - `[ResourceId <String>]`: Required.
The id of the resource that the role setting is associated with.
      - `[RoleDefinition <IMicrosoftGraphGovernanceRoleDefinition>]`: governanceRoleDefinition
      - `[RoleDefinitionId <String>]`: Required.
The id of the role definition that the role setting is associated with.
      - `[UserEligibleSettings <IMicrosoftGraphGovernanceRuleSetting- `[]`>]`: The rule settings that are evaluated when a user tries to add an eligible role assignment.
The setting is not supported for now.
      - `[UserMemberSettings <IMicrosoftGraphGovernanceRuleSetting- `[]`>]`: The rule settings that are evaluated when a user tries to activate his role assignment.
    - `[Status <String>]`: The status of a given resource.
For example, it could represent whether the resource is locked or not (values: Active/Locked).
Note: This property may be extended in the future to support more scenarios.
    - `[Type <String>]`: Required.
Resource type.
For example, for Azure resources, the type could be 'Subscription', 'ResourceGroup', 'Microsoft.Sql/server', etc.
  - `[ResourceId <String>]`: Required.
The ID of the resource associated with the role definition.
  - `[RoleSetting <IMicrosoftGraphGovernanceRoleSetting>]`: governanceRoleSetting
  - `[TemplateId <String>]`: The unique identifier for the template.

SCHEDULE `<IMicrosoftGraphGovernanceSchedule>`: governanceSchedule
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Duration <TimeSpan?>]`: The duration of a role assignment.
It is in format of a TimeSpan.
  - `[EndDateTime <DateTime?>]`: The end time of the role assignment.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z.
Note: if the value is null, it indicates a permanent assignment.
  - `[StartDateTime <DateTime?>]`: The start time of the role assignment.
The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.
For example, midnight UTC on Jan 1, 2014 is 2014-01-01T00:00:00Z
  - `[Type <String>]`: The role assignment schedule type.
Only Once is supported for now.

STATUS `<IMicrosoftGraphGovernanceRoleAssignmentRequestStatus>`: governanceRoleAssignmentRequestStatus
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Status <String>]`: The status of the role assignment request.
The value can be InProgress or Closed.
  - `[StatusDetails <IMicrosoftGraphKeyValue- `[]`>]`: The details of the status of the role assignment request.
It represents the evaluation results of different rules.
    - `[Key <String>]`: Key.
    - `[Value <String>]`: Value.
  - `[SubStatus <String>]`: The sub status of the role assignment request.
The values can be Accepted, PendingEvaluation, Granted, Denied, PendingProvisioning, Provisioned, PendingRevocation, Revoked, Canceled, Failed, PendingApprovalProvisioning, PendingApproval, FailedAsResourceIsLocked, PendingAdminDecision, AdminApproved, AdminDenied, TimedOut, and ProvisioningStarted.

SUBJECT `<IMicrosoftGraphGovernanceSubject>`: governanceSubject
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[DisplayName <String>]`: The display name of the subject.
  - `[Email <String>]`: The email address of the user subject.
If the subject is in other types, it's empty.
  - `[PrincipalName <String>]`: The principal name of the user subject.
If the subject is in other types, it's empty.
  - `[Type <String>]`: The type of the subject.
The value can be User, Group, and ServicePrincipal.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/new-mgbetaprivilegedaccessroleassignmentrequest](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.governance/new-mgbetaprivilegedaccessroleassignmentrequest)























