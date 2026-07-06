# CMS.gov Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cmsgov-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Access public healthcare data from the Centers for Medicare & Medicaid Services, including provider information.

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


## Available Tools (8)
- **get_dataset_metadata**: Returns the dataset title, full description, publication date, last modification date, and publisher information. Use the dataset ID obtained from list_datasets.

Get detailed metadata for a specific CMS dataset
- **get_doctor_by_npi**: Returns the provider's full name, primary and secondary specialties, practice address, city, state, ZIP code, and Medicare enrollment status. NPI is a unique 10-digit number (e.g. "1234567890").

Get detailed provider information by NPI number
- **get_hospital_ratings**: Filter by US state code (e.g. "CA", "NY", "TX") to see hospitals in that state. Returns overall ratings (1-5 stars), hospital type, and emergency services. Without a state filter, returns top-rated hospitals nationwide.

Get hospital quality ratings, optionally by state
- **list_datasets**: gov. Returns dataset identifiers, titles, descriptions, publication dates, and last-modified timestamps. The CMS data catalog includes datasets on Medicare utilization, hospital quality measures, provider enrollment, prescription drugs, and more.

List available CMS open data datasets
- **search_providers_by_specialty**: Examples: "Cardiology", "Internal Medicine", "Orthopedic Surgery", "Family Practice", "Dermatology", "Psychiatry". Returns matching providers with their NPI, name, practice location, and enrollment details.

Search for healthcare providers by medical specialty
- **search_doctors**: Accepts names, specialties, cities, or states. Returns NPI numbers, full names, primary specialty, practice addresses, and Medicare enrollment IDs. The database covers 2.4 million+ active providers across the United States.

Search for doctors and clinicians enrolled in Medicare
- **search_hospitals**: Accepts hospital names, cities, or states. Returns provider IDs, hospital names, types (Acute Care, Critical Access, etc.), overall quality ratings (1-5 stars), locations, and emergency services availability.

Search for hospitals by name or location
- **search_nursing_homes**: Returns facility names, provider IDs, locations, and overall quality ratings. Useful for finding elder care facilities in a specific area.

Search nursing homes and long-term care facilities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CMS.gov Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for cardiologists in New York using CMS.gov data."

**🤖 AI Agent:**
> I've searched the CMS Medicare provider database for cardiologists in New York. Found 847 enrolled cardiologists across the state. The top results include providers at major medical centers in Manhattan, Brooklyn, and the Bronx, with NPI numbers and practice addresses. Would you like me to get detailed information on any specific provider?

---

**👤 You:**
> "List top-rated hospitals in California according to CMS data."

**🤖 AI Agent:**
> I've retrieved hospital quality ratings for California from the CMS Hospital Compare program. There are 42 hospitals with a 5-star overall rating in the state, including facilities in Los Angeles, San Francisco, and San Diego. The ratings cover patient experience, mortality, readmission rates, and safety measures. Would you like me to compare specific hospitals or filter by region?

---

**👤 You:**
> "Get details for the provider with NPI 1234567890 from CMS."

**🤖 AI Agent:**
> I've retrieved the Medicare provider profile for NPI 1234567890. This is Dr. John Smith, a board-certified Internal Medicine specialist practicing at 123 Main Street, New York, NY 10001. Their Medicare enrollment ID is active and they accept Medicare assignment. Would you like to search for other providers in the same specialty or area?


## ❓ FAQ

**Q: Do I need an API key to use this server?**
No. The CMS.gov Provider Data API is completely public and requires no authentication. Simply subscribe to this server to start querying Medicare provider data, hospital ratings, and open datasets immediately.

**Q: How current is the data?**
CMS updates the Provider Data Catalog periodically, typically on a quarterly or monthly basis depending on the dataset. Hospital quality ratings are updated annually through the Hospital Compare program. All data is sourced directly from the official CMS.gov open data APIs.

**Q: What is an NPI number?**
The National Provider Identifier (NPI) is a unique 10-digit identification number issued by CMS to every US healthcare provider. It's the universal standard for identifying doctors, hospitals, and healthcare organizations in Medicare and Medicaid transactions. You can search for any provider by their NPI using this server.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cmsgov-data](https://vinkius.com/mcp/cmsgov-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CMS.gov Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cmsgov-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CMS.gov Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cmsgov-data": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
