---
external help file: Microsoft.Graph.Beta.Bookings-help.xml
Module Name: Microsoft.Graph.Beta.Bookings
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/remove-mgbetabookingbusinessappointment
schema: 2.0.0
---

# Remove-MgBetaBookingBusinessAppointment

## SYNOPSIS
Delete navigation property appointments for bookingBusinesses

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Remove-MgBookingBusinessAppointment](/powershell/module/Microsoft.Graph.Bookings/Remove-MgBookingBusinessAppointment?view=graph-powershell-1.0)

## SYNTAX

### Delete (Default)
```
Remove-MgBetaBookingBusinessAppointment -BookingAppointmentId <String> -BookingBusinessId <String>
 [-IfMatch <String>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Delete1
```
Remove-MgBetaBookingBusinessAppointment -BookingAppointmentId <String> -BookingBusinessId <String>
 [-IfMatch <String>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### DeleteViaIdentity1
```
Remove-MgBetaBookingBusinessAppointment -InputObject <IBookingsIdentity> [-IfMatch <String>]
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### DeleteViaIdentity
```
Remove-MgBetaBookingBusinessAppointment -InputObject <IBookingsIdentity> [-IfMatch <String>]
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Delete navigation property appointments for bookingBusinesses

**Permissions**

| Permission type | Permissions (from least to most privileged) |
| --------------- | ------------------------------------------  |
| Delegated (work or school account) | BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All,  |
| Delegated (personal Microsoft account) | Not supported |
| Application | BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Read.All, Bookings.Manage.All,  |

## EXAMPLES
### Example 1: Using the Remove-MgBetaBookingBusinessAppointment Cmdlet
```powershell
Import-Module Microsoft.Graph.Beta.Bookings
Remove-MgBetaBookingBusinessAppointment -BookingBusinessId $bookingBusinessId -BookingAppointmentId $bookingAppointmentId
```
This example shows how to use the Remove-MgBetaBookingBusinessAppointment Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

## PARAMETERS

### -BookingAppointmentId
The unique identifier of bookingAppointment

```yaml
Type: String
Parameter Sets: Delete, Delete1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BookingBusinessId
The unique identifier of bookingBusiness

```yaml
Type: String
Parameter Sets: Delete, Delete1
Aliases:

Required: True
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

### -IfMatch
ETag

```yaml
Type: String
Parameter Sets: (All)
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
Type: IBookingsIdentity
Parameter Sets: DeleteViaIdentity1, DeleteViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

### Microsoft.Graph.Beta.PowerShell.Models.IBookingsIdentity
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<IBookingsIdentity>`: Identity Parameter
  - `[AttendanceRecordId <String>]`: The unique identifier of attendanceRecord
  - `[BookingAppointmentId <String>]`: The unique identifier of bookingAppointment
  - `[BookingBusinessId <String>]`: The unique identifier of bookingBusiness
  - `[BookingCurrencyId <String>]`: The unique identifier of bookingCurrency
  - `[BookingCustomQuestionId <String>]`: The unique identifier of bookingCustomQuestion
  - `[BookingCustomerId <String>]`: The unique identifier of bookingCustomer
  - `[BookingServiceId <String>]`: The unique identifier of bookingService
  - `[BookingStaffMemberId <String>]`: The unique identifier of bookingStaffMember
  - `[Email <String>]`: Alternate key of virtualEventRegistration
  - `[JoinWebUrl <String>]`: Alternate key of virtualEventSession
  - `[MeetingAttendanceReportId <String>]`: The unique identifier of meetingAttendanceReport
  - `[Role <String>]`: Usage: role='{role}'
  - `[UserId <String>]`: Alternate key of virtualEventRegistration
  - `[VirtualEventId <String>]`: The unique identifier of virtualEvent
  - `[VirtualEventPresenterId <String>]`: The unique identifier of virtualEventPresenter
  - `[VirtualEventRegistrationId <String>]`: The unique identifier of virtualEventRegistration
  - `[VirtualEventRegistrationQuestionBaseId <String>]`: The unique identifier of virtualEventRegistrationQuestionBase
  - `[VirtualEventSessionId <String>]`: The unique identifier of virtualEventSession
  - `[VirtualEventTownhallId <String>]`: The unique identifier of virtualEventTownhall
  - `[VirtualEventWebinarId <String>]`: The unique identifier of virtualEventWebinar

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/remove-mgbetabookingbusinessappointment](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.bookings/remove-mgbetabookingbusinessappointment)

[https://learn.microsoft.com/graph/api/bookingappointment-delete?view=graph-rest-beta](https://learn.microsoft.com/graph/api/bookingappointment-delete?view=graph-rest-beta)























