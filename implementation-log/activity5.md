Vendor Management Module

## Objective

Develop the **Vendor Management** module to maintain information about all vendors supplying hardware, software, cloud services, and office equipment to the organization.

---

## Business Requirement

Every enterprise procures assets and services from multiple vendors. Maintaining vendor information in a centralized repository improves procurement efficiency, warranty management, contract tracking, and vendor performance analysis.

This module serves as the master data source for all procurement-related activities within the Enterprise Nexus 360 application.

---

## Table Created

**Table Name:** ENX Vendor

**Application:** Enterprise Nexus 360

---

## Fields Added

| Field | Type | Description |
|--------|------|-------------|
| Vendor Code | String | Unique vendor identifier |
| Vendor Name | String | Name of the vendor |
| Contact Person | String | Primary contact |
| Email | Email | Vendor email |
| Phone | Phone Number | Contact number |
| Address | Multi-line Text | Vendor address |
| Vendor Type | Choice | Business category |
| Status | Choice | Current vendor status |
| GST Number | String | Tax registration number |
| Remarks | Multi-line Text | Additional notes |

---

## Vendor Types

- Hardware
- Software
- Cloud
- Network
- Office Supplies
- Security
- Other

---

## Status Values

- Active
- Inactive
- Blacklisted

---

## Design Decisions

The Vendor module has been designed as a standalone master table so it can be reused across multiple enterprise processes without data duplication.

Future integrations include:

- Procurement Management
- Asset Purchasing
- Warranty Tracking
- Contract Management
- Invoice Processing

---

## Concepts Learned

- Custom Table Creation
- Choice Fields
- Form Design
- Enterprise Data Modeling
- Master Data Management

---

## Screenshots

- Vendor Table
- Vendor Fields
---
