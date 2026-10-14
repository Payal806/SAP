# Golden Repository Review Checklist

## Business completeness
- [ ] SAP edition, release, and modules are defined
- [ ] Scope items and organizational units are identified
- [ ] Country localization and compliance requirements are identified
- [ ] Business roles and responsibilities are defined
- [ ] End-to-end process (e.g. O2C, P2P) is covered
- [ ] In-scope and out-of-scope items are explicit

## Functional completeness
- [ ] Main, alternate, exception, cancellation, and reversal flows exist
- [ ] Document status, blocks, and document flow are documented
- [ ] Master data and configuration prerequisites are listed
- [ ] Rules are atomic and versioned
- [ ] Output (forms, email, EDI) and notifications are covered
- [ ] Integration failure handling is defined

## Technical completeness
- [ ] OData APIs, IDocs, and events are identified
- [ ] Extensions follow clean-core principles
- [ ] Data ownership, retention, and archiving are defined
- [ ] Authorization (roles, restrictions, SoD) matrix is included
- [ ] Audit and monitoring requirements exist
- [ ] Performance and upgrade-regression targets are stated

## AI-generated artifact quality
- [ ] Output is grounded in the selected source scope
- [ ] No unrelated epics, invented SAP apps, or invented requirements are introduced
- [ ] Every story has testable acceptance criteria
- [ ] UI test steps use Launchpad navigation (menu/tile) and stable locators
- [ ] Traceability is preserved from BRD to tests
- [ ] Assumptions and open questions are separated from confirmed facts
