Lookup Available Assets

## Objective

Enhance the onboarding workflow by searching for an available laptop before allocating an asset.

---

## Business Requirement

Before allocating a laptop to a new employee, the system should verify whether an available laptop exists in inventory.

---

## Flow Enhancement

Added a **Look Up Records** action.

### Configuration

- Table: ENX Asset
- Asset Type = Laptop
- Status = Available
- Maximum Records = 1

---

## Business Value

This approach prevents allocating unavailable assets and prepares the workflow for automatic procurement when inventory is exhausted.

---

## Concepts Learned

- Look Up Records
- Inventory Search
- Enterprise Asset Lifecycle
- Flow Data Pills

---

## Outcome

Configured the workflow to search for available inventory before performing asset allocation.
