# Reference Architecture

## Suggested logical components
- SAP Fiori Launchpad (web, mobile via SAP Mobile Start)
- SAP S/4HANA core (SD, MM, FI/CO, PP, EWM)
- SAP HANA database (Universal Journal, CDS views)
- Identity and access management (SAP Cloud Identity Services / corporate IdP)
- SAP Business Technology Platform (BTP) for side-by-side extensions
- SAP Integration Suite (Cloud Integration, API Management)
- Output management (Adobe Forms, email, EDI)
- External systems: CRM, e-commerce, tax engine, banks, logistics carriers
- Reporting and analytics (embedded analytics, SAP Analytics Cloud)
- Monitoring and observability (SAP Cloud ALM)

## Integration patterns
- OData V2 / V4 APIs from SAP Business Accelerator Hub (e.g. API_SALES_ORDER_SRV)
- SOAP services for legacy and B2B exchanges
- Business events (SAP Event Mesh) for document lifecycle changes
- IDoc / EDI for partner communication (ORDERS, INVOIC, DESADV)
- Batch / file interfaces for migration (SAP Migration Cockpit)
- Idempotency via external reference (e.g. customer PO number) to avoid duplicates
- Correlation IDs, retry, timeout, and error monitoring (Message Monitoring)

## Extension principles (clean core)
- No modification of SAP standard code
- Key-user extensibility (custom fields, custom logic) in tenant
- Developer extensibility using released APIs only
- Side-by-side apps on SAP BTP

## Security baseline
- Business roles built from SAP business catalogs; least privilege
- Restrictions by sales area, company code, plant
- Segregation of duties (e.g. create PO vs. approve PO vs. post invoice)
- MFA / SSO for all users
- Communication users and arrangements for integrations; no shared credentials
- Personal data blocking, masking, and read access logging
- Change documents and security audit log
