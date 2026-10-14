# Business Rules Catalog

Rules should be uniquely identified, versioned, effective-dated, and linked to SAP modules, organizational units, and document types.

Examples:
- BR-001: A sales order cannot be saved without a valid sold-to party assigned to the sales area.
- BR-002: A sales order item requires a valid material that is extended to the sales area and delivering plant.
- BR-003: Prices must be determined from condition records valid on the pricing date.
- BR-004: Order quantity must be greater than zero and in an allowed unit of measure.
- BR-005: If requested quantity exceeds available stock, the ATP check must propose a confirmed date/quantity.
- BR-006: A customer exceeding the credit limit results in a credit block; delivery cannot be created until released.
- BR-007: A duplicate customer PO reference for the same sold-to party triggers a warning.
- BR-008: A sales order cannot be changed in quantity below the already delivered quantity.
- BR-009: Billing is allowed only after goods issue for delivery-related billing.
- BR-010: Supplier invoices must match PO and goods receipt within configured tolerances (3-way match).
- BR-011: Postings are allowed only in open posting periods.
- BR-012: A user may create or change documents only within their assigned business role restrictions.
- BR-013: Changes to master data (business partner, bank details, credit limit) must be recorded in change documents.
- BR-014: The same user must not create and approve the same purchase order (segregation of duties).
