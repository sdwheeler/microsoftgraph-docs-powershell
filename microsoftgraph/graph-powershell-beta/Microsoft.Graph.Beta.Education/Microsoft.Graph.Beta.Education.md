---
Module Name: Microsoft.Graph.Beta.Education
Module Guid: 93e18191-d418-4d25-9d4d-4c3060dc47a4
Download Help Link: https://learn.microsoft.com/en-us/powershell/module/microsoft.graph.beta.education/?view=graph-powershell-beta
Help Version: 1.0.0.0
Locale: en-US
---

# Microsoft.Graph.Beta.Education Module
## Description
Microsoft Graph PowerShell Cmdlets

## Microsoft.Graph.Beta.Education Cmdlets
### [Get-MgBetaEducationClass](Get-MgBetaEducationClass.md)
Retrieve a class from the system. A class is a universal group with a special property that indicates to the system that the group is a class. Group members represent the students; group admins represent the teachers in the class. If you're using the delegated token, the user will only see classes in which they are members.

### [Get-MgBetaEducationClassAssignment](Get-MgBetaEducationClassAssignment.md)
Get the properties and relationships of an assignment. Only teachers, students, and applications with application permissions can perform this operation. Students can only see assignments assigned to them; teachers and applications with application permissions can see all assignments in a class. You can use the Prefer header in your request to get the inactive status in case the assignment is deactivated; otherwise, the response value for the status property is unknownFutureValue.

### [Get-MgBetaEducationClassAssignmentCategory](Get-MgBetaEducationClassAssignmentCategory.md)
Retrieve an educationCategory object. Only teachers, students, and applications with application permissions can perform this operation.

### [Get-MgBetaEducationClassAssignmentCategoryByRef](Get-MgBetaEducationClassAssignmentCategoryByRef.md)
List all categories for an assignment. Only teachers, students, and applications with application permissions can perform this operation.

### [Get-MgBetaEducationClassAssignmentCategoryCount](Get-MgBetaEducationClassAssignmentCategoryCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassAssignmentCategoryDelta](Get-MgBetaEducationClassAssignmentCategoryDelta.md)
Get a list of newly created or updated educationCategory objects without performing a full read of the collection.

### [Get-MgBetaEducationClassAssignmentCount](Get-MgBetaEducationClassAssignmentCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassAssignmentDefault](Get-MgBetaEducationClassAssignmentDefault.md)
Read the properties and relationships of an educationAssignmentDefaults object. These are the class-level assignment defaults respected by new assignments created in the class. Callers can continue to specify custom values on each assignment creation if they don't want the default behaviors. Only teachers can perform this operation.

### [Get-MgBetaEducationClassAssignmentDelta](Get-MgBetaEducationClassAssignmentDelta.md)
Get a list of newly-created or updated assignments without reading the entire collection. A teacher or an application running with application permissions can see all assignment objects for the class. Students can only see assignments that are assigned to them.

### [Get-MgBetaEducationClassAssignmentGradingCategory](Get-MgBetaEducationClassAssignmentGradingCategory.md)
When set, enables users to weight assignments differently when computing a class average grade.

### [Get-MgBetaEducationClassAssignmentGradingScheme](Get-MgBetaEducationClassAssignmentGradingScheme.md)
Get gradingScheme from education

### [Get-MgBetaEducationClassAssignmentResource](Get-MgBetaEducationClassAssignmentResource.md)
Get the properties of an education assignment resource associated with an assignment. Only teachers, students, and applications with application permissions can perform this operation.

### [Get-MgBetaEducationClassAssignmentResourceCount](Get-MgBetaEducationClassAssignmentResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassAssignmentResourceDependentResource](Get-MgBetaEducationClassAssignmentResourceDependentResource.md)
Get dependentResources from education

### [Get-MgBetaEducationClassAssignmentResourceDependentResourceCount](Get-MgBetaEducationClassAssignmentResourceDependentResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassAssignmentRubric](Get-MgBetaEducationClassAssignmentRubric.md)
Get the educationRubric object attached to an educationAssignment, if one exists. Only teachers, students, and applications with application permissions can perform this operation.

### [Get-MgBetaEducationClassAssignmentRubricByRef](Get-MgBetaEducationClassAssignmentRubricByRef.md)
Get the educationRubric object attached to an educationAssignment, if one exists. Only teachers, students, and applications with application permissions can perform this operation.

### [Get-MgBetaEducationClassAssignmentSetting](Get-MgBetaEducationClassAssignmentSetting.md)
Read the properties and relationships of an educationAssignmentSettings object. Only teachers can perform this operation.

### [Get-MgBetaEducationClassAssignmentSettingDefaultGradingScheme](Get-MgBetaEducationClassAssignmentSettingDefaultGradingScheme.md)
Get defaultGradingScheme from education

### [Get-MgBetaEducationClassAssignmentSettingGradingCategory](Get-MgBetaEducationClassAssignmentSettingGradingCategory.md)
When set, enables users to weight assignments differently when computing a class average grade.

### [Get-MgBetaEducationClassAssignmentSettingGradingCategoryCount](Get-MgBetaEducationClassAssignmentSettingGradingCategoryCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassAssignmentSettingGradingScheme](Get-MgBetaEducationClassAssignmentSettingGradingScheme.md)
Read the properties and relationships of an educationGradingScheme object.

### [Get-MgBetaEducationClassAssignmentSettingGradingSchemeCount](Get-MgBetaEducationClassAssignmentSettingGradingSchemeCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassAssignmentSubmission](Get-MgBetaEducationClassAssignmentSubmission.md)
Retrieve a particular submission. Only teachers, students, and applications with application permissions can perform this operation. A submission object represents a student's work for an assignment. Resources associated with the submission represent this work. Only the assignedTo student can see and modify the submission. A teacher or application with application permissions has full access to all submissions. The grade and feedback from a teacher are part of the educationOutcome associated with this object. Only teachers or applications with application permissions can add or change grades and feedback. Students will not see the grade or feedback until the assignment has been released. Provide the header Prefer: include-unknown-enum-members to properly list submissions with the reassigned status. For details, see the examples section.

### [Get-MgBetaEducationClassAssignmentSubmissionCount](Get-MgBetaEducationClassAssignmentSubmissionCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassAssignmentSubmissionOutcome](Get-MgBetaEducationClassAssignmentSubmissionOutcome.md)
Get outcomes from education

### [Get-MgBetaEducationClassAssignmentSubmissionOutcomeCount](Get-MgBetaEducationClassAssignmentSubmissionOutcomeCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassAssignmentSubmissionResource](Get-MgBetaEducationClassAssignmentSubmissionResource.md)
Retrieve the properties of a specific resource associated with a submission. Only teachers, students, and applications with application permissions can perform this operation. This resource is in the 'working' resource list and should be considered work in process by a student. This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.

### [Get-MgBetaEducationClassAssignmentSubmissionResourceCount](Get-MgBetaEducationClassAssignmentSubmissionResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassAssignmentSubmissionResourceDependentResource](Get-MgBetaEducationClassAssignmentSubmissionResourceDependentResource.md)
Get dependentResources from education

### [Get-MgBetaEducationClassAssignmentSubmissionResourceDependentResourceCount](Get-MgBetaEducationClassAssignmentSubmissionResourceDependentResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassAssignmentSubmissionSubmittedResource](Get-MgBetaEducationClassAssignmentSubmissionSubmittedResource.md)
Get submittedResources from education

### [Get-MgBetaEducationClassAssignmentSubmissionSubmittedResourceCount](Get-MgBetaEducationClassAssignmentSubmissionSubmittedResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassAssignmentSubmissionSubmittedResourceDependentResource](Get-MgBetaEducationClassAssignmentSubmissionSubmittedResourceDependentResource.md)
Get dependentResources from education

### [Get-MgBetaEducationClassAssignmentSubmissionSubmittedResourceDependentResourceCount](Get-MgBetaEducationClassAssignmentSubmissionSubmittedResourceDependentResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassCount](Get-MgBetaEducationClassCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassDelta](Get-MgBetaEducationClassDelta.md)
Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection. See Use delta query for details.

### [Get-MgBetaEducationClassGroup](Get-MgBetaEducationClassGroup.md)
Retrieve the Microsoft 365 group that corresponds to this educationClass.

### [Get-MgBetaEducationClassGroupServiceProvisioningError](Get-MgBetaEducationClassGroupServiceProvisioningError.md)
Errors published by a federated service describing a non-transient, service-specific error regarding the properties or link from a group object.

### [Get-MgBetaEducationClassGroupServiceProvisioningErrorCount](Get-MgBetaEducationClassGroupServiceProvisioningErrorCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassMember](Get-MgBetaEducationClassMember.md)
Retrieve the teachers and students for a class. Note that if the delegated token is used, members can only be seen by other members of the class.

### [Get-MgBetaEducationClassMemberByRef](Get-MgBetaEducationClassMemberByRef.md)
Retrieve the teachers and students for a class. Note that if the delegated token is used, members can only be seen by other members of the class.

