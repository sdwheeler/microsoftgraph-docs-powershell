---
external help file: Microsoft.Graph.Bookings-help.xml
Module Name: Microsoft.Graph.Bookings
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.bookings/set-mgvirtualeventexternaleventinformation
schema: 2.0.0
---

# Set-MgVirtualEventExternalEventInformation

## SYNOPSIS
Invoke action setExternalEventInformation

> [!NOTE]
> To view the beta release of this cmdlet, view [Set-MgBetaVirtualEventExternalEventInformation](/powershell/module/Microsoft.Graph.Beta.Bookings/Set-MgBetaVirtualEventExternalEventInformation?view=graph-powershell-beta)

## SYNTAX

### SetExpanded (Default)
```
Set-MgVirtualEventExternalEventInformation -VirtualEventId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ExternalEventId <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Set
```
Set-MgVirtualEventExternalEventInformation -VirtualEventId <String>
 -BodyParameter <IPaths168Q9LmSolutionsVirtualeventsEventsVirtualeventIdMicrosoftGraphSetexternaleventinformationPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SetViaIdentityExpanded
```
Set-MgVirtualEventExternalEventInformation -InputObject <IBookingsIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ExternalEventId <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SetViaIdentity
```
Set-MgVirtualEventExternalEventInformation -InputObject <IBookingsIdentity>
 -BodyParameter <IPaths168Q9LmSolutionsVirtualeventsEventsVirtualeventIdMicrosoftGraphSetexternaleventinformationPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Invoke action setExternalEventInformation

## EXAMPLES

## PARAMETERS

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

To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IPaths168Q9LmSolutionsVirtualeventsEventsVirtualeventIdMicrosoftGraphSetexternaleventinformationPostRequestbodyContentApplicationJsonSchema
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

### -ExternalEventId


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
Type: IBookingsIdentity
Parameter Sets: SetViaIdentityExpanded, SetViaIdentity
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

### -VirtualEventId
The unique identifier of virtualEvent

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

### Microsoft.Graph.PowerShell.Models.IBookingsIdentity
### Microsoft.Graph.PowerShell.Models.IPaths168Q9LmSolutionsVirtualeventsEventsVirtualeventIdMicrosoftGraphSetexternaleventinformationPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IPaths168Q9LmSolutionsVirtualeventsEventsVirtualeventIdMicrosoftGraphSetexternaleventinformationPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[ExternalEventId <String>]`:

INPUTOBJECT `<IBookingsIdentity>`: Identity Parameter
  - `[AttendanceRecordId <String>]`: The unique identifier of attendanceRecord
  - `[BookingAppointmentId <String>]`: The unique identifier of bookingAppointment
  - `[BookingBusinessId <String>]`: The unique identifier of bookingBusiness
  - `[BookingCurrencyId <String>]`: The unique identifier of bookingCurrency
  - `[BookingCustomQuestionId <String>]`: The unique identifier of bookingCustomQuestion
  - `[BookingCustomerBaseId <String>]`: The unique identifier of bookingCustomerBase
  - `[BookingServiceId <String>]`: The unique identifier of bookingService
  - `[BookingStaffMemberBaseId <String>]`: The unique identifier of bookingStaffMemberBase
  - `[Email <String>]`: Alternate key of virtualEventRegistration
  - `[MeetingAttendanceReportId <String>]`: The unique identifier of meetingAttendanceReport
  - `[Role <String>]`: Usage: role='{role}'
  - `[UserId <String>]`: Usage: userId='{userId}'
  - `[VirtualEventId <String>]`: The unique identifier of virtualEvent
  - `[VirtualEventPresenterId <String>]`: The unique identifier of virtualEventPresenter
  - `[VirtualEventRegistrationId <String>]`: The unique identifier of virtualEventRegistration
  - `[VirtualEventRegistrationQuestionBaseId <String>]`: The unique identifier of virtualEventRegistrationQuestionBase
  - `[VirtualEventSessionId <String>]`: The unique identifier of virtualEventSession
  - `[VirtualEventTownhallId <String>]`: The unique identifier of virtualEventTownhall
  - `[VirtualEventWebinarId <String>]`: The unique identifier of virtualEventWebinar

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.bookings/set-mgvirtualeventexternaleventinformation](https://learn.microsoft.com/powershell/module/microsoft.graph.bookings/set-mgvirtualeventexternaleventinformation)
























