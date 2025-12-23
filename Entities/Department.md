---
tags:
  - Entity
---

# Department

Represents a functional unit or division within a company.

## Properties

| Property | Type | Description |
| --- | --- | --- |
| `ID` | `DepartmentId` | Unique identifier for the department. |
| `TenantID` | `Guid` | The ID of the tenant. |
| `CompanyId` | `CompanyId` | The ID of the company this department belongs to. |
| `Name` | `string` | The name of the department. |
| `ManagerId` | `EmployeeId` | The ID of the department manager. **Validation:** Must be an employee in the same tenant. |
| `ParentDepartmentId` | `Option<DepartmentId>` | The ID of the parent department (if any). **Validation:** Must be in the same tenant. |
