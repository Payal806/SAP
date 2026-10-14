# SAP S/4HANA Project Golden Repository

A reusable reference repository for generating high-quality SAP S/4HANA BRDs, epics, features, user stories, acceptance criteria, Fiori UX prompts, API/OData specifications, data models, and test cases.

## Scope
Supports SAP S/4HANA Cloud (public and private edition) and on-premise implementations, with a focus on Fiori Launchpad based business processes. Covers Sales (SD), Procurement (MM), Finance (FI/CO), Inventory and Warehouse, and Production (PP). Adapt the configuration values (company code, sales organization, plant, etc.) and compliance rules to the target country, company, and SAP release.

## Core lifecycle
1. Business partner management (customer and supplier master data)
2. Material / product master and pricing configuration
3. Order to Cash (O2C): inquiry, quotation, sales order, delivery, billing, payment
4. Procure to Pay (P2P): purchase requisition, purchase order, goods receipt, supplier invoice, payment
5. Inventory management: stock overview, goods movements, physical inventory
6. Plan to Produce: MRP, production order, confirmation
7. Record to Report: journal entries, period-end close, financial statements
8. Credit management, returns, and credit/debit memos
9. Output management (order confirmation, invoice PDF, email)
10. Analytics, reporting, and audit

## Default sample landscape (SAP demo tenant, US)
- Company code: 1710
- Sales organization: 1710 / Distribution channel: 10 / Division: 00
- Plant: 1710 / Storage location: 171A
- Purchasing organization: 1710

Replace these with the values configured in the target tenant.

## Important
This is a generic accelerator, not a certified SAP implementation or legal/tax advice. Validate requirements against the SAP Best Practices scope items activated in the tenant, company configuration, internal controls (e.g. SOX), and local tax and e-invoicing rules.
