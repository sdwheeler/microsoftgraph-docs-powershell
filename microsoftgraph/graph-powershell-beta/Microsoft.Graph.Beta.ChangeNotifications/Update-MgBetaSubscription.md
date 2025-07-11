---
external help file: Microsoft.Graph.Beta.ChangeNotifications-help.xml
Module Name: Microsoft.Graph.Beta.ChangeNotifications
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.changenotifications/update-mgbetasubscription
schema: 2.0.0
ms.subservice: change-notifications
---

# Update-MgBetaSubscription

## SYNOPSIS
Renew a subscription by extending its expiry time.
The table in the Permissions section lists the resources that support subscribing to change notifications.
Subscriptions expire after a length of time that varies by resource type.
In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.
See subscription for maximum length of a subscription for each resource type.

> [!NOTE]
> To view the v1.0 release of this cmdlet, view [Update-MgSubscription](/powershell/module/Microsoft.Graph.ChangeNotifications/Update-MgSubscription?view=graph-powershell-1.0)

## SYNTAX

### UpdateExpanded (Default)
```
Update-MgBetaSubscription -SubscriptionId <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ApplicationId <String>] [-ChangeType <String>] [-ClientState <String>]
 [-CreatorId <String>] [-EncryptionCertificate <String>] [-EncryptionCertificateId <String>]
 [-ExpirationDateTime <DateTime>] [-Id <String>] [-IncludeResourceData] [-LatestSupportedTlsVersion <String>]
 [-LifecycleNotificationUrl <String>] [-NotificationContentType <String>] [-NotificationQueryOptions <String>]
 [-NotificationUrl <String>] [-NotificationUrlAppId <String>] [-Resource <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Update
```
Update-MgBetaSubscription -SubscriptionId <String> -BodyParameter <IMicrosoftGraphSubscription>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-MgBetaSubscription -InputObject <IChangeNotificationsIdentity> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-ApplicationId <String>] [-ChangeType <String>] [-ClientState <String>]
 [-CreatorId <String>] [-EncryptionCertificate <String>] [-EncryptionCertificateId <String>]
 [-ExpirationDateTime <DateTime>] [-Id <String>] [-IncludeResourceData] [-LatestSupportedTlsVersion <String>]
 [-LifecycleNotificationUrl <String>] [-NotificationContentType <String>] [-NotificationQueryOptions <String>]
 [-NotificationUrl <String>] [-NotificationUrlAppId <String>] [-Resource <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-MgBetaSubscription -InputObject <IChangeNotificationsIdentity>
 -BodyParameter <IMicrosoftGraphSubscription> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Renew a subscription by extending its expiry time.
The table in the Permissions section lists the resources that support subscribing to change notifications.
Subscriptions expire after a length of time that varies by resource type.
In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.
See subscription for maximum length of a subscription for each resource type.

## EXAMPLES
### Example 1: Code snippet

```powershell

Import-Module Microsoft.Graph.Beta.ChangeNotifications

$params = @{
	expirationDateTime = [System.DateTime]::Parse("2016-11-22T18:23:45.9356913Z")
}

Update-MgBetaSubscription -SubscriptionId $subscriptionId -BodyParameter $params

```
This example shows how to use the Update-MgBetaSubscription Cmdlet.


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

### -ApplicationId
Optional.
Identifier of the application used to create the subscription.
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

### -BodyParameter
subscription
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphSubscription
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ChangeType
Required.
Indicates the type of change in the subscribed resource that raises a change notification.
The supported values are: created, updated, deleted.
Multiple values can be combined using a comma-separated list.
Note: Drive root item and list change notifications support only the updated changeType.
User and group change notifications support updated and deleted changeType.
Use updated to receive notifications when user or group is created, updated, or soft deleted.
Use deleted to receive notifications when user or group is permanently deleted.

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

### -ClientState
Optional.
Specifies the value of the clientState property sent by the service in each change notification.
The maximum length is 255 characters.
The client can check that the change notification came from the service by comparing the value of the clientState property sent with the subscription with the value of the clientState property received with each change notification.

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

### -CreatorId
Optional.
Identifier of the user or service principal that created the subscription.
If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.
If the app used application permissions, this field contains the ID of the service principal corresponding to the app.
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

### -EncryptionCertificate
Optional.
A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.
Optional but required when includeResourceData is true.

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

### -EncryptionCertificateId
Optional.
A custom app-provided identifier to help identify the certificate needed to decrypt resource data.
Required when includeResourceData is true.

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

### -ExpirationDateTime
Required.
Specifies the date and time when the webhook subscription expires.
The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.
For the maximum supported subscription length of time, see Subscription lifetime.

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

### -IncludeResourceData
Optional.
When set to true, change notifications include resource data (such as content of a chat message).

```yaml
Type: SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: IChangeNotificationsIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -LatestSupportedTlsVersion
Optional.
Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by notificationUrl, supports.
The possible values are: v10, v11, v12, v13.
For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set timeline allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.
For these subscribers, not setting this property per the timeline would result in subscription operations failing.
For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.
In such cases, Microsoft Graph defaults the property to v1_2.

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

### -LifecycleNotificationUrl
Required for Teams resources if the expirationDateTime value is more than 1 hour from now; optional otherwise.
The URL of the endpoint that receives lifecycle notifications, including subscriptionRemoved, reauthorizationRequired, and missed notifications.
This URL must make use of the HTTPS protocol.
For more information, see Reduce missing subscriptions and change notifications.

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

### -NotificationContentType
Optional.
Desired content-type for Microsoft Graph change notifications for supported resource types.
The default content-type is application/json.

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

### -NotificationQueryOptions
Optional.
OData query options for specifying the value for the targeting resource.
Clients receive notifications when the resource reaches the state matching the query options provided here.
With this new property in the subscription creation payload along with all existing properties, Webhooks deliver notifications whenever a resource reaches the desired state mentioned in the notificationQueryOptions property.
For example, when the print job is completed or when a print job resource isFetchable property value becomes true etc.
Supported only for Universal Print Service.
For more information, see Subscribe to change notifications from cloud printing APIs using Microsoft Graph.

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

### -NotificationUrl
Required.
The URL of the endpoint that receives the change notifications.
This URL must make use of the HTTPS protocol.
Any query string parameter included in the notificationUrl property is included in the HTTP POST request when Microsoft Graph sends the change notifications.

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

### -NotificationUrlAppId
Optional.
The app ID that the subscription service can use to generate the validation token.
The value allows the client to validate the authenticity of the notification received.

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

### -Resource
Required.
Specifies the resource that is monitored for changes.
Don't include the base URL (https://graph.microsoft.com/beta/).
See the possible resource path values for each supported resource.

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

### -SubscriptionId
The unique identifier of subscription

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

### Microsoft.Graph.Beta.PowerShell.Models.IChangeNotificationsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSubscription
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphSubscription
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphSubscription>`: subscription
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Id <String>]`: The unique identifier for an entity.
Read-only.
  - `[ApplicationId <String>]`: Optional.
Identifier of the application used to create the subscription.
Read-only.
  - `[ChangeType <String>]`: Required.
Indicates the type of change in the subscribed resource that raises a change notification.
The supported values are: created, updated, deleted.
Multiple values can be combined using a comma-separated list.
Note:  Drive root item and list change notifications support only the updated changeType.
User and group change notifications support updated and deleted changeType.
Use updated to receive notifications when user or group is created, updated, or soft deleted.
Use deleted to receive notifications when user or group is permanently deleted.
  - `[ClientState <String>]`: Optional.
Specifies the value of the clientState property sent by the service in each change notification.
The maximum length is 255 characters.
The client can check that the change notification came from the service by comparing the value of the clientState property sent with the subscription with the value of the clientState property received with each change notification.
  - `[CreatorId <String>]`: Optional.
Identifier of the user or service principal that created the subscription.
If the app used delegated permissions to create the subscription, this field contains the ID of the signed-in user the app called on behalf of.
If the app used application permissions, this field contains the ID of the service principal corresponding to the app.
Read-only.
  - `[EncryptionCertificate <String>]`: Optional.
A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications.
Optional but required when includeResourceData is true.
  - `[EncryptionCertificateId <String>]`: Optional.
A custom app-provided identifier to help identify the certificate needed to decrypt resource data.
Required when includeResourceData is true.
  - `[ExpirationDateTime <DateTime?>]`: Required.
Specifies the date and time when the webhook subscription expires.
The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.
For the maximum supported subscription length of time, see Subscription lifetime.
  - `[IncludeResourceData <Boolean?>]`: Optional.
When set to true, change notifications include resource data (such as content of a chat message).
  - `[LatestSupportedTlsVersion <String>]`: Optional.
Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint, specified by notificationUrl, supports.
The possible values are: v10, v11, v12, v13.
For subscribers whose notification endpoint supports a version lower than the currently recommended version (TLS 1.2), specifying this property by a set timeline allows them to temporarily use their deprecated version of TLS before completing their upgrade to TLS 1.2.
For these subscribers, not setting this property per the timeline would result in subscription operations failing.
For subscribers whose notification endpoint already supports TLS 1.2, setting this property is optional.
In such cases, Microsoft Graph defaults the property to v1_2.
  - `[LifecycleNotificationUrl <String>]`: Required for Teams resources if the expirationDateTime value is more than 1 hour from now; optional otherwise.
The URL of the endpoint that receives lifecycle notifications, including subscriptionRemoved, reauthorizationRequired, and missed notifications.
This URL must make use of the HTTPS protocol.
For more information, see Reduce missing subscriptions and change notifications.
  - `[NotificationContentType <String>]`: Optional.
Desired content-type for Microsoft Graph change notifications for supported resource types.
The default content-type is application/json.
  - `[NotificationQueryOptions <String>]`: Optional.
OData query options for specifying the value for the targeting resource.
Clients receive notifications when the resource reaches the state matching the query options provided here.
With this new property in the subscription creation payload along with all existing properties, Webhooks deliver notifications whenever a resource reaches the desired state mentioned in the notificationQueryOptions property.
For example, when the print job is completed or when a print job resource isFetchable property value becomes true etc. 
Supported only for Universal Print Service.
For more information, see Subscribe to change notifications from cloud printing APIs using Microsoft Graph.
  - `[NotificationUrl <String>]`: Required.
The URL of the endpoint that receives the change notifications.
This URL must make use of the HTTPS protocol.
Any query string parameter included in the notificationUrl property is included in the HTTP POST request when Microsoft Graph sends the change notifications.
  - `[NotificationUrlAppId <String>]`: Optional.
The app ID that the subscription service can use to generate the validation token.
The value allows the client to validate the authenticity of the notification received.
  - `[Resource <String>]`: Required.
Specifies the resource that is monitored for changes.
Don't include the base URL (https://graph.microsoft.com/beta/).
See the possible resource path values for each supported resource.

INPUTOBJECT `<IChangeNotificationsIdentity>`: Identity Parameter
  - `[SubscriptionId <String>]`: The unique identifier of subscription

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.changenotifications/update-mgbetasubscription](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.changenotifications/update-mgbetasubscription)

[https://learn.microsoft.com/graph/api/subscription-update?view=graph-rest-beta](https://learn.microsoft.com/graph/api/subscription-update?view=graph-rest-beta)























