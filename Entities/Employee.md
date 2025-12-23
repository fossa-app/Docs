---
tags:
  - Entity
---

# Employee

Represents an individual working for the company.

## Properties

| Property | Type | Description |
| --- | --- | --- |
| `ID` | `EmployeeId` | Unique identifier for the employee. |
| `TenantID` | `Guid` | The ID of the tenant. |
| `UserID` | `Guid` | The ID of the associated user account. |
| `CompanyId` | `CompanyId` | The ID of the company. |
| `AssignedBranchId` | `Option<BranchId>` | The branch the employee is assigned to. |
| `AssignedDepartmentId` | `Option<DepartmentId>` | The department the employee is assigned to. |
| `ReportsToId` | `Option<EmployeeId>` | The direct supervisor of the employee. |
| `JobTitle` | `string` | The job title or position. |
| `FirstName` | `string` | First name. |
| `LastName` | `string` | Last name. |
| `FullName` | `string` | Full name (computed or stored). |
