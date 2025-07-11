---
external help file: Microsoft.Graph.Beta.BackupRestore-help.xml
Module Name: Microsoft.Graph.Beta.BackupRestore
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.backuprestore/update-mgbetasolutionbackuprestoresharepointrestoresession
schema: 2.0.0
---

# Update-MgBetaSolutionBackupRestoreSharePointRestoreSession

## SYNOPSIS
Update the navigation property sharePointRestoreSessions in solutions

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgSolutionBackupRestoreSharePointRestoreSession](/powershell/module/Microsoft.Graph.BackupRestore/Update-MgSolutionBackupRestoreSharePointRestoreSession?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaSolutionBackupRestoreSharePointRestoreSession -SharePointRestoreSessionId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-CompletedDateTime <DateTime>]
 [-CreatedBy <IMicrosoftGraphIdentitySet>] [-CreatedDateTime <DateTime>] [-Error <IMicrosoftGraphPublicError>]
 [-Id <String>] [-LastModifiedBy <IMicrosoftGraphIdentitySet>] [-LastModifiedDateTime <DateTime>]
 [-RestoreJobType <String>] [-RestoreSessionArtifactCount <IMicrosoftGraphRestoreSessionArtifactCount>]
 [-SiteRestoreArtifacts <IMicrosoftGraphSiteRestoreArtifact[]>]
 [-SiteRestoreArtifactsBulkAdditionRequests <IMicrosoftGraphSiteRestoreArtifactsBulkAdditionRequest[]>]
 [-Status <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Update
```
Update-MgBetaSolutionBackupRestoreSharePointRestoreSession -SharePointRestoreSessionId <String>
 -BodyParameter <IMicrosoftGraphSharePointRestoreSession> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaSolutionBackupRestoreSharePointRestoreSession -InputObject <IBackupRestoreIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-CompletedDateTime <DateTime>]
 [-CreatedBy <IMicrosoftGraphIdentitySet>] [-CreatedDateTime <DateTime>] [-Error <IMicrosoftGraphPublicError>]
 [-Id <String>] [-LastModifiedBy <IMicrosoftGraphIdentitySet>] [-LastModifiedDateTime <DateTime>]
 [-RestoreJobType <String>] [-RestoreSessionArtifactCount <IMicrosoftGraphRestoreSessionArtifactCount>]
 [-SiteRestoreArtifacts <IMicrosoftGraphSiteRestoreArtifact[]>]
 [-SiteRestoreArtifactsBulkAdditionRequests <IMicrosoftGraphSiteRestoreArtifactsBulkAdditionRequest[]>]
 [-Status <String>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaSolutionBackupRestoreSharePointRestoreSession -InputObject <IBackupRestoreIdentity>
 -BodyParameter <IMicrosoftGraphSharePointRestoreSession> [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Update the navigation property sharePointRestoreSessions in solutions

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
sharePointRestoreSession
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphSharePointRestoreSession
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CompletedDateTime
The time of completion of the restore session.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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

### -CreatedBy
identitySet
To construct, see NOTES section for CREATEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentitySet
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CreatedDateTime
The time of creation of the restore session.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Error
publicError
To construct, see NOTES section for ERROR properties and create a hash table.

```yaml
Type: IMicrosoftGraphPublicError
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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
Type: IBackupRestoreIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -LastModifiedBy
identitySet
To construct, see NOTES section for LASTMODIFIEDBY properties and create a hash table.

```yaml
Type: IMicrosoftGraphIdentitySet
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedDateTime
Timestamp of the last modification of the restore session.

```yaml
Type: DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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

### -RestoreJobType
restoreJobType

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RestoreSessionArtifactCount
restoreSessionArtifactCount
To construct, see NOTES section for RESTORESESSIONARTIFACTCOUNT properties and create a hash table.

```yaml
Type: IMicrosoftGraphRestoreSessionArtifactCount
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SharePointRestoreSessionId
The unique identifier of sharePointRestoreSession

```yaml
Type: String
Parameter Sets: UpdateExpanded, Update
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SiteRestoreArtifacts
A collection of restore points and destination details that can be used to restore SharePoint sites.
To construct, see NOTES section for SITERESTOREARTIFACTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphSiteRestoreArtifact[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SiteRestoreArtifactsBulkAdditionRequests
A collection of SharePoint site URLs and destination details that can be used to restore SharePoint sites.
To construct, see NOTES section for SITERESTOREARTIFACTSBULKADDITIONREQUESTS properties and create a hash table.

```yaml
Type: IMicrosoftGraphSiteRestoreArtifactsBulkAdditionRequest[]
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Status
restoreSessionStatus

```yaml
Type: String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IBackupRestoreIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSharePointRestoreSession
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSharePointRestoreSession
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphSharePointRestoreSession>`: sharePointRestoreSession
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[CompletedDateTime <DateTime?>]`: The time of completion of the restore session.
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
      - `[Id <String>]`: The identifier of the identity.
This property is read-only.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[CreatedDateTime <DateTime?>]`: The time of creation of the restore session.
  - `[Error <IMicrosoftGraphPublicError>]`: publicError
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Code <String>]`: Represents the error code.
    - `[Details <IMicrosoftGraphPublicErrorDetail- `[]`>]`: Details of the error.
      - `[Code <String>]`: The error code.
      - `[Message <String>]`: The error message.
      - `[Target <String>]`: The target of the error.
    - `[InnerError <IMicrosoftGraphPublicInnerError>]`: publicInnerError
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Code <String>]`: The error code.
      - `[Details <IMicrosoftGraphPublicErrorDetail- `[]`>]`: A collection of error details.
      - `[Message <String>]`: The error message.
      - `[Target <String>]`: The target of the error.
    - `[Message <String>]`: A non-localized message for the developer.
    - `[Target <String>]`: The target of the error.
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[LastModifiedDateTime <DateTime?>]`: Timestamp of the last modification of the restore session.
  - `[RestoreJobType <String>]`: restoreJobType
  - `[RestoreSessionArtifactCount <IMicrosoftGraphRestoreSessionArtifactCount>]`: restoreSessionArtifactCount
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Completed <Int32?>]`: The number of artifacts whose restoration completed.
    - `[Failed <Int32?>]`: The number of artifacts whose restoration failed.
    - `[InProgress <Int32?>]`: The number of artifacts whose restoration is in progress.
    - `[Total <Int32?>]`: The number of artifacts present in the restore session.
  - `[Status <String>]`: restoreSessionStatus
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[SiteRestoreArtifacts <IMicrosoftGraphSiteRestoreArtifact- `[]`>]`: A collection of restore points and destination details that can be used to restore SharePoint sites.
    - `[CompletionDateTime <DateTime?>]`: The time when restoration of restore artifact is completed.
    - `[DestinationType <String>]`: destinationType
    - `[Error <IMicrosoftGraphPublicError>]`: publicError
    - `[RestorePoint <IMicrosoftGraphRestorePoint>]`: restorePoint
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[ExpirationDateTime <DateTime?>]`: Expiration date time of the restore point.
      - `[ProtectionDateTime <DateTime?>]`: Date time when the restore point was created.
      - `[ProtectionUnit <IMicrosoftGraphProtectionUnitBase>]`: protectionUnitBase
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Id <String>]`: The unique identifier for an entity.
Read-only.
        - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[CreatedDateTime <DateTime?>]`: The time of creation of the protection unit.
        - `[Error <IMicrosoftGraphPublicError>]`: publicError
        - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[LastModifiedDateTime <DateTime?>]`: Timestamp of the last modification of this protection unit.
        - `[PolicyId <String>]`: The unique identifier of the protection policy based on which protection unit was created.
        - `[ProtectionSources <String>]`: protectionSource
        - `[Status <String>]`: protectionUnitStatus
      - `[Tags <String>]`: restorePointTags
    - `[StartDateTime <DateTime?>]`: The time when restoration of restore artifact is started.
    - `[Status <String>]`: artifactRestoreStatus
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[RestoredSiteId <String>]`: The new site identifier if the value of the destinationType property is new, and the existing site ID if the value is inPlace.
  - `[SiteRestoreArtifactsBulkAdditionRequests <IMicrosoftGraphSiteRestoreArtifactsBulkAdditionRequest- `[]`>]`: A collection of SharePoint site URLs and destination details that can be used to restore SharePoint sites.
    - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[CreatedDateTime <DateTime?>]`: The time when the bulk request was created.
    - `[DestinationType <String>]`: destinationType
    - `[DisplayName <String>]`: Name of the addition request.
    - `[Error <IMicrosoftGraphPublicError>]`: publicError
    - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[LastModifiedDateTime <DateTime?>]`: Timestamp when this entity was last modified.
    - `[ProtectionTimePeriod <IMicrosoftGraphTimePeriod>]`: timePeriod
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[EndDateTime <DateTime?>]`: The date time of the end of the time period.
      - `[StartDateTime <DateTime?>]`: The date time of the start of the time period.
    - `[ProtectionUnitIds <String- `[]`>]`: Indicates which protection units to restore.
