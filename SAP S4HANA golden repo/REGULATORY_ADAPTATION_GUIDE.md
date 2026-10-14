# Compliance and Localization Adaptation Guide

Do not treat this repository as a complete legal, tax, or regulatory baseline.

Before implementation, identify:
- Country, state/province, and company codes in scope
- SAP country localization (country version) activated in the tenant
- Tax determination (sales tax, VAT, GST) and external tax engine, if any
- E-invoicing and statutory reporting obligations
- Financial reporting standards (local GAAP, IFRS, US GAAP)
- Internal controls framework (e.g. SOX) and segregation-of-duties rules
- Data protection and cross-border transfer requirements (e.g. GDPR, India DPDP Act)
- Export control, sanctions, and trade compliance screening
- Record retention, archiving, and audit requirements
- Electronic signature and document validity
- Accessibility and language obligations

For India-specific implementations, confirm current GST rules, e-invoicing (IRN) and e-way bill requirements, and the SAP India localization in the tenant. For US implementations, confirm sales and use tax handling and SOX controls. Applicability depends on the actual solution scope.
