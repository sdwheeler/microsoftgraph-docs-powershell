---
external help file: Microsoft.Graph.Reports-help.xml
Module Name: Microsoft.Graph.Reports
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.reports/get-mgreportskypeforbusinessdeviceusageusercount
schema: 2.0.0
ms.subservice: reports
---

# Get-MgReportSkypeForBusinessDeviceUsageUserCount

## SYNOPSIS
Get the usage trends on how many users in your organization have connected using the Skype for Business app.
You'll also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.

> [!NOTE]
> To view the beta release of this cmdlet, view [Get-MgBetaReportSkypeForBusinessDeviceUsageUserCount](/powershell/module/Microsoft.Graph.Beta.Reports/Get-MgBetaReportSkypeForBusinessDeviceUsageUserCount?view=graph-powershell-beta)

## SYNTAX

### Get (Default)
```
Get-MgReportSkypeForBusinessDeviceUsageUserCount -Period <String> -OutFile <String>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [<CommonParameters>]
```

### GetViaIdentity
```
Get-MgReportSkypeForBusinessDeviceUsageUserCount -InputObject <IReportsIdentity> -OutFile <String>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [<CommonParameters>]
```

## DESCRIPTION
Get the usage trends on how many users in your organization have connected using the Skype for Business app.
You'll also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Reports

Get-MgReportSkypeForBusinessDeviceUsageUserCount -Period $periodId

```
This example shows how to use the Get-MgReportSkypeForBusinessDeviceUsageUserCount Cmdlet.


## PARAMETERS

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
Type: IReportsIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -OutFile
Path to write output file to

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Returns true when the command succeeds

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Period
Usage: period='{period}'

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IReportsIdentity
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<IReportsIdentity>`: Identity Parameter
  - `[Date <DateTime?>]`: Usage: date={date}
  - `[DeviceManagementExportJobId <String>]`: The unique identifier of deviceManagementExportJob
  - `[DirectoryAuditId <String>]`: The unique identifier of directoryAudit
  - `[EndDateTime <DateTime?>]`: Usage: endDateTime={endDateTime}
  - `[Filter <String>]`: Usage: filter='{filter}'
  - `[GroupId <String>]`: Usage: groupId='{groupId}'
  - `[IncludedUserRoles <String>]`: Usage: includedUserRoles='{includedUserRoles}'
  - `[IncludedUserTypes <String>]`: Usage: includedUserTypes='{includedUserTypes}'
  - `[ManifestId <String>]`: The unique identifier of manifest
  - `[OperationId <String>]`: The unique identifier of operation
  - `[Period <String>]`: Usage: period='{period}'
  - `[PrintUsageByPrinterId <String>]`: The unique identifier of printUsageByPrinter
  - `[PrintUsageByUserId <String>]`: The unique identifier of printUsageByUser
  - `[PrinterId <String>]`: Usage: printerId='{printerId}'
  - `[ProvisioningObjectSummaryId <String>]`: The unique identifier of provisioningObjectSummary
  - `[SignInId <String>]`: The unique identifier of signIn
  - `[Skip <Int32?>]`: Usage: skip={skip}
  - `[SkipToken <String>]`: Usage: skipToken='{skipToken}'
  - `[StartDateTime <DateTime?>]`: Usage: startDateTime={startDateTime}
  - `[Top <Int32?>]`: Usage: top={top}
  - `[UserId <String>]`: Usage: userId='{userId}'
  - `[UserRegistrationDetailsId <String>]`: The unique identifier of userRegistrationDetails

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.reports/get-mgreportskypeforbusinessdeviceusageusercount](https://learn.microsoft.com/powershell/module/microsoft.graph.reports/get-mgreportskypeforbusinessdeviceusageusercount)

[https://learn.microsoft.com/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-1.0](https://learn.microsoft.com/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-1.0)























