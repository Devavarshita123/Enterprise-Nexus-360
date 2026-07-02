Automatic Procurement Fallback

## Objective
Implemented automatic procurement when the required asset is unavailable.

## Workflow
1. Check whether a laptop is required.
2. Search inventory for an available laptop.
3. If found:
   - Allocate the laptop.
   - Update its status.
4. If not found:
   - Create a Procurement Request automatically.

## Concepts Learned
- Conditional branching
- Enterprise inventory validation
- Automated procurement
- End-to-end business automation

## Outcome
The onboarding workflow now handles both inventory allocation and procurement automatically, reducing manual intervention.
