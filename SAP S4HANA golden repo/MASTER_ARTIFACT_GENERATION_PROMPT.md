# Master Prompt for Artifact Generation

You are generating SAP S/4HANA SDLC and test artifacts using this golden repository as the source of truth.

## Instructions
1. Read the business context, domain glossary, process catalog, quality rules, architecture, data model, test strategy, and compliance adaptation guide.
2. Identify the selected SAP edition, release, module, scope item, organizational units, business roles, and scope.
3. Generate only artifacts supported by the selected scope.
4. Preserve traceability across BRD -> Epic -> Feature -> User Story -> Acceptance Criteria -> Test Case.
5. Prefer SAP standard functionality; label any extension, custom field, or custom logic explicitly.
6. Mark assumptions, dependencies, configuration prerequisites, unresolved questions, and compliance items requiring validation.
7. Do not invent SAP apps, transactions, tables, or configuration values. Cite the source or mark the item as needing confirmation in the tenant.
8. Include happy path, alternate path, negative path, blocked document, insufficient stock, credit block, cancellation, reversal, and duplicate-submission scenarios where applicable.
9. Include authorization (business roles, restrictions, SoD), audit (change documents), privacy, accessibility, localization, and output requirements.
10. For UI test cases, navigate through Launchpad menus and tiles (e.g. Sales -> Create Sales Order) rather than search, and capture generated document numbers for later steps.
11. Provide a coverage summary with:
   - Functional coverage
   - Business-rule coverage
   - Master data and configuration coverage
   - Data coverage
   - Integration coverage
   - Security/authorization coverage
   - Exception coverage
   - Testability coverage

## Output quality gate
Reject or revise any artifact that is vague, non-testable, duplicates another item, references unrelated scope, uses unverified SAP objects, or lacks required dependencies and exception handling.
