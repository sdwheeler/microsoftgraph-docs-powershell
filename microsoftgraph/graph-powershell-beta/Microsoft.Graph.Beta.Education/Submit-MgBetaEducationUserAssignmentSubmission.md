---
external help file: Microsoft.Graph.Beta.Education-help.xml
Module Name: Microsoft.Graph.Beta.Education
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.education/submit-mgbetaeducationuserassignmentsubmission
schema: 2.0.0
ms.subservice: education
---

# Submit-MgBetaEducationUserAssignmentSubmission

## SYNOPSIS
Indicate that a student is done with the work and is ready to hand in the assignment.
Only teachers, students, and applications with application permissions can perform this operation.
This method changes the status of the submission from working to submitted.
During the submit process, all the resources are copied to the submittedResources bucket.
The teacher will be looking at the submitted resources list for grading.
A teacher can also submit a student's assignment on their behalf.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Submit-MgEducationUserAssignmentSubmission](/powershell/module/Microsoft.Graph.Education/Submit-MgEducationUserAssignmentSubmission?view=graph-powershell-1.0)

## SYNTAX

### Submit (Default)
```
Submit-MgBetaEducationUserAssignmentSubmission -EducationAssignmentId <String> -EducationSubmissionId <String>
 -EducationUserId <String> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SubmitViaIdentity
```
Submit-MgBetaEducationUserAssignmentSubmission -InputObject <IEducationIdentity>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Indicate that a student is done with the work and is ready to hand in the assignment.
Only teachers, students, and applications with application permissions can perform this operation.
This method changes the status of the submission from working to submitted.
During the submit process, all the resources are copied to the submittedResources bucket.
The teacher will be looking at the submitted resources list for grading.
A teacher can also submit a student's assignment on their behalf.

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
Parameter Sets: Submit
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EducationSubmissionId
The unique identifier of educationSubmission

```yaml
Type: String
Parameter Sets: Submit
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
Parameter Sets: Submit
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

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IEducationIdentity
Parameter Sets: SubmitViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphEducationSubmission
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

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.education/submit-mgbetaeducationuserassignmentsubmission](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.education/submit-mgbetaeducationuserassignmentsubmission)

[https://learn.microsoft.com/graph/api/educationsubmission-submit?view=graph-rest-beta](https://learn.microsoft.com/graph/api/educationsubmission-submit?view=graph-rest-beta)
























