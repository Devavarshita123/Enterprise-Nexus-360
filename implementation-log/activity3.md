# Activity 3: Employee Profile Module

## Objective

Design and implement the **ENX Employee Profile** module to maintain enterprise-specific employee information while following ServiceNow best practices. Instead of modifying the native **User [sys_user]** table, a separate Employee Profile table was created and linked to the User table using a reference field.

---

## Why This Design?

The ServiceNow platform already provides the **User [sys_user]** table to manage all users. To avoid unnecessary customization of core platform tables and to keep the application maintainable and upgrade-friendly, a separate **ENX Employee Profile** table was created.

This design follows enterprise best practices by:
- Keeping custom application data separate from platform data.
- Establishing relationships using reference fields.
- Making the application modular and scalable.

---

## Table Created

**Table Name:** ENX Employee Profile

**Application:** Enterprise Nexus 360

**Purpose:** Stores enterprise-specific employee details required for HR, onboarding, asset management, approvals, and workflow automation.

---

## Fields Added

| Field | Type | Purpose |
|--------|------|---------|
| User | Reference (sys_user) | Links employee profile to a ServiceNow user |
| Employee ID | String | Unique employee identifier |
| Department | Reference (ENX Department) | Associates employee with a department |
| Manager | Reference (sys_user) | Reporting manager |
| Employee Type | Choice | Full Time, Intern, Contractor, Consultant |
| Joining Date | Date | Employee joining date |
| Employment Status | Choice | Active, On Leave, Resigned, Terminated |
| Work Location | String | Employee work location |
| Cost Center | String | Cost center allocation |
| Remarks | Multi-line Text | Additional employee notes |

---

## Sample Records Created

Three sample employee profiles were created for testing future modules.

### Record 1

- Employee ID: EMP0001
- Department: Information Technology
- Employee Type: Full Time
- Employment Status: Active
- Work Location: Hyderabad

### Record 2

- Employee ID: EMP0002
- Department: Human Resources
- Employee Type: Full Time
- Employment Status: Active
- Work Location: Bangalore

### Record 3

- Employee ID: EMP0003
- Department: Information Technology
- Employee Type: Intern
- Employment Status: Active
- Work Location: Remote

---

## Concepts Learned

- Creating custom tables
- Reference fields
- Choice fields
- Form configuration
- Relational data modeling
- Display fields
- Application scoping
- Enterprise data modeling

---
