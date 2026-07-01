Employee Onboarding Flow – Part 1 (Flow Trigger)

## Objective

Begin automating the employee onboarding process by creating the initial Flow Designer workflow. This flow will serve as the foundation for automating HR and IT provisioning tasks whenever a new employee onboarding request is approved.

---

## Business Requirement

In a traditional onboarding process, HR manually coordinates with multiple departments to provision resources such as laptops, email accounts, VPN access, ID cards, and software. This manual approach is time-consuming and prone to delays.

To improve efficiency, the onboarding process should automatically begin once an onboarding request is approved.

---

## Flow Created

**Flow Name:** ENX Employee Onboarding Flow

**Application:** Enterprise Nexus 360

---

## Trigger Configuration

| Property | Value |
|----------|-------|
| Trigger Type | Record |
| Table | ENX Onboarding Request |
| Event | Updated |
| Condition | Status changes to **Approved** |

---

## Current Flow Design

```
ENX Onboarding Request
        │
        ▼
Record Updated
        │
        ▼
Status = Approved
        │
        ▼
Flow Triggered
```

---

## Planned Automation (Upcoming Activities)

The flow currently contains only the trigger. The following actions will be added in the next implementation phases:

- Create Service Request automatically
- Allocate enterprise assets
- Send notification to HR
- Send notification to employee
- Update onboarding status
- Generate audit logs
- Create approval records
- Provision IT resources

---

## Concepts Learned

- Introduction to Flow Designer
- Record-based Flow Triggers
- Trigger Conditions
- Workflow Automation
- Enterprise Process Automation

---

## Business Value

Automating employee onboarding reduces manual effort, improves provisioning speed, minimizes human error, and ensures a standardized onboarding experience across the organization.
