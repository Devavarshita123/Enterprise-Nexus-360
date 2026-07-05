# Activity 4: Asset Management Module

## Objective

Design and implement the **ENX Asset** module for the Enterprise Nexus 360 application. This module serves as the central repository for managing enterprise assets throughout their lifecycle, including allocation, maintenance, warranty tracking, and retirement.

---

# Background

Every organization manages a wide range of physical assets such as laptops, desktops, monitors, mobile phones, printers, ID cards, and other office equipment.

The objective of this module is to provide a centralized system for storing asset information and linking assets to employees and departments.

This module will serve as the foundation for future implementations such as:

* Employee Onboarding
* Employee Offboarding
* Asset Allocation
* Asset Return
* Incident Management
* Procurement
* CMDB Integration
* AI-based Asset Recommendations

---

# Table Created

**Table Name:** ENX Asset

**Application:** Enterprise Nexus 360

**Purpose:**

Stores enterprise asset information and maintains relationships with employees and departments.

---

# Fields Added

| Field             | Type                             | Purpose                            |
| ----------------- | -------------------------------- | ---------------------------------- |
| Asset Number      | String                           | Unique identifier for every asset  |
| Asset Name        | String                           | Name of the asset                  |
| Asset Type        | Choice                           | Categorizes the asset              |
| Serial Number     | String                           | Manufacturer serial number         |
| Assigned Employee | Reference (ENX Employee Profile) | Employee currently using the asset |
| Department        | Reference (ENX Department)       | Department owning the asset        |
| Status            | Choice                           | Current lifecycle status           |
| Purchase Date     | Date                             | Asset purchase date                |
| Warranty Expiry   | Date                             | Warranty expiration date           |
| Purchase Cost     | Decimal                          | Purchase cost of the asset         |
| Remarks           | Multi-line Text                  | Additional notes                   |

---

# Asset Types

The following asset categories were configured.

* Laptop
* Desktop
* Monitor
* Mobile
* Printer
* Keyboard
* Mouse
* Headset
* ID Card
* Other

---

# Asset Status Values

The asset lifecycle includes the following statuses.

* Available
* Allocated
* In Repair
* Retired
* Lost
* Disposed

---

# Relationships

The Asset module establishes relationships with other modules.

```
ENX Asset
│
├── Assigned Employee
│      └── ENX Employee Profile
│
└── Department
       └── ENX Department
```

These relationships enable tracking of asset ownership and departmental allocation.

---

# Design Decisions

Instead of using simple text fields for employee and department information, reference fields were used to maintain data consistency and eliminate duplication.

The module has been designed with future scalability in mind so that it can later integrate with:

* Procurement
* CMDB
* Service Catalog
* Incident Management
* Change Management
* AI Services

without requiring structural modifications.

---

This module acts as one of the core pillars of the Enterprise Nexus 360 platform and will be extended throughout subsequent development phases.