### [Get-MgBetaEducationClassMemberCount](Get-MgBetaEducationClassMemberCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassModule](Get-MgBetaEducationClassModule.md)
Get the properties and relationships of a module. Only teachers, students, and applications with application permissions can perform this operation. Students can only see published modules; teachers and applications with application permissions can see all modules in a class.

### [Get-MgBetaEducationClassModuleCount](Get-MgBetaEducationClassModuleCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassModuleResource](Get-MgBetaEducationClassModuleResource.md)
Get the properties of a resource associated with a module. Only teachers, students, and applications with application permissions can perform this operation.

### [Get-MgBetaEducationClassModuleResourceCount](Get-MgBetaEducationClassModuleResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassRecentlyModifiedSubmission](Get-MgBetaEducationClassRecentlyModifiedSubmission.md)
Retrieve submissions modified in the previous seven days. Only teachers and applications with application permissions can perform this operation. A submission object represents a student's work for an assignment. Resources associated with the submission represent their work. A teacher or application with application permissions has full access to all submission objects. The grade and feedback from a teacher are part of the educationOutcome associated with this object. Only teachers or applications with application permissions can add or change grades and feedback. Students can't see the grade or feedback until the assignment is released.

### [Get-MgBetaEducationClassSchool](Get-MgBetaEducationClassSchool.md)
All schools that this class is associated with. Nullable.

### [Get-MgBetaEducationClassSchoolCount](Get-MgBetaEducationClassSchoolCount.md)
Get the number of the resource

### [Get-MgBetaEducationClassTeacher](Get-MgBetaEducationClassTeacher.md)
Retrieve a list of teachers for a class. Delegated tokens must be members of the class to get the teacher list.

### [Get-MgBetaEducationClassTeacherByRef](Get-MgBetaEducationClassTeacherByRef.md)
Retrieve a list of teachers for a class. Delegated tokens must be members of the class to get the teacher list.

### [Get-MgBetaEducationClassTeacherCount](Get-MgBetaEducationClassTeacherCount.md)
Get the number of the resource

### [Get-MgBetaEducationMe](Get-MgBetaEducationMe.md)
Get me from education

### [Get-MgBetaEducationMeAssignment](Get-MgBetaEducationMeAssignment.md)
List of assignments for the user. Nullable.

### [Get-MgBetaEducationMeAssignmentCategory](Get-MgBetaEducationMeAssignmentCategory.md)
When set, enables users to easily find assignments of a given type. Read-only. Nullable.

### [Get-MgBetaEducationMeAssignmentCategoryByRef](Get-MgBetaEducationMeAssignmentCategoryByRef.md)
When set, enables users to easily find assignments of a given type. Read-only. Nullable.

### [Get-MgBetaEducationMeAssignmentCategoryCount](Get-MgBetaEducationMeAssignmentCategoryCount.md)
Get the number of the resource

### [Get-MgBetaEducationMeAssignmentCategoryDelta](Get-MgBetaEducationMeAssignmentCategoryDelta.md)
Get a list of newly created or updated educationCategory objects without performing a full read of the collection.

### [Get-MgBetaEducationMeAssignmentCount](Get-MgBetaEducationMeAssignmentCount.md)
Get the number of the resource

### [Get-MgBetaEducationMeAssignmentDelta](Get-MgBetaEducationMeAssignmentDelta.md)
Get a list of newly-created or updated assignments without reading the entire collection. A teacher or an application running with application permissions can see all assignment objects for the class. Students can only see assignments that are assigned to them.

### [Get-MgBetaEducationMeAssignmentGradingCategory](Get-MgBetaEducationMeAssignmentGradingCategory.md)
When set, enables users to weight assignments differently when computing a class average grade.

### [Get-MgBetaEducationMeAssignmentGradingScheme](Get-MgBetaEducationMeAssignmentGradingScheme.md)
Get gradingScheme from education

### [Get-MgBetaEducationMeAssignmentResource](Get-MgBetaEducationMeAssignmentResource.md)
Learning objects that are associated with this assignment. Only teachers can modify this list. Nullable.

### [Get-MgBetaEducationMeAssignmentResourceCount](Get-MgBetaEducationMeAssignmentResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationMeAssignmentResourceDependentResource](Get-MgBetaEducationMeAssignmentResourceDependentResource.md)
Get dependentResources from education

### [Get-MgBetaEducationMeAssignmentResourceDependentResourceCount](Get-MgBetaEducationMeAssignmentResourceDependentResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationMeAssignmentRubric](Get-MgBetaEducationMeAssignmentRubric.md)
When set, the grading rubric attached to this assignment.

### [Get-MgBetaEducationMeAssignmentRubricByRef](Get-MgBetaEducationMeAssignmentRubricByRef.md)
When set, the grading rubric attached to this assignment.

### [Get-MgBetaEducationMeAssignmentSubmission](Get-MgBetaEducationMeAssignmentSubmission.md)
Once published, there is a submission object for each student representing their work and grade. Read-only. Nullable.

### [Get-MgBetaEducationMeAssignmentSubmissionCount](Get-MgBetaEducationMeAssignmentSubmissionCount.md)
Get the number of the resource

### [Get-MgBetaEducationMeAssignmentSubmissionOutcome](Get-MgBetaEducationMeAssignmentSubmissionOutcome.md)
Get outcomes from education

### [Get-MgBetaEducationMeAssignmentSubmissionOutcomeCount](Get-MgBetaEducationMeAssignmentSubmissionOutcomeCount.md)
Get the number of the resource

### [Get-MgBetaEducationMeAssignmentSubmissionResource](Get-MgBetaEducationMeAssignmentSubmissionResource.md)
Get resources from education

### [Get-MgBetaEducationMeAssignmentSubmissionResourceCount](Get-MgBetaEducationMeAssignmentSubmissionResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationMeAssignmentSubmissionResourceDependentResource](Get-MgBetaEducationMeAssignmentSubmissionResourceDependentResource.md)
Get dependentResources from education

### [Get-MgBetaEducationMeAssignmentSubmissionResourceDependentResourceCount](Get-MgBetaEducationMeAssignmentSubmissionResourceDependentResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationMeAssignmentSubmissionSubmittedResource](Get-MgBetaEducationMeAssignmentSubmissionSubmittedResource.md)
Get submittedResources from education

### [Get-MgBetaEducationMeAssignmentSubmissionSubmittedResourceCount](Get-MgBetaEducationMeAssignmentSubmissionSubmittedResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationMeAssignmentSubmissionSubmittedResourceDependentResource](Get-MgBetaEducationMeAssignmentSubmissionSubmittedResourceDependentResource.md)
Get dependentResources from education

### [Get-MgBetaEducationMeAssignmentSubmissionSubmittedResourceDependentResourceCount](Get-MgBetaEducationMeAssignmentSubmissionSubmittedResourceDependentResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationMeClass](Get-MgBetaEducationMeClass.md)
Classes to which the user belongs. Nullable.

### [Get-MgBetaEducationMeClassCount](Get-MgBetaEducationMeClassCount.md)
Get the number of the resource

### [Get-MgBetaEducationMeRubric](Get-MgBetaEducationMeRubric.md)
Retrieve the properties and relationships of an educationRubric object. Only teachers and students can perform this operation.

### [Get-MgBetaEducationMeRubricCount](Get-MgBetaEducationMeRubricCount.md)
Get the number of the resource

### [Get-MgBetaEducationMeSchool](Get-MgBetaEducationMeSchool.md)
Schools to which the user belongs. Nullable.

### [Get-MgBetaEducationMeSchoolCount](Get-MgBetaEducationMeSchoolCount.md)
Get the number of the resource

### [Get-MgBetaEducationMeTaughtClass](Get-MgBetaEducationMeTaughtClass.md)
Classes for which the user is a teacher.

### [Get-MgBetaEducationMeTaughtClassCount](Get-MgBetaEducationMeTaughtClassCount.md)
Get the number of the resource

### [Get-MgBetaEducationMeUser](Get-MgBetaEducationMeUser.md)
Retrieve the simple directory user that corresponds to this educationUser.

### [Get-MgBetaEducationMeUserMailboxSetting](Get-MgBetaEducationMeUserMailboxSetting.md)
Settings for the primary mailbox of the signed-in user. You can get or update settings for sending automatic replies to incoming messages, locale, and time zone. For more information, see User preferences for languages and regional formats. Returned only on $select.

### [Get-MgBetaEducationMeUserServiceProvisioningError](Get-MgBetaEducationMeUserServiceProvisioningError.md)
Errors published by a federated service describing a nontransient, service-specific error regarding the properties or link from a user object.

### [Get-MgBetaEducationMeUserServiceProvisioningErrorCount](Get-MgBetaEducationMeUserServiceProvisioningErrorCount.md)
Get the number of the resource

### [Get-MgBetaEducationReport](Get-MgBetaEducationReport.md)
Get reports from education

### [Get-MgBetaEducationReportReadingAssignmentSubmission](Get-MgBetaEducationReportReadingAssignmentSubmission.md)
Get readingAssignmentSubmissions from education

