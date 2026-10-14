# Requirements Quality Rules

Every requirement must be:

- Atomic: one primary behavior or obligation.
- Testable: measurable acceptance criteria exist.
- Unambiguous: avoid vague terms such as fast, user-friendly, or appropriate.
- Traceable: linked to business objective, process, SAP scope item, business rule, data, API, and test.
- Role-specific: SAP business role and restrictions (sales area, company code, plant) are explicit.
- State-aware: document status, blocks, and status transitions are defined.
- Organization-aware: company code, sales area, plant, and document type are identified.
- Standard-first: prefer SAP standard configuration; extensions are marked as such.
- Secure and privacy-aware: sensitive data (bank, personal data, pricing) handling is explicit.
- Auditable: change documents, user, timestamp, and before/after values are defined when relevant.

## Mandatory requirement fields
- Requirement ID
- Title
- Business rationale
- SAP module / scope item
- Fiori app (name / app ID) or transaction
- Actor (business role)
- Trigger
- Preconditions (master data and configuration)
- Main flow
- Alternate and exception flows
- Business rules
- Data inputs and outputs (fields, tables, CDS views)
- Permissions
- Audit requirements
- Output / notifications
- Acceptance criteria
- Dependencies (preceding / subsequent documents)
- Traceability links
