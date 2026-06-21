# Health Gorilla MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/health-gorilla)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Connect Health Gorilla to any AI agent via MCP.



## Available Tools (12)
- **cancel_lab_order**: Orders in "received" or "pending" status can typically be cancelled. Orders already in "collected" or "testing" status cannot be cancelled and require lab notification. A cancellation reason is recommended for audit purposes. Use this when an order was submitted in error, the patient refused testing, or clinical circumstances have changed.

Cancel a pending laboratory order
- **create_patient_record**: Required fields: first name, last name, date of birth, and gender. Optional: address, phone, email, MRN (Medical Record Number), and insurance information. Use this to register a new patient before submitting lab orders. Returns the patient ID for use in subsequent order submissions.

Create a new patient record in the Health Gorilla system
- **get_lab_results**: Returns structured data suitable for EHR integration or clinical review. Results include timestamp of completion, pathologist sign-off (if applicable), and any critical value notifications. Use this to review patient results, identify abnormal values, or populate EHR records.

Retrieve detailed laboratory results for a specific completed order
- **list_orders**: Optional filters: status (e.g., "pending", "completed", "cancelled") and patient_id. Each order includes order ID, patient name, test names, status, order date, and performing lab. Use this to review recent orders, track pending work, or audit ordering patterns.

List laboratory orders with optional filtering by status or patient
- **list_patient_results**: Includes test names, values, dates, and order references. Useful for trend analysis and longitudinal patient monitoring (e.g., tracking HbA1c over time, monitoring lipid panels). Use this for chronic disease management, preventive care follow-up, or comprehensive patient history review.

List all laboratory results for a specific patient across all orders
- **match_patient**: Returns match score and potential matches. Use this before creating new orders to avoid duplicate patient records and ensure results are attributed to the correct patient. Critical for data integrity in healthcare systems.

Match a patient against existing records in the Health Gorilla network
- **get_order_status**: Status values include: "received", "in_progress", "collected", "testing", "completed", "cancelled". Returns order details, specimen collection status, lab processing information, and estimated completion time. Use this to track order progress, update patients on result timelines, or verify completion status.

Check the current status of a submitted laboratory order
- **get_patient_demographics**: Returns name, DOB, gender, contact information, MRN, and registration date. Use this to verify patient identity before order submission or to review patient registration details.

Get demographic information for a registered patient
- **get_provider_details**: Use this to verify provider credentials, obtain contact information for referrals, or confirm network participation before ordering tests.

Get detailed information about a specific healthcare provider
- **search_providers**: Results include provider name, specialty, NPI number, location, and contact information. Use this to find ordering providers, verify network participation, or locate specialists in a specific area. Optional filters: specialty (e.g., "Internal Medicine", "Cardiology") and location.

Search for healthcare providers in the Health Gorilla network
- **search_lab_tests**: Returns test names, LOINC codes, categories (chemistry, hematology, microbiology, etc.), turnaround times, and performing laboratory information. Use this to find the correct test codes (LOINC/CPT) before submitting orders, explore available diagnostic options, or verify test availability. Optional query parameter accepts free-text search. Optional category parameter filters by test type.

Search the Health Gorilla lab test catalog by name, LOINC code, or category
- **submit_lab_order**: The order includes patient demographics, ordering provider information, requested tests (LOINC/CPT codes), clinical indication/diagnosis (ICD-10 codes), and specimen collection details. Returns an order ID for tracking status and retrieving results. Use this to place lab orders electronically without manual paperwork. Supported test types include chemistry panels, CBC, metabolic panels, infectious disease testing, genetic testing, and radiology orders. The order is routed to the appropriate performing laboratory (Quest, LabCorp, etc.).

Submit a new laboratory or radiology order through the Health Gorilla diagnostic network






## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/health-gorilla](https://vinkius.com/mcp/health-gorilla)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Health Gorilla** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `health-gorilla` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Health Gorilla** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "health-gorilla": {
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
