---
tags:
  - Entity
---

# Company Settings

Represents configuration settings for a company.

## Properties

| Property | Type | Description |
| --- | --- | --- |
| `ID` | `CompanySettingsId` | Unique identifier for the settings. |
| `CompanyId` | `CompanyId` | The ID of the company these settings belong to. **Validation:** Required (`TenantID`). |
| `ColorSchemeId` | `ColorSchemeId` | The ID of the preferred color scheme. **Validation:** Required. |

## Validation Rules

- `TenantID` (CompanyId), `UserID`, and `ColorSchemeId` are strictly required (NotEmpty).