### [Get-MgBetaEducationReportReadingAssignmentSubmissionCount](Get-MgBetaEducationReportReadingAssignmentSubmissionCount.md)
Get the number of the resource

### [Get-MgBetaEducationReportReflectCheck](Get-MgBetaEducationReportReflectCheck.md)
Get reflectCheckInResponses from education

### [Get-MgBetaEducationReportReflectCheckInResponseCount](Get-MgBetaEducationReportReflectCheckInResponseCount.md)
Get the number of the resource

### [Get-MgBetaEducationRoot](Get-MgBetaEducationRoot.md)
Get education

### [Get-MgBetaEducationSchool](Get-MgBetaEducationSchool.md)
Retrieve the properties and relationships of the school object.

### [Get-MgBetaEducationSchoolAdministrativeUnit](Get-MgBetaEducationSchoolAdministrativeUnit.md)
Retrieve the directory administrativeUnit that corresponds to this educationSchool.

### [Get-MgBetaEducationSchoolClass](Get-MgBetaEducationSchoolClass.md)
Retrieve a list of classes owned by a school.

### [Get-MgBetaEducationSchoolClassByRef](Get-MgBetaEducationSchoolClassByRef.md)
Retrieve a list of classes owned by a school.

### [Get-MgBetaEducationSchoolClassCount](Get-MgBetaEducationSchoolClassCount.md)
Get the number of the resource

### [Get-MgBetaEducationSchoolCount](Get-MgBetaEducationSchoolCount.md)
Get the number of the resource

### [Get-MgBetaEducationSchoolDelta](Get-MgBetaEducationSchoolDelta.md)
Get newly created or updated schools without having to perform a full read of the entire school collection. See Use delta query for details.

### [Get-MgBetaEducationSchoolUser](Get-MgBetaEducationSchoolUser.md)
Retrieve a list of users at a school.

### [Get-MgBetaEducationSchoolUserByRef](Get-MgBetaEducationSchoolUserByRef.md)
Retrieve a list of users at a school.

### [Get-MgBetaEducationSchoolUserCount](Get-MgBetaEducationSchoolUserCount.md)
Get the number of the resource

### [Get-MgBetaEducationUser](Get-MgBetaEducationUser.md)
Retrieve the properties and relationships of a user.

### [Get-MgBetaEducationUserAssignment](Get-MgBetaEducationUserAssignment.md)
List of assignments for the user. Nullable.

### [Get-MgBetaEducationUserAssignmentCategory](Get-MgBetaEducationUserAssignmentCategory.md)
When set, enables users to easily find assignments of a given type. Read-only. Nullable.

### [Get-MgBetaEducationUserAssignmentCategoryByRef](Get-MgBetaEducationUserAssignmentCategoryByRef.md)
When set, enables users to easily find assignments of a given type. Read-only. Nullable.

### [Get-MgBetaEducationUserAssignmentCategoryCount](Get-MgBetaEducationUserAssignmentCategoryCount.md)
Get the number of the resource

### [Get-MgBetaEducationUserAssignmentCategoryDelta](Get-MgBetaEducationUserAssignmentCategoryDelta.md)
Get a list of newly created or updated educationCategory objects without performing a full read of the collection.

### [Get-MgBetaEducationUserAssignmentCount](Get-MgBetaEducationUserAssignmentCount.md)
Get the number of the resource

### [Get-MgBetaEducationUserAssignmentDelta](Get-MgBetaEducationUserAssignmentDelta.md)
Get a list of newly-created or updated assignments without reading the entire collection. A teacher or an application running with application permissions can see all assignment objects for the class. Students can only see assignments that are assigned to them.

### [Get-MgBetaEducationUserAssignmentGradingCategory](Get-MgBetaEducationUserAssignmentGradingCategory.md)
When set, enables users to weight assignments differently when computing a class average grade.

### [Get-MgBetaEducationUserAssignmentGradingScheme](Get-MgBetaEducationUserAssignmentGradingScheme.md)
Get gradingScheme from education

### [Get-MgBetaEducationUserAssignmentResource](Get-MgBetaEducationUserAssignmentResource.md)
Learning objects that are associated with this assignment. Only teachers can modify this list. Nullable.

### [Get-MgBetaEducationUserAssignmentResourceCount](Get-MgBetaEducationUserAssignmentResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationUserAssignmentResourceDependentResource](Get-MgBetaEducationUserAssignmentResourceDependentResource.md)
Get dependentResources from education

### [Get-MgBetaEducationUserAssignmentResourceDependentResourceCount](Get-MgBetaEducationUserAssignmentResourceDependentResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationUserAssignmentRubric](Get-MgBetaEducationUserAssignmentRubric.md)
When set, the grading rubric attached to this assignment.

### [Get-MgBetaEducationUserAssignmentRubricByRef](Get-MgBetaEducationUserAssignmentRubricByRef.md)
When set, the grading rubric attached to this assignment.

### [Get-MgBetaEducationUserAssignmentSubmission](Get-MgBetaEducationUserAssignmentSubmission.md)
Once published, there is a submission object for each student representing their work and grade. Read-only. Nullable.

### [Get-MgBetaEducationUserAssignmentSubmissionCount](Get-MgBetaEducationUserAssignmentSubmissionCount.md)
Get the number of the resource

### [Get-MgBetaEducationUserAssignmentSubmissionOutcome](Get-MgBetaEducationUserAssignmentSubmissionOutcome.md)
Get outcomes from education

### [Get-MgBetaEducationUserAssignmentSubmissionOutcomeCount](Get-MgBetaEducationUserAssignmentSubmissionOutcomeCount.md)
Get the number of the resource

### [Get-MgBetaEducationUserAssignmentSubmissionResource](Get-MgBetaEducationUserAssignmentSubmissionResource.md)
Get resources from education

### [Get-MgBetaEducationUserAssignmentSubmissionResourceCount](Get-MgBetaEducationUserAssignmentSubmissionResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationUserAssignmentSubmissionResourceDependentResource](Get-MgBetaEducationUserAssignmentSubmissionResourceDependentResource.md)
Get dependentResources from education

### [Get-MgBetaEducationUserAssignmentSubmissionResourceDependentResourceCount](Get-MgBetaEducationUserAssignmentSubmissionResourceDependentResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationUserAssignmentSubmissionSubmittedResource](Get-MgBetaEducationUserAssignmentSubmissionSubmittedResource.md)
Get submittedResources from education

### [Get-MgBetaEducationUserAssignmentSubmissionSubmittedResourceCount](Get-MgBetaEducationUserAssignmentSubmissionSubmittedResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationUserAssignmentSubmissionSubmittedResourceDependentResource](Get-MgBetaEducationUserAssignmentSubmissionSubmittedResourceDependentResource.md)
Get dependentResources from education

### [Get-MgBetaEducationUserAssignmentSubmissionSubmittedResourceDependentResourceCount](Get-MgBetaEducationUserAssignmentSubmissionSubmittedResourceDependentResourceCount.md)
Get the number of the resource

### [Get-MgBetaEducationUserClass](Get-MgBetaEducationUserClass.md)
Classes to which the user belongs. Nullable.

### [Get-MgBetaEducationUserClassCount](Get-MgBetaEducationUserClassCount.md)
Get the number of the resource

### [Get-MgBetaEducationUserCount](Get-MgBetaEducationUserCount.md)
Get the number of the resource

### [Get-MgBetaEducationUserDelta](Get-MgBetaEducationUserDelta.md)
Get newly created or updated educationUser without having to perform a full read of the entire collection. See Use delta query for details.

### [Get-MgBetaEducationUserMailboxSetting](Get-MgBetaEducationUserMailboxSetting.md)
Settings for the primary mailbox of the signed-in user. You can get or update settings for sending automatic replies to incoming messages, locale, and time zone. For more information, see User preferences for languages and regional formats. Returned only on $select.

### [Get-MgBetaEducationUserRubric](Get-MgBetaEducationUserRubric.md)
When set, the grading rubric attached to the assignment.

### [Get-MgBetaEducationUserRubricCount](Get-MgBetaEducationUserRubricCount.md)
Get the number of the resource

### [Get-MgBetaEducationUserSchool](Get-MgBetaEducationUserSchool.md)
Schools to which the user belongs. Nullable.

### [Get-MgBetaEducationUserSchoolCount](Get-MgBetaEducationUserSchoolCount.md)
Get the number of the resource

### [Get-MgBetaEducationUserServiceProvisioningError](Get-MgBetaEducationUserServiceProvisioningError.md)
Errors published by a federated service describing a nontransient, service-specific error regarding the properties or link from a user object.

### [Get-MgBetaEducationUserServiceProvisioningErrorCount](Get-MgBetaEducationUserServiceProvisioningErrorCount.md)
Get the number of the resource

### [Get-MgBetaEducationUserTaughtClass](Get-MgBetaEducationUserTaughtClass.md)
Classes for which the user is a teacher.

