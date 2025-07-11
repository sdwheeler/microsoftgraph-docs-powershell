---
external help file: Microsoft.Graph.Beta.Financials-help.xml
Module Name: Microsoft.Graph.Beta.Financials
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.financials/new-mgbetafinancialcompanyjournalline
schema: 2.0.0
---

# New-MgBetaFinancialCompanyJournalLine

## SYNOPSIS
Create new navigation property to journalLines for financials

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaFinancialCompanyJournalLine -CompanyId <String> [-ResponseHeadersVariable <String>]
 [-Account <IMicrosoftGraphAccount>] [-AccountId <String>] [-AccountNumber <String>]
 [-AdditionalProperties <Hashtable>] [-Amount <Decimal>] [-Comment <String>] [-Description <String>]
 [-DocumentNumber <String>] [-ExternalDocumentNumber <String>] [-Id <String>] [-JournalDisplayName <String>]
 [-LastModifiedDateTime <DateTime>] [-LineNumber <Int32>] [-PostingDate <DateTime>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateExpanded1
```
New-MgBetaFinancialCompanyJournalLine -CompanyId <String> -JournalId <String>
 [-ResponseHeadersVariable <String>] [-Account <IMicrosoftGraphAccount>] [-AccountId <String>]
 [-AccountNumber <String>] [-AdditionalProperties <Hashtable>] [-Amount <Decimal>] [-Comment <String>]
 [-Description <String>] [-DocumentNumber <String>] [-ExternalDocumentNumber <String>] [-Id <String>]
 [-JournalDisplayName <String>] [-LastModifiedDateTime <DateTime>] [-LineNumber <Int32>]
 [-PostingDate <DateTime>] [-Headers <IDictionary>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Create1
```
New-MgBetaFinancialCompanyJournalLine -CompanyId <String> -JournalId <String>
 -BodyParameter <IMicrosoftGraphJournalLine> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaFinancialCompanyJournalLine -CompanyId <String> -BodyParameter <IMicrosoftGraphJournalLine>
 [-ResponseHeadersVariable <String>] [-Headers <IDictionary>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded1
```
New-MgBetaFinancialCompanyJournalLine -InputObject <IFinancialsIdentity> [-ResponseHeadersVariable <String>]
 [-Account <IMicrosoftGraphAccount>] [-AccountId <String>] [-AccountNumber <String>]
 [-AdditionalProperties <Hashtable>] [-Amount <Decimal>] [-Comment <String>] [-Description <String>]
 [-DocumentNumber <String>] [-ExternalDocumentNumber <String>] [-Id <String>] [-JournalDisplayName <String>]
 [-LastModifiedDateTime <DateTime>] [-LineNumber <Int32>] [-PostingDate <DateTime>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgBetaFinancialCompanyJournalLine -InputObject <IFinancialsIdentity> [-ResponseHeadersVariable <String>]
 [-Account <IMicrosoftGraphAccount>] [-AccountId <String>] [-AccountNumber <String>]
 [-AdditionalProperties <Hashtable>] [-Amount <Decimal>] [-Comment <String>] [-Description <String>]
 [-DocumentNumber <String>] [-ExternalDocumentNumber <String>] [-Id <String>] [-JournalDisplayName <String>]
 [-LastModifiedDateTime <DateTime>] [-LineNumber <Int32>] [-PostingDate <DateTime>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity1
```
New-MgBetaFinancialCompanyJournalLine -InputObject <IFinancialsIdentity>
 -BodyParameter <IMicrosoftGraphJournalLine> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgBetaFinancialCompanyJournalLine -InputObject <IFinancialsIdentity>
 -BodyParameter <IMicrosoftGraphJournalLine> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to journalLines for financials

## EXAMPLES

## PARAMETERS

### -Account
account
To construct, see NOTES section for ACCOUNT properties and create a hash table.

```yaml
Type: IMicrosoftGraphAccount
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AccountId


```yaml
Type: String
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AccountNumber


```yaml
Type: String
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Amount


```yaml
Type: Decimal
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
journalLine
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphJournalLine
Parameter Sets: Create1, Create, CreateViaIdentity1, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Comment


```yaml
Type: String
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CompanyId
The unique identifier of company

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateExpanded1, Create1, Create
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

### -Description


```yaml
Type: String
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DocumentNumber


```yaml
Type: String
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExternalDocumentNumber


```yaml
Type: String
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
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


```yaml
Type: String
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
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
Type: IFinancialsIdentity
Parameter Sets: CreateViaIdentityExpanded1, CreateViaIdentityExpanded, CreateViaIdentity1, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -JournalDisplayName


```yaml
Type: String
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JournalId
The unique identifier of journal

```yaml
Type: String
Parameter Sets: CreateExpanded1, Create1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LastModifiedDateTime


```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LineNumber


```yaml
Type: Int32
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -PostingDate


```yaml
Type: DateTime
Parameter Sets: CreateExpanded, CreateExpanded1, CreateViaIdentityExpanded1, CreateViaIdentityExpanded
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

### Microsoft.Graph.Beta.PowerShell.Models.IFinancialsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphJournalLine
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphJournalLine
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

ACCOUNT `<IMicrosoftGraphAccount>`: account
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Blocked <Boolean?>]`: 
  - `[Category <String>]`: 
  - `[DisplayName <String>]`: 
  - `[Id <String>]`: 
  - `[LastModifiedDateTime <DateTime?>]`: 
  - `[Number <String>]`: 
  - `[SubCategory <String>]`: 

BODYPARAMETER `<IMicrosoftGraphJournalLine>`: journalLine
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Account <IMicrosoftGraphAccount>]`: account
    - `[(Any) <Object>]`: This indicates any property can be added to this object.
    - `[Blocked <Boolean?>]`: 
    - `[Category <String>]`: 
    - `[DisplayName <String>]`: 
    - `[Id <String>]`: 
    - `[LastModifiedDateTime <DateTime?>]`: 
    - `[Number <String>]`: 
    - `[SubCategory <String>]`: 
  - `[AccountId <String>]`: 
  - `[AccountNumber <String>]`: 
  - `[Amount <Decimal?>]`: 
  - `[Comment <String>]`: 
  - `[Description <String>]`: 
  - `[DocumentNumber <String>]`: 
  - `[ExternalDocumentNumber <String>]`: 
  - `[Id <String>]`: 
  - `[JournalDisplayName <String>]`: 
  - `[LastModifiedDateTime <DateTime?>]`: 
  - `[LineNumber <Int32?>]`: 
  - `[PostingDate <DateTime?>]`: 

INPUTOBJECT `<IFinancialsIdentity>`: Identity Parameter
  - `[AccountId <String>]`: The unique identifier of account
  - `[AgedAccountsPayableId <String>]`: The unique identifier of agedAccountsPayable
  - `[AgedAccountsReceivableId <String>]`: The unique identifier of agedAccountsReceivable
  - `[CompanyId <String>]`: The unique identifier of company
  - `[CompanyInformationId <String>]`: The unique identifier of companyInformation
  - `[CountryRegionId <String>]`: The unique identifier of countryRegion
  - `[CurrencyId <String>]`: The unique identifier of currency
  - `[CustomerId <String>]`: The unique identifier of customer
  - `[CustomerPaymentId <String>]`: The unique identifier of customerPayment
  - `[CustomerPaymentJournalId <String>]`: The unique identifier of customerPaymentJournal
  - `[DimensionId <String>]`: The unique identifier of dimension
  - `[DimensionValueId <String>]`: The unique identifier of dimensionValue
  - `[EmployeeId <String>]`: The unique identifier of employee
  - `[GeneralLedgerEntryId <String>]`: The unique identifier of generalLedgerEntry
  - `[ItemCategoryId <String>]`: The unique identifier of itemCategory
  - `[ItemId <String>]`: The unique identifier of item
  - `[JournalId <String>]`: The unique identifier of journal
  - `[JournalLineId <String>]`: The unique identifier of journalLine
  - `[PaymentMethodId <String>]`: The unique identifier of paymentMethod
  - `[PaymentTermId <String>]`: The unique identifier of paymentTerm
  - `[PictureId <String>]`: The unique identifier of picture
  - `[PurchaseInvoiceId <String>]`: The unique identifier of purchaseInvoice
  - `[PurchaseInvoiceLineId <String>]`: The unique identifier of purchaseInvoiceLine
  - `[SalesCreditMemoId <String>]`: The unique identifier of salesCreditMemo
  - `[SalesCreditMemoLineId <String>]`: The unique identifier of salesCreditMemoLine
  - `[SalesInvoiceId <String>]`: The unique identifier of salesInvoice
  - `[SalesInvoiceLineId <String>]`: The unique identifier of salesInvoiceLine
  - `[SalesOrderId <String>]`: The unique identifier of salesOrder
  - `[SalesOrderLineId <String>]`: The unique identifier of salesOrderLine
  - `[SalesQuoteId <String>]`: The unique identifier of salesQuote
  - `[SalesQuoteLineId <String>]`: The unique identifier of salesQuoteLine
  - `[ShipmentMethodId <String>]`: The unique identifier of shipmentMethod
  - `[TaxAreaId <String>]`: The unique identifier of taxArea
  - `[TaxGroupId <String>]`: The unique identifier of taxGroup
  - `[UnitOfMeasureId <String>]`: The unique identifier of unitOfMeasure
  - `[VendorId <String>]`: The unique identifier of vendor

## RELATED LINKS

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.financials/new-mgbetafinancialcompanyjournalline](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.financials/new-mgbetafinancialcompanyjournalline)
























