---
tags:
  - Flow
---
[[Employees]] flow enables listing and management of [[Employee]] entities.

## Employee Management
### Management of Employee Reports To
#### Management of Employee Reports To API
Employee Managements endpoint includes `ReportsToId` which is `EmployeeId` of employee's direct manager. 
An employee record may not be deleted if there is another employee whose `ReportsToId` references the ID of the employee marked for removal.
During the modification of employee's `ReportsToId` makes sure an employee with the given Id exists.
Cyclical references are not allowed.
The employee listing endpoints support filtering either by `ReportsToId` or by the `TopLevelOnly` Boolean flag, which returns only employees without a `ReportsToId` (i.e., where `ReportsToId` is `NULL`).
### Management of Employee Job Title
#### Management of Employee Job Title API
Employee Managements endpoint includes `JobTitle` which is nullable, not empty string and can be edited only by administrators.
Job Title can't be set as `NULL`, empty string or white spaces.