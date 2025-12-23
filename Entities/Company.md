---
tags:
  - Entity
---

# Company

Represents a legal entity or organization tenant in the system.

## Properties

| Property | Type | Description |
| --- | --- | --- |
| `ID` | `CompanyId` | Unique identifier for the company. |
| `TenantID` | `Guid` | The ID of the tenant. |
| `Name` | `string` | The registered name of the company. |
| `Country` | `RegionInfo` | The country of incorporation or operation. **Validation:** Must be a licensed country. |