This property isn't implemented yet.
Future value; don't use.
    - `[RestorePointPreference <String>]`: restorePointPreference
    - `[Status <String>]`: restoreArtifactsBulkRequestStatus
    - `[Tags <String>]`: restorePointTags
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[SiteIds <String- `[]`>]`: The list of SharePoint site IDs that are added to the corresponding SharePoint restore session in a bulk operation.
This property isn't implemented yet.
Future value; don't use.
    - `[SiteWebUrls <String- `[]`>]`: The list of SharePoint site URLs that are added to the corresponding SharePoint restore session in a bulk operation.

CREATEDBY `<IMicrosoftGraphIdentitySet>`: identitySet
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Application <IMicrosoftGraphIdentity>]`: identity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
    - `[Id <String>]`: The identifier of the identity.
This property is read-only.
  - `[Device <IMicrosoftGraphIdentity>]`: identity
  - `[User <IMicrosoftGraphIdentity>]`: identity

ERROR `<IMicrosoftGraphPublicError>`: publicError
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Code <String>]`: Represents the error code.
  - `[Details <IMicrosoftGraphPublicErrorDetail- `[]`>]`: Details of the error.
    - `[Code <String>]`: The error code.
    - `[Message <String>]`: The error message.
    - `[Target <String>]`: The target of the error.
  - `[InnerError <IMicrosoftGraphPublicInnerError>]`: publicInnerError
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Code <String>]`: The error code.
    - `[Details <IMicrosoftGraphPublicErrorDetail- `[]`>]`: A collection of error details.
    - `[Message <String>]`: The error message.
    - `[Target <String>]`: The target of the error.
  - `[Message <String>]`: A non-localized message for the developer.
  - `[Target <String>]`: The target of the error.