### [Get-MgBetaEducationUserTaughtClassCount](Get-MgBetaEducationUserTaughtClassCount.md)
Get the number of the resource

### [Initialize-MgBetaEducationClassAssignment](Initialize-MgBetaEducationClassAssignment.md)
Activate an inactive educationAssignment to signal that the assignment has further action items for teachers or students. This action can only be performed by a teacher on currently inactive assignments.

### [Initialize-MgBetaEducationMeAssignment](Initialize-MgBetaEducationMeAssignment.md)
Activate an inactive educationAssignment to signal that the assignment has further action items for teachers or students. This action can only be performed by a teacher on currently inactive assignments.

### [Initialize-MgBetaEducationUserAssignment](Initialize-MgBetaEducationUserAssignment.md)
Activate an inactive educationAssignment to signal that the assignment has further action items for teachers or students. This action can only be performed by a teacher on currently inactive assignments.

### [Invoke-MgBetaDeactivateEducationClassAssignment](Invoke-MgBetaDeactivateEducationClassAssignment.md)
Mark an assigned educationAssignment as inactive to signal that the assignment has no further action items for teachers and students. This action can only be performed by a teacher on assigned assignments.

### [Invoke-MgBetaDeactivateEducationMeAssignment](Invoke-MgBetaDeactivateEducationMeAssignment.md)
Mark an assigned educationAssignment as inactive to signal that the assignment has no further action items for teachers and students. This action can only be performed by a teacher on assigned assignments.

### [Invoke-MgBetaDeactivateEducationUserAssignment](Invoke-MgBetaDeactivateEducationUserAssignment.md)
Mark an assigned educationAssignment as inactive to signal that the assignment has no further action items for teachers and students. This action can only be performed by a teacher on assigned assignments.

### [Invoke-MgBetaExcuseEducationClassAssignmentSubmission](Invoke-MgBetaExcuseEducationClassAssignmentSubmission.md)
Excuse a submission. Excused submissions aren't included in average grade calculations. Grading rubrics and feedback are deleted. Only teachers can perform this action. If the Prefer: include-unknown-enum-members request header is provided, the excused submission retains the excused status. Otherwise, the submission status changes to returned. For more information about how to use this header, see the Examples section.

### [Invoke-MgBetaExcuseEducationMeAssignmentSubmission](Invoke-MgBetaExcuseEducationMeAssignmentSubmission.md)
Excuse a submission. Excused submissions aren't included in average grade calculations. Grading rubrics and feedback are deleted. Only teachers can perform this action. If the Prefer: include-unknown-enum-members request header is provided, the excused submission retains the excused status. Otherwise, the submission status changes to returned. For more information about how to use this header, see the Examples section.

### [Invoke-MgBetaExcuseEducationUserAssignmentSubmission](Invoke-MgBetaExcuseEducationUserAssignmentSubmission.md)
Excuse a submission. Excused submissions aren't included in average grade calculations. Grading rubrics and feedback are deleted. Only teachers can perform this action. If the Prefer: include-unknown-enum-members request header is provided, the excused submission retains the excused status. Otherwise, the submission status changes to returned. For more information about how to use this header, see the Examples section.

### [Invoke-MgBetaPinEducationClassModule](Invoke-MgBetaPinEducationClassModule.md)
Pin an educationModule in the class work list. This action sets the isPinned property to true for an educationModule. Only teachers can perform this action and only one module at a time can be pinned in the class work list.

### [Invoke-MgBetaReassignEducationClassAssignmentSubmission](Invoke-MgBetaReassignEducationClassAssignmentSubmission.md)
Reassign the submission to the student with feedback for review. Only teachers can perform this action. Include the Prefer: include-unknown-enum-members header when you call this method; otherwise, a reassigned submission will be treated as a returned submission. This means that the reassigned status will be mapped to the returned status, and reassignedDateTime and reassignedBy properties will be mapped to returnedDateTime and returnedBy respectively. If the header Prefer: include-unknown-enum-members is provided, a reassigned submission retains the reassigned status. For details, see the examples section.

### [Invoke-MgBetaReassignEducationMeAssignmentSubmission](Invoke-MgBetaReassignEducationMeAssignmentSubmission.md)
Reassign the submission to the student with feedback for review. Only teachers can perform this action. Include the Prefer: include-unknown-enum-members header when you call this method; otherwise, a reassigned submission will be treated as a returned submission. This means that the reassigned status will be mapped to the returned status, and reassignedDateTime and reassignedBy properties will be mapped to returnedDateTime and returnedBy respectively. If the header Prefer: include-unknown-enum-members is provided, a reassigned submission retains the reassigned status. For details, see the examples section.

### [Invoke-MgBetaReassignEducationUserAssignmentSubmission](Invoke-MgBetaReassignEducationUserAssignmentSubmission.md)
Reassign the submission to the student with feedback for review. Only teachers can perform this action. Include the Prefer: include-unknown-enum-members header when you call this method; otherwise, a reassigned submission will be treated as a returned submission. This means that the reassigned status will be mapped to the returned status, and reassignedDateTime and reassignedBy properties will be mapped to returnedDateTime and returnedBy respectively. If the header Prefer: include-unknown-enum-members is provided, a reassigned submission retains the reassigned status. For details, see the examples section.

### [Invoke-MgBetaReturnEducationClassAssignmentSubmission](Invoke-MgBetaReturnEducationClassAssignmentSubmission.md)
Make the grade and feedback associated with this submission available to the student. This will change the status of the submission from 'submitted' to 'returned' and indicates that feedback is provided or grading is done. This action can only be done by the teacher.

### [Invoke-MgBetaReturnEducationMeAssignmentSubmission](Invoke-MgBetaReturnEducationMeAssignmentSubmission.md)
Make the grade and feedback associated with this submission available to the student. This will change the status of the submission from 'submitted' to 'returned' and indicates that feedback is provided or grading is done. This action can only be done by the teacher.

### [Invoke-MgBetaReturnEducationUserAssignmentSubmission](Invoke-MgBetaReturnEducationUserAssignmentSubmission.md)
Make the grade and feedback associated with this submission available to the student. This will change the status of the submission from 'submitted' to 'returned' and indicates that feedback is provided or grading is done. This action can only be done by the teacher.

### [Invoke-MgBetaUnpinEducationClassModule](Invoke-MgBetaUnpinEducationClassModule.md)
Unpin an educationModule in the classwork list. This action sets the isPinned property to false for an educationModule. Only teachers in the class can perform this operation.

### [Invoke-MgBetaUnsubmitEducationClassAssignmentSubmission](Invoke-MgBetaUnsubmitEducationClassAssignmentSubmission.md)
Indicate that a student wants to work on the submitted assignment after it was turned in. Only teachers, students, and applications with application permissions can perform this operation. This method changes the status of the submission from submitted to working. During the submit process, all the resources are copied from submittedResources to  workingResources. The teacher will be looking at the working resources list for grading. A teacher can also unsubmit a student's assignment on their behalf.

### [Invoke-MgBetaUnsubmitEducationMeAssignmentSubmission](Invoke-MgBetaUnsubmitEducationMeAssignmentSubmission.md)
Indicate that a student wants to work on the submitted assignment after it was turned in. Only teachers, students, and applications with application permissions can perform this operation. This method changes the status of the submission from submitted to working. During the submit process, all the resources are copied from submittedResources to  workingResources. The teacher will be looking at the working resources list for grading. A teacher can also unsubmit a student's assignment on their behalf.

### [Invoke-MgBetaUnsubmitEducationUserAssignmentSubmission](Invoke-MgBetaUnsubmitEducationUserAssignmentSubmission.md)
Indicate that a student wants to work on the submitted assignment after it was turned in. Only teachers, students, and applications with application permissions can perform this operation. This method changes the status of the submission from submitted to working. During the submit process, all the resources are copied from submittedResources to  workingResources. The teacher will be looking at the working resources list for grading. A teacher can also unsubmit a student's assignment on their behalf.

### [New-MgBetaEducationClass](New-MgBetaEducationClass.md)
Create a new class. This will also create a universal group. When you use this API to create a class, it will add special properties to the group, which willadd features such as assignments and special handling within Microsoft Teams when teams are created using the group. Please note that this API only creates the universal group and does not create a team. Microsoft Teams provides a user interface for teachers to create teams for their own classes using the groups created by this API.

### [New-MgBetaEducationClassAssignment](New-MgBetaEducationClassAssignment.md)
Create a new assignment. Only teachers in a class can create an assignment. Assignments start in draft status, which means that students can't see the assignment until it's published.

### [New-MgBetaEducationClassAssignmentCategory](New-MgBetaEducationClassAssignmentCategory.md)
Create a new educationCategory on an educationClass. Only teachers can perform this operation.

### [New-MgBetaEducationClassAssignmentCategoryByRef](New-MgBetaEducationClassAssignmentCategoryByRef.md)
Add one or more existing educationCategory objects to this educationAssignment. Only teachers and students can perform this operation.

