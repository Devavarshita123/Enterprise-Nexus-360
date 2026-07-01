Automating Service Request Creation

## Objective

Extend the Employee Onboarding Flow to automatically generate a Service Request whenever an onboarding request is approved.

---

## Business Requirement

When HR approves a new employee onboarding request, IT teams should not manually create service requests for provisioning. The workflow should automate this process to improve efficiency and reduce manual effort.

---

## Flow Enhancement

Added a **Create Record** action to the **ENX Employee Onboarding Flow**.

### Trigger

- Record Updated
- Table: ENX Onboarding Request
- Condition: Status changes to Approved

### Action

Create a new record in **ENX Service Request**.

---

## Field Mapping

| Service Request Field | Source |
|------------------------|--------|
| Requested By | Employee from Onboarding Request |
| Department | Department from Onboarding Request |
| Request Type | Asset Request |
| Category | Hardware |
| Short Description | Employee Onboarding Asset Provisioning |
| Description | Auto-generated from onboarding workflow |
| Priority | High |
| Status | New |
| Approval Status | Pending |

---

## Concepts Learned

- Flow Designer Actions
- Create Record Action
- Cross-table Automation
- Dynamic Field Mapping
- Enterprise Workflow Automation

---

## Outcome

Successfully automated the creation of Service Requests from approved onboarding requests, eliminating manual intervention and improving onboarding efficiency.

---