INPUTOBJECT `<IBackupRestoreIdentity>`: Identity Parameter
  - `[DriveProtectionRuleId <String>]`: The unique identifier of driveProtectionRule
  - `[DriveProtectionUnitId <String>]`: The unique identifier of driveProtectionUnit
  - `[DriveProtectionUnitsBulkAdditionJobId <String>]`: The unique identifier of driveProtectionUnitsBulkAdditionJob
  - `[DriveRestoreArtifactId <String>]`: The unique identifier of driveRestoreArtifact
  - `[DriveRestoreArtifactsBulkAdditionRequestId <String>]`: The unique identifier of driveRestoreArtifactsBulkAdditionRequest
  - `[ExchangeProtectionPolicyId <String>]`: The unique identifier of exchangeProtectionPolicy
  - `[ExchangeRestoreSessionId <String>]`: The unique identifier of exchangeRestoreSession
  - `[GranularMailboxRestoreArtifactId <String>]`: The unique identifier of granularMailboxRestoreArtifact
  - `[MailboxProtectionRuleId <String>]`: The unique identifier of mailboxProtectionRule
  - `[MailboxProtectionUnitId <String>]`: The unique identifier of mailboxProtectionUnit
  - `[MailboxProtectionUnitsBulkAdditionJobId <String>]`: The unique identifier of mailboxProtectionUnitsBulkAdditionJob
  - `[MailboxRestoreArtifactId <String>]`: The unique identifier of mailboxRestoreArtifact
  - `[MailboxRestoreArtifactsBulkAdditionRequestId <String>]`: The unique identifier of mailboxRestoreArtifactsBulkAdditionRequest
  - `[OneDriveForBusinessProtectionPolicyId <String>]`: The unique identifier of oneDriveForBusinessProtectionPolicy
  - `[OneDriveForBusinessRestoreSessionId <String>]`: The unique identifier of oneDriveForBusinessRestoreSession
  - `[ProtectionPolicyBaseId <String>]`: The unique identifier of protectionPolicyBase
  - `[ProtectionUnitBaseId <String>]`: The unique identifier of protectionUnitBase
  - `[RestorePointId <String>]`: The unique identifier of restorePoint
  - `[RestoreSessionBaseId <String>]`: The unique identifier of restoreSessionBase
  - `[ServiceAppId <String>]`: The unique identifier of serviceApp
  - `[SharePointProtectionPolicyId <String>]`: The unique identifier of sharePointProtectionPolicy
  - `[SharePointRestoreSessionId <String>]`: The unique identifier of sharePointRestoreSession
  - `[SiteProtectionRuleId <String>]`: The unique identifier of siteProtectionRule
  - `[SiteProtectionUnitId <String>]`: The unique identifier of siteProtectionUnit
  - `[SiteProtectionUnitsBulkAdditionJobId <String>]`: The unique identifier of siteProtectionUnitsBulkAdditionJob
  - `[SiteRestoreArtifactId <String>]`: The unique identifier of siteRestoreArtifact
  - `[SiteRestoreArtifactsBulkAdditionRequestId <String>]`: The unique identifier of siteRestoreArtifactsBulkAdditionRequest