### [New-MgBetaEducationClassAssignmentResource](New-MgBetaEducationClassAssignmentResource.md)
Create an assignment resource. Only teachers can perform this operation. You can create the following types of assignment resources: Every resource has an @odata.type property to indicate which type of resource is being created.

### [New-MgBetaEducationClassAssignmentResourceDependentResource](New-MgBetaEducationClassAssignmentResourceDependentResource.md)
Create new navigation property to dependentResources for education

### [New-MgBetaEducationClassAssignmentSettingGradingCategory](New-MgBetaEducationClassAssignmentSettingGradingCategory.md)
Create new navigation property to gradingCategories for education

### [New-MgBetaEducationClassAssignmentSettingGradingScheme](New-MgBetaEducationClassAssignmentSettingGradingScheme.md)
Create a new educationGradingScheme object.

### [New-MgBetaEducationClassAssignmentSubmission](New-MgBetaEducationClassAssignmentSubmission.md)
Create new navigation property to submissions for education

### [New-MgBetaEducationClassAssignmentSubmissionOutcome](New-MgBetaEducationClassAssignmentSubmissionOutcome.md)
Create a new feedback resource for a submission. Only a teacher can perform this operation. To create a new file-based resource, upload the file to the feedback resources folder associated with the assignment. If the file doesn't exist or is not in that folder, the POST request will fail.

### [New-MgBetaEducationClassAssignmentSubmissionResource](New-MgBetaEducationClassAssignmentSubmissionResource.md)
Add a educationSubmissionResource to a submission resource list. Only teachers and students can perform this operation. The operation will not succeed if the allowStudentsToAddResources flag is not set to true. To create a new file-based resource, upload the file to the resources folder associated with the submission. If the file doesn't exist or is not in that folder, the POST request will fail.

### [New-MgBetaEducationClassAssignmentSubmissionResourceDependentResource](New-MgBetaEducationClassAssignmentSubmissionResourceDependentResource.md)
Create new navigation property to dependentResources for education

### [New-MgBetaEducationClassAssignmentSubmissionSubmittedResource](New-MgBetaEducationClassAssignmentSubmissionSubmittedResource.md)
Create new navigation property to submittedResources for education

### [New-MgBetaEducationClassAssignmentSubmissionSubmittedResourceDependentResource](New-MgBetaEducationClassAssignmentSubmissionSubmittedResourceDependentResource.md)
Create new navigation property to dependentResources for education

### [New-MgBetaEducationClassMemberByRef](New-MgBetaEducationClassMemberByRef.md)
Add an educationUser member to an educationClass.

### [New-MgBetaEducationClassModule](New-MgBetaEducationClassModule.md)
Create a new module in a class. Only teachers in a class can create a module. Modules start in the draft state, which means that students won't see the modules until publication.

### [New-MgBetaEducationClassModuleResource](New-MgBetaEducationClassModuleResource.md)
Create a resource in a module. Only teachers can perform this operation. You can create the following types of module resources: Every resource has an @odata.type property to indicate which type of resource is being created.

### [New-MgBetaEducationClassTeacherByRef](New-MgBetaEducationClassTeacherByRef.md)
Add a teacher to a class.

### [New-MgBetaEducationMeAssignment](New-MgBetaEducationMeAssignment.md)
Create new navigation property to assignments for education

### [New-MgBetaEducationMeAssignmentCategory](New-MgBetaEducationMeAssignmentCategory.md)
Create new navigation property to categories for education

### [New-MgBetaEducationMeAssignmentCategoryByRef](New-MgBetaEducationMeAssignmentCategoryByRef.md)
Create new navigation property ref to categories for education

### [New-MgBetaEducationMeAssignmentResource](New-MgBetaEducationMeAssignmentResource.md)
Create new navigation property to resources for education

### [New-MgBetaEducationMeAssignmentResourceDependentResource](New-MgBetaEducationMeAssignmentResourceDependentResource.md)
Create new navigation property to dependentResources for education

### [New-MgBetaEducationMeAssignmentSubmission](New-MgBetaEducationMeAssignmentSubmission.md)
Create new navigation property to submissions for education

### [New-MgBetaEducationMeAssignmentSubmissionOutcome](New-MgBetaEducationMeAssignmentSubmissionOutcome.md)
Create new navigation property to outcomes for education

### [New-MgBetaEducationMeAssignmentSubmissionResource](New-MgBetaEducationMeAssignmentSubmissionResource.md)
Create new navigation property to resources for education

### [New-MgBetaEducationMeAssignmentSubmissionResourceDependentResource](New-MgBetaEducationMeAssignmentSubmissionResourceDependentResource.md)
Create new navigation property to dependentResources for education

### [New-MgBetaEducationMeAssignmentSubmissionSubmittedResource](New-MgBetaEducationMeAssignmentSubmissionSubmittedResource.md)
Create new navigation property to submittedResources for education

### [New-MgBetaEducationMeAssignmentSubmissionSubmittedResourceDependentResource](New-MgBetaEducationMeAssignmentSubmissionSubmittedResourceDependentResource.md)
Create new navigation property to dependentResources for education

### [New-MgBetaEducationMeRubric](New-MgBetaEducationMeRubric.md)
Create a new educationRubric object.

### [New-MgBetaEducationReportReadingAssignmentSubmission](New-MgBetaEducationReportReadingAssignmentSubmission.md)
Create new navigation property to readingAssignmentSubmissions for education

### [New-MgBetaEducationReportReflectCheck](New-MgBetaEducationReportReflectCheck.md)
Create new navigation property to reflectCheckInResponses for education

### [New-MgBetaEducationSchool](New-MgBetaEducationSchool.md)
Create a school.

### [New-MgBetaEducationSchoolClassByRef](New-MgBetaEducationSchoolClassByRef.md)
Add a class to a school.

### [New-MgBetaEducationSchoolUserByRef](New-MgBetaEducationSchoolUserByRef.md)
Add a user to a school.

### [New-MgBetaEducationUser](New-MgBetaEducationUser.md)
Create a new user.

### [New-MgBetaEducationUserAssignment](New-MgBetaEducationUserAssignment.md)
Create new navigation property to assignments for education

### [New-MgBetaEducationUserAssignmentCategory](New-MgBetaEducationUserAssignmentCategory.md)
Create new navigation property to categories for education

### [New-MgBetaEducationUserAssignmentCategoryByRef](New-MgBetaEducationUserAssignmentCategoryByRef.md)
Create new navigation property ref to categories for education

### [New-MgBetaEducationUserAssignmentResource](New-MgBetaEducationUserAssignmentResource.md)
Create new navigation property to resources for education

### [New-MgBetaEducationUserAssignmentResourceDependentResource](New-MgBetaEducationUserAssignmentResourceDependentResource.md)
Create new navigation property to dependentResources for education

### [New-MgBetaEducationUserAssignmentSubmission](New-MgBetaEducationUserAssignmentSubmission.md)
Create new navigation property to submissions for education

### [New-MgBetaEducationUserAssignmentSubmissionOutcome](New-MgBetaEducationUserAssignmentSubmissionOutcome.md)
Create new navigation property to outcomes for education

### [New-MgBetaEducationUserAssignmentSubmissionResource](New-MgBetaEducationUserAssignmentSubmissionResource.md)
Create new navigation property to resources for education

### [New-MgBetaEducationUserAssignmentSubmissionResourceDependentResource](New-MgBetaEducationUserAssignmentSubmissionResourceDependentResource.md)
Create new navigation property to dependentResources for education

### [New-MgBetaEducationUserAssignmentSubmissionSubmittedResource](New-MgBetaEducationUserAssignmentSubmissionSubmittedResource.md)
Create new navigation property to submittedResources for education

### [New-MgBetaEducationUserAssignmentSubmissionSubmittedResourceDependentResource](New-MgBetaEducationUserAssignmentSubmissionSubmittedResourceDependentResource.md)
Create new navigation property to dependentResources for education

### [New-MgBetaEducationUserRubric](New-MgBetaEducationUserRubric.md)
Create new navigation property to rubrics for education

### [Publish-MgBetaEducationClassAssignment](Publish-MgBetaEducationClassAssignment.md)
Change the status of an educationAssignment from its original draft status to the published status. You can change the status from draft to scheduled if the assignment is scheduled for a future date. Only a teacher in the class can make this call. When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects. When you call this API, educationSubmission objects are created and the assignment appears in the student's list. The status of the assignment goes back to draft if there is any backend failure during publish process. To update the properties of a published assignment, see update an assignment. To update the properties of a published assignment, see update an assignment.

### [Publish-MgBetaEducationClassModule](Publish-MgBetaEducationClassModule.md)
Change the state of an educationModule from its original draft status to the published status. Only teachers in the class can perform this operation. When a module is in draft status, students won't see the module. When you call this API, the module appears in the student's class work list.

### [Publish-MgBetaEducationMeAssignment](Publish-MgBetaEducationMeAssignment.md)
Change the status of an educationAssignment from its original draft status to the published status. You can change the status from draft to scheduled if the assignment is scheduled for a future date. Only a teacher in the class can make this call. When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects. When you call this API, educationSubmission objects are created and the assignment appears in the student's list. The status of the assignment goes back to draft if there is any backend failure during publish process. To update the properties of a published assignment, see update an assignment. To update the properties of a published assignment, see update an assignment.

