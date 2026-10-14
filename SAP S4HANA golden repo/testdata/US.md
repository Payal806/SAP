---
name: United States
description: Sample SAP S/4HANA test data for US company code 1710 (SAP demo tenant defaults; confirm in target tenant)
isActive: true
---

## Organizational data
| Field | Value |
|---|---|
| Company code | 1710 |
| Sales organization | 1710 |
| Distribution channel | 10 |
| Division | 00 |
| Plant | 1710 |
| Storage location | 171A |
| Purchasing organization | 1710 |
| Currency | USD |

## Sales order (Sales -> Create Sales Order)
| Field | Value |
|---|---|
| Order type | OR (Standard Order) |
| Sold-to party | 17100001 |
| Customer reference | PO-AUTO-001 |
| Requested delivery date | Today + 7 days |
| Material | TG11 |
| Quantity | 10 |

## Negative test data
| Scenario | Value |
|---|---|
| Invalid customer | 99999999 |
| Invalid material | INVALID-MAT |
| Zero quantity | 0 |
| Past delivery date | Today - 5 days |