LASTMODIFIEDBY `<IMicrosoftGraphIdentitySet>`: identitySet
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Application <IMicrosoftGraphIdentity>]`: identity
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
    - `[Id <String>]`: The identifier of the identity.
This property is read-only.
  - `[Device <IMicrosoftGraphIdentity>]`: identity
  - `[User <IMicrosoftGraphIdentity>]`: identity

RESTORESESSIONARTIFACTCOUNT `<IMicrosoftGraphRestoreSessionArtifactCount>`: restoreSessionArtifactCount
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Completed <Int32?>]`: The number of artifacts whose restoration completed.
  - `[Failed <Int32?>]`: The number of artifacts whose restoration failed.
  - `[InProgress <Int32?>]`: The number of artifacts whose restoration is in progress.
  - `[Total <Int32?>]`: The number of artifacts present in the restore session.

SITERESTOREARTIFACTS `<IMicrosoftGraphSiteRestoreArtifact- `[]`>`: A collection of restore points and destination details that can be used to restore SharePoint sites.
  - `[CompletionDateTime <DateTime?>]`: The time when restoration of restore artifact is completed.
  - `[DestinationType <String>]`: destinationType
  - `[Error <IMicrosoftGraphPublicError>]`: publicError
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Code <String>]`: Represents the error code.
    - `[Details <IMicrosoftGraphPublicErrorDetail- `[]`>]`: Details of the error.
      - `[Code <String>]`: The error code.
      - `[Message <String>]`: The error message.
      - `[Target <String>]`: The target of the error.
    - `[InnerError <IMicrosoftGraphPublicInnerError>]`: publicInnerError
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Code <String>]`: The error code.
      - `[Details <IMicrosoftGraphPublicErrorDetail- `[]`>]`: A collection of error details.
      - `[Message <String>]`: The error message.
      - `[Target <String>]`: The target of the error.
    - `[Message <String>]`: A non-localized message for the developer.
    - `[Target <String>]`: The target of the error.
  - `[RestorePoint <IMicrosoftGraphRestorePoint>]`: restorePoint
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Id <String>]`: The unique identifier for an entity.
Read-only.
    - `[ExpirationDateTime <DateTime?>]`: Expiration date time of the restore point.
    - `[ProtectionDateTime <DateTime?>]`: Date time when the restore point was created.
    - `[ProtectionUnit <IMicrosoftGraphProtectionUnitBase>]`: protectionUnitBase
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Id <String>]`: The unique identifier for an entity.
Read-only.
      - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
        - `[(Any) <Object>]`: This indicates any property can be added to this object.
        - `[Application <IMicrosoftGraphIdentity>]`: identity
          - `[(Any) <Object>]`: This indicates any property can be added to this object.
          - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
          - `[Id <String>]`: The identifier of the identity.