### [Publish-MgBetaEducationUserAssignment](Publish-MgBetaEducationUserAssignment.md)
Change the status of an educationAssignment from its original draft status to the published status. You can change the status from draft to scheduled if the assignment is scheduled for a future date. Only a teacher in the class can make this call. When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects. When you call this API, educationSubmission objects are created and the assignment appears in the student's list. The status of the assignment goes back to draft if there is any backend failure during publish process. To update the properties of a published assignment, see update an assignment. To update the properties of a published assignment, see update an assignment.

### [Remove-MgBetaEducationClass](Remove-MgBetaEducationClass.md)
Delete an educationClass. Because a class is also a universal group, deleting a class deletes the group.

### [Remove-MgBetaEducationClassAssignment](Remove-MgBetaEducationClassAssignment.md)
Delete an existing assignment. Only teachers within a class can delete assignments.

### [Remove-MgBetaEducationClassAssignmentCategory](Remove-MgBetaEducationClassAssignmentCategory.md)
Delete an existing category. Only teachers can perform this operation.

### [Remove-MgBetaEducationClassAssignmentCategoryByRef](Remove-MgBetaEducationClassAssignmentCategoryByRef.md)
Remove an educationCategory from an educationAssignment. Only teachers can perform this operation.

### [Remove-MgBetaEducationClassAssignmentCategoryEducationCategoryByRef](Remove-MgBetaEducationClassAssignmentCategoryEducationCategoryByRef.md)
Remove an educationCategory from an educationAssignment. Only teachers can perform this operation.

### [Remove-MgBetaEducationClassAssignmentDefault](Remove-MgBetaEducationClassAssignmentDefault.md)
Delete navigation property assignmentDefaults for education

### [Remove-MgBetaEducationClassAssignmentResource](Remove-MgBetaEducationClassAssignmentResource.md)
Delete a specific educationAssignmentResource attached to an assignment. Only teachers in the class can remove a resource. After an assignment has been published to students, teachers can't remove resources that are marked as 'distributeToStudents'.

### [Remove-MgBetaEducationClassAssignmentResourceDependentResource](Remove-MgBetaEducationClassAssignmentResourceDependentResource.md)
Delete navigation property dependentResources for education

### [Remove-MgBetaEducationClassAssignmentRubric](Remove-MgBetaEducationClassAssignmentRubric.md)
Delete an educationRubric from an educationAssignment. This method doesn't delete the rubric itself and can only be performed by teachers.

### [Remove-MgBetaEducationClassAssignmentRubricByRef](Remove-MgBetaEducationClassAssignmentRubricByRef.md)
Delete an educationRubric from an educationAssignment. This method doesn't delete the rubric itself and can only be performed by teachers.

### [Remove-MgBetaEducationClassAssignmentSetting](Remove-MgBetaEducationClassAssignmentSetting.md)
Delete navigation property assignmentSettings for education

### [Remove-MgBetaEducationClassAssignmentSettingGradingCategory](Remove-MgBetaEducationClassAssignmentSettingGradingCategory.md)
Delete navigation property gradingCategories for education

### [Remove-MgBetaEducationClassAssignmentSettingGradingScheme](Remove-MgBetaEducationClassAssignmentSettingGradingScheme.md)
Delete an educationGradingScheme object.

### [Remove-MgBetaEducationClassAssignmentSubmission](Remove-MgBetaEducationClassAssignmentSubmission.md)
Delete navigation property submissions for education

### [Remove-MgBetaEducationClassAssignmentSubmissionOutcome](Remove-MgBetaEducationClassAssignmentSubmissionOutcome.md)
Delete a feedback resource from a submission. This can only be done by a teacher.

### [Remove-MgBetaEducationClassAssignmentSubmissionResource](Remove-MgBetaEducationClassAssignmentSubmissionResource.md)
Delete an educationSubmissionResource from the submission. Only teachers and students can perform this operation. If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted. This allows you to 'reset' the resource to its original state. If the resource wasn't copied from the assignment but was added from the student, the resource is deleted.

### [Remove-MgBetaEducationClassAssignmentSubmissionResourceDependentResource](Remove-MgBetaEducationClassAssignmentSubmissionResourceDependentResource.md)
Delete navigation property dependentResources for education

### [Remove-MgBetaEducationClassAssignmentSubmissionSubmittedResource](Remove-MgBetaEducationClassAssignmentSubmissionSubmittedResource.md)
Delete navigation property submittedResources for education

### [Remove-MgBetaEducationClassAssignmentSubmissionSubmittedResourceDependentResource](Remove-MgBetaEducationClassAssignmentSubmissionSubmittedResourceDependentResource.md)
Delete navigation property dependentResources for education

### [Remove-MgBetaEducationClassMemberByRef](Remove-MgBetaEducationClassMemberByRef.md)
Remove an educationUser from an educationClass.

### [Remove-MgBetaEducationClassMemberEducationUserByRef](Remove-MgBetaEducationClassMemberEducationUserByRef.md)
Remove an educationUser from an educationClass.

### [Remove-MgBetaEducationClassModule](Remove-MgBetaEducationClassModule.md)
Delete an existing module in a class. Only teachers within a class can delete modules.

### [Remove-MgBetaEducationClassModuleResource](Remove-MgBetaEducationClassModuleResource.md)
Delete a specific educationModuleResource attached to a module. Only teachers in the class can remove a resource.

### [Remove-MgBetaEducationClassTeacherByRef](Remove-MgBetaEducationClassTeacherByRef.md)
Remove a teacher from an educationClass.

### [Remove-MgBetaEducationClassTeacherEducationUserByRef](Remove-MgBetaEducationClassTeacherEducationUserByRef.md)
Remove a teacher from an educationClass.

### [Remove-MgBetaEducationMe](Remove-MgBetaEducationMe.md)
Delete navigation property me for education

### [Remove-MgBetaEducationMeAssignment](Remove-MgBetaEducationMeAssignment.md)
Delete navigation property assignments for education

### [Remove-MgBetaEducationMeAssignmentCategoryByRef](Remove-MgBetaEducationMeAssignmentCategoryByRef.md)
Delete ref of navigation property categories for education

### [Remove-MgBetaEducationMeAssignmentCategoryEducationCategoryByRef](Remove-MgBetaEducationMeAssignmentCategoryEducationCategoryByRef.md)
Delete ref of navigation property categories for education

### [Remove-MgBetaEducationMeAssignmentResource](Remove-MgBetaEducationMeAssignmentResource.md)
Delete navigation property resources for education

### [Remove-MgBetaEducationMeAssignmentResourceDependentResource](Remove-MgBetaEducationMeAssignmentResourceDependentResource.md)
Delete navigation property dependentResources for education

### [Remove-MgBetaEducationMeAssignmentRubric](Remove-MgBetaEducationMeAssignmentRubric.md)
Delete navigation property rubric for education

### [Remove-MgBetaEducationMeAssignmentRubricByRef](Remove-MgBetaEducationMeAssignmentRubricByRef.md)
Delete ref of navigation property rubric for education

### [Remove-MgBetaEducationMeAssignmentSubmission](Remove-MgBetaEducationMeAssignmentSubmission.md)
Delete navigation property submissions for education

### [Remove-MgBetaEducationMeAssignmentSubmissionOutcome](Remove-MgBetaEducationMeAssignmentSubmissionOutcome.md)
Delete navigation property outcomes for education

### [Remove-MgBetaEducationMeAssignmentSubmissionResource](Remove-MgBetaEducationMeAssignmentSubmissionResource.md)
Delete navigation property resources for education

### [Remove-MgBetaEducationMeAssignmentSubmissionResourceDependentResource](Remove-MgBetaEducationMeAssignmentSubmissionResourceDependentResource.md)
Delete navigation property dependentResources for education

### [Remove-MgBetaEducationMeAssignmentSubmissionSubmittedResource](Remove-MgBetaEducationMeAssignmentSubmissionSubmittedResource.md)
Delete navigation property submittedResources for education

### [Remove-MgBetaEducationMeAssignmentSubmissionSubmittedResourceDependentResource](Remove-MgBetaEducationMeAssignmentSubmissionSubmittedResourceDependentResource.md)
Delete navigation property dependentResources for education

### [Remove-MgBetaEducationMeRubric](Remove-MgBetaEducationMeRubric.md)
Delete an educationRubric object. Only teachers can perform this operation.

### [Remove-MgBetaEducationReport](Remove-MgBetaEducationReport.md)
Delete navigation property reports for education

### [Remove-MgBetaEducationReportReadingAssignmentSubmission](Remove-MgBetaEducationReportReadingAssignmentSubmission.md)
Delete navigation property readingAssignmentSubmissions for education

### [Remove-MgBetaEducationReportReflectCheck](Remove-MgBetaEducationReportReflectCheck.md)
Delete navigation property reflectCheckInResponses for education

