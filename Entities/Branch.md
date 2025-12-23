---
tags:
  - Entity
---

# Branch

Represents a branch office or location within a company.

## Properties

| Property | Type | Description |
| --- | --- | --- |
| `ID` | `BranchId` | Unique identifier for the branch. |
| `TenantID` | `Guid` | The ID of the tenant. |
| `CompanyId` | `CompanyId` | The ID of the company this branch belongs to. |
| `Name` | `string` | The name of the branch. |
| `TimeZone` | `DateTimeZone` | The time zone of the branch. **Validation:** Must match Company country. |
| `Address` | `Option<Address>` | Physical address of the branch. **Validation:** Country must match Company country. |
