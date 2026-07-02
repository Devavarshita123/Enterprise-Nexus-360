Intelligent Asset Allocation

## Objective
Enhanced the onboarding workflow to allocate an actual available laptop instead of creating a generic allocation record.

## Changes Made
- Added an IF condition to verify whether an available laptop exists.
- Used the Look Up Record output to identify the specific laptop.
- Created an Asset Allocation record using the retrieved asset.
- Updated the asset status from Available to Allocated.

## Concepts Learned
- Look Up Record
- Data Pills
- Conditional Flow Logic
- Update Record Action
- Inventory Synchronization

## Outcome
The onboarding workflow now allocates real inventory and keeps asset status synchronized, matching enterprise ServiceNow implementation practices.