### [Remove-MgBetaEducationSchool](Remove-MgBetaEducationSchool.md)
Delete a school.

### [Remove-MgBetaEducationSchoolClassByRef](Remove-MgBetaEducationSchoolClassByRef.md)
Delete a class from a school.

### [Remove-MgBetaEducationSchoolClassEducationClassByRef](Remove-MgBetaEducationSchoolClassEducationClassByRef.md)
Delete a class from a school.

### [Remove-MgBetaEducationSchoolUserByRef](Remove-MgBetaEducationSchoolUserByRef.md)
Delete a user from a school.

### [Remove-MgBetaEducationSchoolUserEducationUserByRef](Remove-MgBetaEducationSchoolUserEducationUserByRef.md)
Delete a user from a school.

### [Remove-MgBetaEducationUser](Remove-MgBetaEducationUser.md)
Delete a user.

### [Remove-MgBetaEducationUserAssignment](Remove-MgBetaEducationUserAssignment.md)
Delete navigation property assignments for education

### [Remove-MgBetaEducationUserAssignmentCategoryByRef](Remove-MgBetaEducationUserAssignmentCategoryByRef.md)
Delete ref of navigation property categories for education

### [Remove-MgBetaEducationUserAssignmentCategoryEducationCategoryByRef](Remove-MgBetaEducationUserAssignmentCategoryEducationCategoryByRef.md)
Delete ref of navigation property categories for education

### [Remove-MgBetaEducationUserAssignmentResource](Remove-MgBetaEducationUserAssignmentResource.md)
Delete navigation property resources for education

### [Remove-MgBetaEducationUserAssignmentResourceDependentResource](Remove-MgBetaEducationUserAssignmentResourceDependentResource.md)
Delete navigation property dependentResources for education

### [Remove-MgBetaEducationUserAssignmentRubric](Remove-MgBetaEducationUserAssignmentRubric.md)
Delete navigation property rubric for education

### [Remove-MgBetaEducationUserAssignmentRubricByRef](Remove-MgBetaEducationUserAssignmentRubricByRef.md)
Delete ref of navigation property rubric for education

### [Remove-MgBetaEducationUserAssignmentSubmission](Remove-MgBetaEducationUserAssignmentSubmission.md)
Delete navigation property submissions for education

### [Remove-MgBetaEducationUserAssignmentSubmissionOutcome](Remove-MgBetaEducationUserAssignmentSubmissionOutcome.md)
Delete navigation property outcomes for education

### [Remove-MgBetaEducationUserAssignmentSubmissionResource](Remove-MgBetaEducationUserAssignmentSubmissionResource.md)
Delete navigation property resources for education

### [Remove-MgBetaEducationUserAssignmentSubmissionResourceDependentResource](Remove-MgBetaEducationUserAssignmentSubmissionResourceDependentResource.md)
Delete navigation property dependentResources for education

### [Remove-MgBetaEducationUserAssignmentSubmissionSubmittedResource](Remove-MgBetaEducationUserAssignmentSubmissionSubmittedResource.md)
Delete navigation property submittedResources for education

### [Remove-MgBetaEducationUserAssignmentSubmissionSubmittedResourceDependentResource](Remove-MgBetaEducationUserAssignmentSubmissionSubmittedResourceDependentResource.md)
Delete navigation property dependentResources for education

### [Remove-MgBetaEducationUserRubric](Remove-MgBetaEducationUserRubric.md)
Delete navigation property rubrics for education

### [Set-MgBetaEducationClassAssignmentRubricByRef](Set-MgBetaEducationClassAssignmentRubricByRef.md)
Attach an existing educationRubric object to an educationAssignment. Only teachers can perform this operation.

### [Set-MgBetaEducationClassAssignmentSubmissionUpResourceFolder](Set-MgBetaEducationClassAssignmentSubmissionUpResourceFolder.md)
Trigger the creation of the SharePoint resource folder where all file-based resources (Word, Excel, and so on) should be uploaded for a given submission. Only teachers and students can perform this operation. Note that files must be located in this folder in order to be added as resources. Only a student in the class can determine what files to upload in a given submission-level resource folder.

### [Set-MgBetaEducationClassAssignmentUpFeedbackResourceFolder](Set-MgBetaEducationClassAssignmentUpFeedbackResourceFolder.md)
Create a SharePoint folder to upload feedback files for a given educationSubmission. Only teachers can perform this operation. The teacher determines the resources to upload in the feedback resources folder of a submission.

### [Set-MgBetaEducationClassAssignmentUpResourceFolder](Set-MgBetaEducationClassAssignmentUpResourceFolder.md)
Create a SharePoint folder to upload files for a given educationAssignment. Only teachers can perform this operation. The teacher determines the resources to upload in the assignment's folder.

### [Set-MgBetaEducationClassModuleUpResourceFolder](Set-MgBetaEducationClassModuleUpResourceFolder.md)
Create a SharePoint folder to upload files for a given educationModule. Only teachers can perform this operation. The teacher determines what resources to upload to the SharePoint folder for the module.

### [Set-MgBetaEducationMeAssignmentRubricByRef](Set-MgBetaEducationMeAssignmentRubricByRef.md)
Update the ref of navigation property rubric in education

### [Set-MgBetaEducationMeAssignmentSubmissionUpResourceFolder](Set-MgBetaEducationMeAssignmentSubmissionUpResourceFolder.md)
Trigger the creation of the SharePoint resource folder where all file-based resources (Word, Excel, and so on) should be uploaded for a given submission. Only teachers and students can perform this operation. Note that files must be located in this folder in order to be added as resources. Only a student in the class can determine what files to upload in a given submission-level resource folder.

### [Set-MgBetaEducationMeAssignmentUpFeedbackResourceFolder](Set-MgBetaEducationMeAssignmentUpFeedbackResourceFolder.md)
Create a SharePoint folder to upload feedback files for a given educationSubmission. Only teachers can perform this operation. The teacher determines the resources to upload in the feedback resources folder of a submission.

### [Set-MgBetaEducationMeAssignmentUpResourceFolder](Set-MgBetaEducationMeAssignmentUpResourceFolder.md)
Create a SharePoint folder to upload files for a given educationAssignment. Only teachers can perform this operation. The teacher determines the resources to upload in the assignment's folder.

### [Set-MgBetaEducationUserAssignmentRubricByRef](Set-MgBetaEducationUserAssignmentRubricByRef.md)
Update the ref of navigation property rubric in education

### [Set-MgBetaEducationUserAssignmentSubmissionUpResourceFolder](Set-MgBetaEducationUserAssignmentSubmissionUpResourceFolder.md)
Trigger the creation of the SharePoint resource folder where all file-based resources (Word, Excel, and so on) should be uploaded for a given submission. Only teachers and students can perform this operation. Note that files must be located in this folder in order to be added as resources. Only a student in the class can determine what files to upload in a given submission-level resource folder.

### [Set-MgBetaEducationUserAssignmentUpFeedbackResourceFolder](Set-MgBetaEducationUserAssignmentUpFeedbackResourceFolder.md)
Create a SharePoint folder to upload feedback files for a given educationSubmission. Only teachers can perform this operation. The teacher determines the resources to upload in the feedback resources folder of a submission.

### [Set-MgBetaEducationUserAssignmentUpResourceFolder](Set-MgBetaEducationUserAssignmentUpResourceFolder.md)
Create a SharePoint folder to upload files for a given educationAssignment. Only teachers can perform this operation. The teacher determines the resources to upload in the assignment's folder.

### [Submit-MgBetaEducationClassAssignmentSubmission](Submit-MgBetaEducationClassAssignmentSubmission.md)
Indicate that a student is done with the work and is ready to hand in the assignment. Only teachers, students, and applications with application permissions can perform this operation. This method changes the status of the submission from working to submitted. During the submit process, all the resources are copied to the submittedResources bucket. The teacher will be looking at the submitted resources list for grading. A teacher can also submit a student's assignment on their behalf.

### [Submit-MgBetaEducationMeAssignmentSubmission](Submit-MgBetaEducationMeAssignmentSubmission.md)
Indicate that a student is done with the work and is ready to hand in the assignment. Only teachers, students, and applications with application permissions can perform this operation. This method changes the status of the submission from working to submitted. During the submit process, all the resources are copied to the submittedResources bucket. The teacher will be looking at the submitted resources list for grading. A teacher can also submit a student's assignment on their behalf.

### [Submit-MgBetaEducationUserAssignmentSubmission](Submit-MgBetaEducationUserAssignmentSubmission.md)
Indicate that a student is done with the work and is ready to hand in the assignment. Only teachers, students, and applications with application permissions can perform this operation. This method changes the status of the submission from working to submitted. During the submit process, all the resources are copied to the submittedResources bucket. The teacher will be looking at the submitted resources list for grading. A teacher can also submit a student's assignment on their behalf.

### [Update-MgBetaEducationClass](Update-MgBetaEducationClass.md)
Update the properties of a class.

