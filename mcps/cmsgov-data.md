# CMS.gov Data MCP Server

Access public healthcare data from the Centers for Medicare & Medicaid Services, including provider information.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cmsgov-data)

## Overview
**Category:** brain-trust
**Tools Count:** 8

## Description
Connect to the **Centers for Medicare & Medicaid Services (CMS)** open data platform and query the US government's most comprehensive healthcare database.

### What you can do

- **Provider Search** — Search 2.4 million+ Medicare-enrolled doctors and clinicians by name, specialty, or location, with NPI numbers and practice addresses
- **Hospital Intelligence** — Query hospital quality star ratings (1-5), types (Acute Care, Critical Access), and emergency services availability across all 50 states
- **Nursing Home Lookup** — Search skilled nursing facilities and long-term care homes with quality ratings and provider details
- **Open Data Catalog** — Browse and retrieve metadata from hundreds of CMS open datasets covering Medicare utilization, prescription drugs, and healthcare spending

### How it works

1. Subscribe to this server
2. No API key required — CMS.gov is a public open data service
3. Start querying healthcare data from Claude, Cursor, or any MCP-compatible client

Your AI agent gains direct access to the same data used by researchers, journalists, and policymakers to analyze the US healthcare system.

### Who is this for?

- **Healthcare Researchers** — query provider enrollment data and hospital quality metrics without navigating government portals
- **Journalists & Analysts** — instantly retrieve Medicare provider statistics for data-driven reporting
- **Patients & Caregivers** — find doctors by specialty and location, compare hospital ratings
- **Policy Professionals** — access open datasets on healthcare spending, utilization, and outcomes


## Available Tools
- **get_dataset_metadata**: Returns the dataset title, full description, publication date, last modification date, and publisher information. Use the dataset ID obtained from list_datasets.

Get detailed metadata for a specific CMS dataset
- **search_doctors**: Accepts names, specialties, cities, or states. Returns NPI numbers, full names, primary specialty, practice addresses, and Medicare enrollment IDs. The database covers 2.4 million+ active providers across the United States.

Search for doctors and clinicians enrolled in Medicare
- **search_hospitals**: Accepts hospital names, cities, or states. Returns provider IDs, hospital names, types (Acute Care, Critical Access, etc.), overall quality ratings (1-5 stars), locations, and emergency services availability.

Search for hospitals by name or location
- **search_providers_by_specialty**: Examples: "Cardiology", "Internal Medicine", "Orthopedic Surgery", "Family Practice", "Dermatology", "Psychiatry". Returns matching providers with their NPI, name, practice location, and enrollment details.

Search for healthcare providers by medical specialty
- **get_doctor_by_npi**: Returns the provider's full name, primary and secondary specialties, practice address, city, state, ZIP code, and Medicare enrollment status. NPI is a unique 10-digit number (e.g. "1234567890").

Get detailed provider information by NPI number
- **get_hospital_ratings**: Filter by US state code (e.g. "CA", "NY", "TX") to see hospitals in that state. Returns overall ratings (1-5 stars), hospital type, and emergency services. Without a state filter, returns top-rated hospitals nationwide.

Get hospital quality ratings, optionally by state
- **list_datasets**: gov. Returns dataset identifiers, titles, descriptions, publication dates, and last-modified timestamps. The CMS data catalog includes datasets on Medicare utilization, hospital quality measures, provider enrollment, prescription drugs, and more.

List available CMS open data datasets
- **search_nursing_homes**: Returns facility names, provider IDs, locations, and overall quality ratings. Useful for finding elder care facilities in a specific area.

Search nursing homes and long-term care facilities


## Installation & Usage

To install and use the **CMS.gov Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cmsgov-data](https://vinkius.com/mcp/cmsgov-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
