---
external help file: Microsoft.Graph.BackupRestore-help.xml
Module Name: Microsoft.Graph.BackupRestore
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.backuprestore/get-mgsolutionbackuprestorepointprotectionunit
schema: 2.0.0
---

# Get-MgSolutionBackupRestorePointProtectionUnit

## SYNOPSIS
The site, drive, or mailbox units that are protected under a protection policy.

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaSolutionBackupRestorePointProtectionUnit](/powershell/module/Microsoft.Graph.Beta.BackupRestore/Get-MgBetaSolutionBackupRestorePointProtectionUnit?view=graph-powershell-beta)

## SYNTAX

### Get (Default)
```
Get-MgSolutionBackupRestorePointProtectionUnit -RestorePointId <String> [-ExpandProperty <String[]>]
 [-Property <String[]>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgSolutionBackupRestorePointProtectionUnit -InputObject <IBackupRestoreIdentity>
 [-ExpandProperty <String[]>] [-Property <String[]>] [-ResponseHeadersVariable <String>]
 [-Headers <IDictionary>] [<CommonParameters>]
```

## DESCRIPTION
The site, drive, or mailbox units that are protected under a protection policy.

## EXAMPLES

## PARAMETERS

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
Type: IBackupRestoreIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

### -RestorePointId
The unique identifier of restorePoint

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IBackupRestoreIdentity
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.PowerShell.Models.IMicrosoftGraphProtectionUnitBase
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<IBackupRestoreIdentity>`: Identity Parameter
  - `[DriveProtectionRuleId <String>]`: The unique identifier of driveProtectionRule
  - `[DriveProtectionUnitId <String>]`: The unique identifier of driveProtectionUnit
  - `[DriveRestoreArtifactId <String>]`: The unique identifier of driveRestoreArtifact
  - `[ExchangeProtectionPolicyId <String>]`: The unique identifier of exchangeProtectionPolicy
  - `[ExchangeRestoreSessionId <String>]`: The unique identifier of exchangeRestoreSession
  - `[GranularMailboxRestoreArtifactId <String>]`: The unique identifier of granularMailboxRestoreArtifact
  - `[MailboxProtectionRuleId <String>]`: The unique identifier of mailboxProtectionRule
  - `[MailboxProtectionUnitId <String>]`: The unique identifier of mailboxProtectionUnit
  - `[MailboxRestoreArtifactId <String>]`: The unique identifier of mailboxRestoreArtifact
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
  - `[SiteRestoreArtifactId <String>]`: The unique identifier of siteRestoreArtifact

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.backuprestore/get-mgsolutionbackuprestorepointprotectionunit](https://learn.microsoft.com/powershell/module/microsoft.graph.backuprestore/get-mgsolutionbackuprestorepointprotectionunit)
























