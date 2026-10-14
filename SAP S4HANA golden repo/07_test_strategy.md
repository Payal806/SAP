# Test Strategy

## Test layers
- Unit tests (custom logic, extensions)
- OData / API and contract tests
- Integration tests (S/4HANA <-> external systems, IDoc, events)
- End-to-end business process tests (O2C, P2P, R2R)
- Fiori UI tests (Launchpad navigation, apps, tiles)
- Role and authorization tests
- Security and SoD tests
- Performance tests (Fiori apps, OData, mass processing)
- Data migration and reconciliation tests
- Upgrade regression tests (quarterly / release upgrades)
- Output and form tests (PDF, email, EDI)

## UI automation guidelines (Fiori)
- Navigate via Launchpad spaces/pages and tiles (e.g. Sales -> Create Sales Order), not via search, unless search is the flow under test.
- Do not rely on generated control IDs (e.g. `__xmlview0--...`, `__button12`); use labels, stable IDs, or UI5 control properties.
- Wait for the UI5 busy indicator to disappear before the next action.
- Capture the document number from the success message toast and reuse it in later steps.
- Parameterize organizational data, customer, material, and quantities.

## SAP-specific scenarios
- Create sales order with valid master data
- Sales order with missing or invalid sold-to party / material
- Pricing determination, discounts, and tax calculation
- Quantity exceeding available stock (ATP)
- Customer exceeding credit limit (credit block)
- Duplicate customer PO reference
- Delivery date in the past
- Change or cancel a sales order after delivery is created
- Delivery and goods issue with insufficient stock
- Billing and posting to accounting (document flow check)
- Returns and credit memo
- PO -> GR -> invoice 3-way match with price/quantity variance
- Posting in a closed period
- User without required business role or outside sales area restriction
- Segregation of duties violations
- Change documents recorded for master data changes