This property is read-only.
        - `[Device <IMicrosoftGraphIdentity>]`: identity
        - `[User <IMicrosoftGraphIdentity>]`: identity
      - `[CreatedDateTime <DateTime?>]`: The time of creation of the protection unit.
      - `[Error <IMicrosoftGraphPublicError>]`: publicError
      - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
      - `[LastModifiedDateTime <DateTime?>]`: Timestamp of the last modification of this protection unit.
      - `[PolicyId <String>]`: The unique identifier of the protection policy based on which protection unit was created.
      - `[ProtectionSources <String>]`: protectionSource
      - `[Status <String>]`: protectionUnitStatus
    - `[Tags <String>]`: restorePointTags
  - `[StartDateTime <DateTime?>]`: The time when restoration of restore artifact is started.
  - `[Status <String>]`: artifactRestoreStatus
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[RestoredSiteId <String>]`: The new site identifier if the value of the destinationType property is new, and the existing site ID if the value is inPlace.

SITERESTOREARTIFACTSBULKADDITIONREQUESTS `<IMicrosoftGraphSiteRestoreArtifactsBulkAdditionRequest- `[]`>`: A collection of SharePoint site URLs and destination details that can be used to restore SharePoint sites.
  - `[CreatedBy <IMicrosoftGraphIdentitySet>]`: identitySet
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Application <IMicrosoftGraphIdentity>]`: identity
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[DisplayName <String>]`: The display name of the identity.
This property is read-only.
      - `[Id <String>]`: The identifier of the identity.
This property is read-only.
    - `[Device <IMicrosoftGraphIdentity>]`: identity
    - `[User <IMicrosoftGraphIdentity>]`: identity
  - `[CreatedDateTime <DateTime?>]`: The time when the bulk request was created.
  - `[DestinationType <String>]`: destinationType
  - `[DisplayName <String>]`: Name of the addition request.
  - `[Error <IMicrosoftGraphPublicError>]`: publicError
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Code <String>]`: Represents the error code.
    - `[Details <IMicrosoftGraphPublicErrorDetail- `[]`>]`: Details of the error.
      - `[Code <String>]`: The error code.
      - `[Message <String>]`: The error message.
      - `[Target <String>]`: The target of the error.
    - `[InnerError <IMicrosoftGraphPublicInnerError>]`: publicInnerError
      - `[(Any) <Object>]`: This indicates any property can be added to this object.
      - `[Code <String>]`: The error code.
      - `[Details <IMicrosoftGraphPublicErrorDetail- `[]`>]`: A collection of error details.
      - `[Message <String>]`: The error message.
      - `[Target <String>]`: The target of the error.
    - `[Message <String>]`: A non-localized message for the developer.
    - `[Target <String>]`: The target of the error.
  - `[LastModifiedBy <IMicrosoftGraphIdentitySet>]`: identitySet
  - `[LastModifiedDateTime <DateTime?>]`: Timestamp when this entity was last modified.
  - `[ProtectionTimePeriod <IMicrosoftGraphTimePeriod>]`: timePeriod
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[EndDateTime <DateTime?>]`: The date time of the end of the time period.
    - `[StartDateTime <DateTime?>]`: The date time of the start of the time period.
  - `[ProtectionUnitIds <String- `[]`>]`: Indicates which protection units to restore.
This property isn't implemented yet.
Future value; don't use.
  - `[RestorePointPreference <String>]`: restorePointPreference
  - `[Status <String>]`: restoreArtifactsBulkRequestStatus
  - `[Tags <String>]`: restorePointTags
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[SiteIds <String- `[]`>]`: The list of SharePoint site IDs that are added to the corresponding SharePoint restore session in a bulk operation.
This property isn't implemented yet.
Future value; don't use.
  - `[SiteWebUrls <String- `[]`>]`: The list of SharePoint site URLs that are added to the corresponding SharePoint restore session in a bulk operation.

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.backuprestore/update-mgbetasolutionbackuprestoresharepointrestoresession](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.backuprestore/update-mgbetasolutionbackuprestoresharepointrestoresession)
























