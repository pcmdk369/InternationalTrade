# Software Training — Excel for Trade Operations

**Level:** Intermediate  
**Goal:** Build reliable operational registers before automating them.

## 1. Workbook design

Create one workbook with these sheets:

1. `Orders`
2. `Shipments`
3. `Suppliers`
4. `Documents`
5. `Costs`
6. `Dashboard`

Use unique IDs to link records. Do not use company names as unique keys because names can change or repeat.

## 2. Orders sheet

Recommended columns:

`Order_ID, Inquiry_ID, Buyer, Seller, Product, Quantity, Unit, Currency, Unit_Price, Order_Value, Order_Date, Required_Date, Status, Owner`

Example formula for order value in a structured Excel table:

`=[@Quantity]*[@Unit_Price]`

## 3. Shipments sheet

Recommended columns:

`Shipment_ID, Order_ID, Origin, Destination, Mode, Incoterm, Named_Place, ETD, ETA, Actual_Delivery, Milestone, Status, Issue_Owner, Next_Action`

Calculate delay days only when planned and actual dates exist. A blank actual delivery date means the shipment is not yet delivered; it must not be treated as zero delay.

Example:

`=IF([@Actual_Delivery]="","",MAX(0,[@Actual_Delivery]-[@ETA]))`

## 4. Data validation

- Use dropdown lists for status, mode and currency.
- Require unique Order_ID and Shipment_ID values.
- Store dates as actual date values, not mixed text.
- Store numeric quantities and prices as numbers.
- Keep currency codes in a separate field.
- Do not mix multiple currencies in one total without conversion and an explicit rate/date.

## 5. Useful formulas

Order value:

`=Quantity*Unit_Price`

Outstanding amount:

`=Invoice_Amount-Payment_Confirmed`

On-time flag:

`=IF(Actual_Delivery="","Pending",IF(Actual_Delivery<=ETA,"On time","Late"))`

Do not use these formulas blindly; verify column names, date meaning and business definitions.

## 6. Dashboard metrics

- Active orders
- Orders awaiting approval
- Shipments in transit
- Delayed shipments
- Documents awaiting review
- Customs holds
- On-time delivery rate
- Open issues by priority

Define each KPI before calculating it. For example, specify whether the on-time rate uses delivered shipments only or all shipments.

## 7. Practical assignment

Build a workbook with at least:
- 10 fictional orders
- 10 shipment records
- 5 suppliers
- 20 document checklist rows
- 10 cost lines

Create a dashboard with four KPIs and a chart. Use fictional data only.

## 8. Quality checks

- Reconcile totals to source records.
- Check duplicate IDs.
- Check missing dates and owners.
- Identify impossible date sequences.
- Protect formulas from accidental edits.
- Keep a dated backup and version history.