### [Update-MgBetaEducationClassAssignment](Update-MgBetaEducationClassAssignment.md)
Update an educationAssignment object. Only teachers in the class can do this. You can't use a PATCH request to change the status of an assignment. Use the publish action to change the assignment status.

### [Update-MgBetaEducationClassAssignmentCategory](Update-MgBetaEducationClassAssignmentCategory.md)
Update the navigation property assignmentCategories in education

### [Update-MgBetaEducationClassAssignmentDefault](Update-MgBetaEducationClassAssignmentDefault.md)
Update the properties of an educationAssignmentDefaults object. Only teachers can update these settings.

### [Update-MgBetaEducationClassAssignmentResource](Update-MgBetaEducationClassAssignmentResource.md)
Update the navigation property resources in education

### [Update-MgBetaEducationClassAssignmentResourceDependentResource](Update-MgBetaEducationClassAssignmentResourceDependentResource.md)
Update the navigation property dependentResources in education

### [Update-MgBetaEducationClassAssignmentRubric](Update-MgBetaEducationClassAssignmentRubric.md)
Attach an existing educationRubric object to an educationAssignment. Only teachers can perform this operation.

### [Update-MgBetaEducationClassAssignmentSetting](Update-MgBetaEducationClassAssignmentSetting.md)
Update the properties of an educationAssignmentSettings object. Only teachers can update these settings.

### [Update-MgBetaEducationClassAssignmentSettingGradingCategory](Update-MgBetaEducationClassAssignmentSettingGradingCategory.md)
Update a single gradingCategory on the educationAssignmentSettings. Only teachers can perform this operation.

### [Update-MgBetaEducationClassAssignmentSettingGradingScheme](Update-MgBetaEducationClassAssignmentSettingGradingScheme.md)
Update the navigation property gradingSchemes in education

### [Update-MgBetaEducationClassAssignmentSubmission](Update-MgBetaEducationClassAssignmentSubmission.md)
Update the navigation property submissions in education

### [Update-MgBetaEducationClassAssignmentSubmissionOutcome](Update-MgBetaEducationClassAssignmentSubmissionOutcome.md)
Update the properties of an educationOutcome object. Only teachers can perform this operation.

### [Update-MgBetaEducationClassAssignmentSubmissionResource](Update-MgBetaEducationClassAssignmentSubmissionResource.md)
Update the navigation property resources in education

### [Update-MgBetaEducationClassAssignmentSubmissionResourceDependentResource](Update-MgBetaEducationClassAssignmentSubmissionResourceDependentResource.md)
Update the navigation property dependentResources in education

### [Update-MgBetaEducationClassAssignmentSubmissionSubmittedResource](Update-MgBetaEducationClassAssignmentSubmissionSubmittedResource.md)
Update the navigation property submittedResources in education

### [Update-MgBetaEducationClassAssignmentSubmissionSubmittedResourceDependentResource](Update-MgBetaEducationClassAssignmentSubmissionSubmittedResourceDependentResource.md)
Update the navigation property dependentResources in education

### [Update-MgBetaEducationClassModule](Update-MgBetaEducationClassModule.md)
Update an educationModule object in a class. Only teachers in the class can perform this operation. Note that you can't use a PATCH request to change the status of a module. Use the publish action to change the module status.

### [Update-MgBetaEducationClassModuleResource](Update-MgBetaEducationClassModuleResource.md)
Update a resource in a module. Only teachers can perform this operation. The only one property that can be updated is displayName, for all resource types.

### [Update-MgBetaEducationMe](Update-MgBetaEducationMe.md)
Update the navigation property me in education

### [Update-MgBetaEducationMeAssignment](Update-MgBetaEducationMeAssignment.md)
Update the navigation property assignments in education

### [Update-MgBetaEducationMeAssignmentResource](Update-MgBetaEducationMeAssignmentResource.md)
Update the navigation property resources in education

### [Update-MgBetaEducationMeAssignmentResourceDependentResource](Update-MgBetaEducationMeAssignmentResourceDependentResource.md)
Update the navigation property dependentResources in education

### [Update-MgBetaEducationMeAssignmentRubric](Update-MgBetaEducationMeAssignmentRubric.md)
Update the navigation property rubric in education

### [Update-MgBetaEducationMeAssignmentSubmission](Update-MgBetaEducationMeAssignmentSubmission.md)
Update the navigation property submissions in education

### [Update-MgBetaEducationMeAssignmentSubmissionOutcome](Update-MgBetaEducationMeAssignmentSubmissionOutcome.md)
Update the navigation property outcomes in education

### [Update-MgBetaEducationMeAssignmentSubmissionResource](Update-MgBetaEducationMeAssignmentSubmissionResource.md)
Update the navigation property resources in education

### [Update-MgBetaEducationMeAssignmentSubmissionResourceDependentResource](Update-MgBetaEducationMeAssignmentSubmissionResourceDependentResource.md)
Update the navigation property dependentResources in education

### [Update-MgBetaEducationMeAssignmentSubmissionSubmittedResource](Update-MgBetaEducationMeAssignmentSubmissionSubmittedResource.md)
Update the navigation property submittedResources in education

### [Update-MgBetaEducationMeAssignmentSubmissionSubmittedResourceDependentResource](Update-MgBetaEducationMeAssignmentSubmissionSubmittedResourceDependentResource.md)
Update the navigation property dependentResources in education

### [Update-MgBetaEducationMeRubric](Update-MgBetaEducationMeRubric.md)
Update the properties of an educationRubric object. Only teachers can perform this operation. Updating a rubric attached to an assignment (PATCH /education/classes/{id}/assignments/{id}/rubric) is only possible before the assignment is published, and what is updated is actually the original rubric that exists under /education/users/{id}/rubrics. After the assignment is published, an immutable copy of the rubric is made that is attached to that specific assignment. That rubric can be retrieved using GET /education/classes/{id}/assignments/{id}/rubric, but it can't be updated.

### [Update-MgBetaEducationMeUserMailboxSetting](Update-MgBetaEducationMeUserMailboxSetting.md)
Update property mailboxSettings value.

### [Update-MgBetaEducationReport](Update-MgBetaEducationReport.md)
Update the navigation property reports in education

### [Update-MgBetaEducationReportReadingAssignmentSubmission](Update-MgBetaEducationReportReadingAssignmentSubmission.md)
Update the navigation property readingAssignmentSubmissions in education

### [Update-MgBetaEducationReportReflectCheck](Update-MgBetaEducationReportReflectCheck.md)
Update the navigation property reflectCheckInResponses in education

### [Update-MgBetaEducationRoot](Update-MgBetaEducationRoot.md)
Update education

### [Update-MgBetaEducationSchool](Update-MgBetaEducationSchool.md)
Update the properties of a school object.

### [Update-MgBetaEducationSchoolAdministrativeUnit](Update-MgBetaEducationSchoolAdministrativeUnit.md)
Update the navigation property administrativeUnit in education

### [Update-MgBetaEducationUser](Update-MgBetaEducationUser.md)
Update the properties of an educationuser object.

### [Update-MgBetaEducationUserAssignment](Update-MgBetaEducationUserAssignment.md)
Update the navigation property assignments in education

### [Update-MgBetaEducationUserAssignmentResource](Update-MgBetaEducationUserAssignmentResource.md)
Update the navigation property resources in education

### [Update-MgBetaEducationUserAssignmentResourceDependentResource](Update-MgBetaEducationUserAssignmentResourceDependentResource.md)
Update the navigation property dependentResources in education

### [Update-MgBetaEducationUserAssignmentRubric](Update-MgBetaEducationUserAssignmentRubric.md)
Update the navigation property rubric in education

### [Update-MgBetaEducationUserAssignmentSubmission](Update-MgBetaEducationUserAssignmentSubmission.md)
Update the navigation property submissions in education

### [Update-MgBetaEducationUserAssignmentSubmissionOutcome](Update-MgBetaEducationUserAssignmentSubmissionOutcome.md)
Update the navigation property outcomes in education

### [Update-MgBetaEducationUserAssignmentSubmissionResource](Update-MgBetaEducationUserAssignmentSubmissionResource.md)
Update the navigation property resources in education

### [Update-MgBetaEducationUserAssignmentSubmissionResourceDependentResource](Update-MgBetaEducationUserAssignmentSubmissionResourceDependentResource.md)
Update the navigation property dependentResources in education

### [Update-MgBetaEducationUserAssignmentSubmissionSubmittedResource](Update-MgBetaEducationUserAssignmentSubmissionSubmittedResource.md)
Update the navigation property submittedResources in education

### [Update-MgBetaEducationUserAssignmentSubmissionSubmittedResourceDependentResource](Update-MgBetaEducationUserAssignmentSubmissionSubmittedResourceDependentResource.md)
Update the navigation property dependentResources in education

### [Update-MgBetaEducationUserMailboxSetting](Update-MgBetaEducationUserMailboxSetting.md)
Update property mailboxSettings value.

### [Update-MgBetaEducationUserRubric](Update-MgBetaEducationUserRubric.md)
Update the navigation property rubrics in education
