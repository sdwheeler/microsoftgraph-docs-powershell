---
external help file: Microsoft.Graph.Beta.Education-help.xml
Module Name: Microsoft.Graph.Beta.Education
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.education/remove-mgbetaeducationuserassignmentcategoryeducationcategorybyref
schema: 2.0.0
---

# Remove-MgBetaEducationUserAssignmentCategoryEducationCategoryByRef

## SYNOPSIS
Delete ref of navigation property categories for education

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Remove-MgEducationUserAssignmentCategoryEducationCategoryByRef](/powershell/module/Microsoft.Graph.Education/Remove-MgEducationUserAssignmentCategoryEducationCategoryByRef?view=graph-powershell-1.0)

## SYNTAX

### Delete (Default)
```
Remove-MgBetaEducationUserAssignmentCategoryEducationCategoryByRef -EducationAssignmentId <String>
 -EducationCategoryId <String> -EducationUserId <String> [-IfMatch <String>]
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### DeleteViaIdentity
```
Remove-MgBetaEducationUserAssignmentCategoryEducationCategoryByRef -InputObject <IEducationIdentity>
 [-IfMatch <String>] [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Delete ref of navigation property categories for education

## EXAMPLES

## PARAMETERS

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

### -EducationAssignmentId
The unique identifier of educationAssignment

```yaml
Type: String
Parameter Sets: Delete
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EducationCategoryId
The unique identifier of educationCategory

```yaml
Type: String
Parameter Sets: Delete
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EducationUserId
The unique identifier of educationUser

```yaml
Type: String
Parameter Sets: Delete
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
Type: IEducationIdentity
Parameter Sets: DeleteViaIdentity
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

### Microsoft.Graph.Beta.PowerShell.Models.IEducationIdentity
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

INPUTOBJECT `<IEducationIdentity>`: Identity Parameter
  - `[EducationAssignmentId <String>]`: The unique identifier of educationAssignment
  - `[EducationAssignmentResourceId <String>]`: The unique identifier of educationAssignmentResource
  - `[EducationAssignmentResourceId1 <String>]`: The unique identifier of educationAssignmentResource
  - `[EducationCategoryId <String>]`: The unique identifier of educationCategory
  - `[EducationClassId <String>]`: The unique identifier of educationClass
  - `[EducationGradingCategoryId <String>]`: The unique identifier of educationGradingCategory
  - `[EducationGradingSchemeId <String>]`: The unique identifier of educationGradingScheme
  - `[EducationModuleId <String>]`: The unique identifier of educationModule
  - `[EducationModuleResourceId <String>]`: The unique identifier of educationModuleResource
  - `[EducationOutcomeId <String>]`: The unique identifier of educationOutcome
  - `[EducationRubricId <String>]`: The unique identifier of educationRubric
  - `[EducationSchoolId <String>]`: The unique identifier of educationSchool
  - `[EducationSubmissionId <String>]`: The unique identifier of educationSubmission
  - `[EducationSubmissionResourceId <String>]`: The unique identifier of educationSubmissionResource
  - `[EducationSubmissionResourceId1 <String>]`: The unique identifier of educationSubmissionResource
  - `[EducationUserId <String>]`: The unique identifier of educationUser
  - `[ReadingAssignmentSubmissionId <String>]`: The unique identifier of readingAssignmentSubmission
  - `[ReflectCheckInResponseId <String>]`: The unique identifier of reflectCheckInResponse

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.education/remove-mgbetaeducationuserassignmentcategoryeducationcategorybyref](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.education/remove-mgbetaeducationuserassignmentcategoryeducationcategorybyref)
























