Conditional Asset Allocation

## Objective

Enhance the Employee Onboarding Flow by introducing conditional logic to allocate enterprise assets only when requested.

---

## Business Requirement

Not every employee requires the same IT resources. The onboarding workflow should dynamically determine which resources need provisioning based on the onboarding request.

---

## Flow Enhancement

Added an **IF** condition to evaluate whether a laptop is required.

### Condition

Laptop Required = True

### Action

Create a new Asset Allocation record.

---

## Asset Allocation Details

| Field | Value |
|--------|-------|
| Employee | Employee from onboarding request |
| Status | Allocated |
| Allocation Date | Current Date |
| Remarks | Laptop allocated during onboarding |

---

## Concepts Learned

- Flow Logic
- IF Conditions
- Conditional Automation
- Dynamic Workflow Execution
