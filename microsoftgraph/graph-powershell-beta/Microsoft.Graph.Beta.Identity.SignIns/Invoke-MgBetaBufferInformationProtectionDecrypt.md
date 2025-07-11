---
external help file: Microsoft.Graph.Beta.Identity.SignIns-help.xml
Module Name: Microsoft.Graph.Beta.Identity.SignIns
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/invoke-mgbetabufferinformationprotectiondecrypt
schema: 2.0.0
---

# Invoke-MgBetaBufferInformationProtectionDecrypt

## SYNOPSIS
Invoke action decryptBuffer

## SYNTAX

### BufferExpanded (Default)
```
Invoke-MgBetaBufferInformationProtectionDecrypt -OutFile <String> [-ResponseHeadersVariable <String>]
 [-AdditionalProperties <Hashtable>] [-EncryptedBufferInputFile <String>]
 [-PublishingLicenseInputFile <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Buffer
```
Invoke-MgBetaBufferInformationProtectionDecrypt -OutFile <String>
 -Body <IPaths41K0CwInformationprotectionMicrosoftGraphDecryptbufferPostRequestbodyContentApplicationJsonSchema>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-PassThru]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Invoke action decryptBuffer

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: BufferExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Body

To construct, see NOTES section for BODY properties and create a hash table.

```yaml
Type: IPaths41K0CwInformationprotectionMicrosoftGraphDecryptbufferPostRequestbodyContentApplicationJsonSchema
Parameter Sets: Buffer
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

### -EncryptedBufferInputFile
Input File for EncryptedBuffer (.)

```yaml
Type: String
Parameter Sets: BufferExpanded
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

### -PublishingLicenseInputFile
Input File for PublishingLicense (.)

```yaml
Type: String
Parameter Sets: BufferExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IPaths41K0CwInformationprotectionMicrosoftGraphDecryptbufferPostRequestbodyContentApplicationJsonSchema
### System.Collections.IDictionary
## OUTPUTS

### System.Boolean
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODY `<IPaths41K0CwInformationprotectionMicrosoftGraphDecryptbufferPostRequestbodyContentApplicationJsonSchema>`: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[EncryptedBuffer <Byte- `[]`>]`: 
  - `[PublishingLicense <Byte- `[]`>]`:

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/invoke-mgbetabufferinformationprotectiondecrypt](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.identity.signins/invoke-mgbetabufferinformationprotectiondecrypt)
























