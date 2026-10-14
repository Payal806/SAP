# Data Model Reference

## Core entities (with key SAP tables / CDS views)
- Business Partner (BUT000, I_BusinessPartner)
- Customer (KNA1, KNVV) / Supplier (LFA1)
- Product / Material (MARA, MARC, MARD, I_Product)
- Pricing condition (PRCD_ELEMENTS, condition records)
- Organizational units: company code, sales organization, plant, storage location
- Sales inquiry / quotation / sales order header and items (VBAK, VBAP, I_SalesOrder)
- Schedule line (VBEP)
- Outbound delivery (LIKP, LIPS)
- Billing document (VBRK, VBRP, I_BillingDocument)
- Document flow (VBFA)
- Purchase requisition (EBAN)
- Purchase order (EKKO, EKPO, I_PurchaseOrder)
- Material document / goods movement (MATDOC)
- Supplier invoice (RBKP, RSEG)
- Journal entry (ACDOCA, BKPF)
- Credit limit / credit exposure (UKMBP_CMS_SGM)
- Production order (AFKO, AFPO)
- Output request
- Change document (CDHDR, CDPOS)

## Data rules
- Document numbers are system-generated from number ranges and are immutable.
- Master data must exist and be valid for the organizational unit before transactional documents are created.
- Store currency and unit of measure explicitly on every amount and quantity.
- Respect configured decimal places and rounding per currency.
- Pricing uses condition records valid on the pricing date.
- Record source system for migrated and integrated data.
- Define required, optional, conditional, and prohibited fields per document type.
- Apply data retention, archiving, blocking, and deletion rules (ILM) by data category.
