---
external help file: Microsoft.Graph.Beta.Financials-help.xml
Module Name: Microsoft.Graph.Beta.Financials
online version: https://learn.microsoft.com/powershell/module/microsoft.graph.beta.financials/new-mgbetafinancialcompanycustomerpaymentcustomerpicture
schema: 2.0.0
---

# New-MgBetaFinancialCompanyCustomerPaymentCustomerPicture

## SYNOPSIS
Create new navigation property to picture for financials

## SYNTAX

### CreateExpanded (Default)
```
New-MgBetaFinancialCompanyCustomerPaymentCustomerPicture -CompanyId <String> -CustomerPaymentId <String>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-ContentInputFile <String>]
 [-ContentType <String>] [-Height <Int32>] [-Id <String>] [-Width <Int32>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Create
```
New-MgBetaFinancialCompanyCustomerPaymentCustomerPicture -CompanyId <String> -CustomerPaymentId <String>
 -BodyParameter <IMicrosoftGraphPicture> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentityExpanded
```
New-MgBetaFinancialCompanyCustomerPaymentCustomerPicture -InputObject <IFinancialsIdentity>
 [-ResponseHeadersVariable <String>] [-AdditionalProperties <Hashtable>] [-ContentInputFile <String>]
 [-ContentType <String>] [-Height <Int32>] [-Id <String>] [-Width <Int32>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### CreateViaIdentity
```
New-MgBetaFinancialCompanyCustomerPaymentCustomerPicture -InputObject <IFinancialsIdentity>
 -BodyParameter <IMicrosoftGraphPicture> [-ResponseHeadersVariable <String>] [-Headers <IDictionary>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Create new navigation property to picture for financials

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: Hashtable
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
picture
To construct, see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: IMicrosoftGraphPicture
Parameter Sets: Create, CreateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CompanyId
The unique identifier of company

```yaml
Type: String
Parameter Sets: CreateExpanded, Create
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

### -ContentInputFile
Input File for Content (.)

```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ContentType


```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CustomerPaymentId
The unique identifier of customerPayment

```yaml
Type: String
Parameter Sets: CreateExpanded, Create
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

### -Height


```yaml
Type: Int32
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id


```yaml
Type: String
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
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
Parameter Sets: CreateViaIdentityExpanded, CreateViaIdentity
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

### -Width


```yaml
Type: Int32
Parameter Sets: CreateExpanded, CreateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IFinancialsIdentity
### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphPicture
### System.Collections.IDictionary
## OUTPUTS

### Microsoft.Graph.Beta.PowerShell.Models.IMicrosoftGraphPicture
## NOTES
COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties.
For information on hash tables, run Get-Help about_Hash_Tables.

BODYPARAMETER `<IMicrosoftGraphPicture>`: picture
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Content <Byte- `[]`>]`: 
  - `[ContentType <String>]`: 
  - `[Height <Int32?>]`: 
  - `[Id <String>]`: 
  - `[Width <Int32?>]`: 

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

[https://learn.microsoft.com/powershell/module/microsoft.graph.beta.financials/new-mgbetafinancialcompanycustomerpaymentcustomerpicture](https://learn.microsoft.com/powershell/module/microsoft.graph.beta.financials/new-mgbetafinancialcompanycustomerpaymentcustomerpicture)
























