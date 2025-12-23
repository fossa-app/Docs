---
tags:
  - Entity
---

# Address

Represents a physical address.

## Properties

| Property | Type | Description |
| --- | --- | --- |
| `Line1` | `string` | The first line of the address. |
| `Line2` | `Option<string>` | The second line of the address (optional). |
| `City` | `string` | The city name. |
| `Subdivision` | `string` | The state, province, or region. |
| `PostalCode` | `string` | The postal or zip code. **Validation:** Must be valid for the specified `Country`. |
| `Country` | `RegionInfo` | The country information. **Validation:** Required. |

## Validation Rules

- All fields refer to `NotEmpty` rule, ensuring they are provided.
- `PostalCode` is validated using a country-specific postal code parser.

