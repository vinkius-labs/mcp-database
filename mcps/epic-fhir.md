# Epic Fhir MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/epic-fhir)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access patient records via Epic's FHIR R4 API — search patients, review encounters, pull lab results and medications from any AI agent.

## Description
Connect **Epic** electronic health records to any AI agent and query clinical data through natural conversation instead of navigating complex EHR interfaces.

### What you can do

- **Patient Search** — Find patients by name, date of birth, or medical record number across your Epic system
- **Clinical Encounters** — Review admissions, ER visits, and outpatient appointments with dates, reasons, and locations
- **Lab Results & Vitals** — Pull observations including blood work, vital signs, and social history with reference ranges
- **Diagnoses & Conditions** — List active and resolved conditions with ICD-10 codes, onset dates, and severity
- **Medications & Allergies** — View current prescriptions, dosage instructions, and documented allergic reactions
- **Appointments & Immunizations** — Check upcoming schedules and full vaccination history with lot numbers

### How it works

1. Subscribe to this server
2. Enter your FHIR Server URL, Client ID, and Access Token from your Epic App Orchard registration
3. Start querying patient records from Claude, Cursor, or any MCP-compatible client

Epic is the world's most widely used electronic health record system, serving over 305 million patients worldwide.

### Who is this for?

- **Clinical Informaticists** — extract patient cohort data and clinical metrics without writing SQL against the data warehouse
- **Care Coordinators** — quickly review a patient's full medical timeline before a care transition meeting
- **Health IT Developers** — prototype FHIR-based workflows and validate API responses interactively


## Available Tools
- **search_patients**: Returns patient demographics including name, DOB, gender, address, and identifiers.

Search patients by name, DOB, or MRN
- **list_immunizations**: Includes vaccine type (CVX code), administration date, dose, site, and lot number.

List immunizations
- **get_patient**: Returns name, DOB, gender, race, ethnicity, address, phone, email, and all identifiers.

Get patient details by ID
- **list_encounters**: Includes encounter type, period, reason, and location.

List patient encounters/visits
- **list_observations**: Filter by category: vital-signs, laboratory, social-history. Includes values, units, reference ranges, and interpretation.

List clinical observations
- **list_conditions**: Includes ICD-10 codes, clinical status, verification status, onset date, and severity.

List diagnoses and conditions
- **list_medications**: Includes medication name, dosage, frequency, route, prescriber, and status.

List medication requests
- **list_allergies**: Includes substance, reaction type, severity, and clinical status.

List allergies and intolerances
- **list_appointments**: Includes date/time, provider, location, and status.

List patient appointments
- **list_diagnostic_reports**: Includes report type, results, conclusion, and performing organization.

List diagnostic reports


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Epic Fhir** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all patients named Smith born in 1985."

**🤖 AI Agent:**
> Found 3 patients matching 'Smith' born in 1985:
1. John Smith (ID: e63wACU8F) — DOB: 1985-03-12, Male, MRN: 203847
2. Sarah Smith (ID: TnOZ.mfU4) — DOB: 1985-09-28, Female, MRN: 410293
3. Robert Smith (ID: eAr3bA.mH) — DOB: 1985-01-05, Male, MRN: 587102
Would you like to see the full medical history for any of these patients?

---

**👤 You:**
> "Show me the latest lab results for patient e63wACU8F."

**🤖 AI Agent:**
> Lab results for John Smith (last 30 days):
• Hemoglobin A1c: 6.2% (ref: <5.7% normal, 5.7-6.4% prediabetes) ⚠️
• Glucose (fasting): 118 mg/dL (ref: 70-100) ⚠️
• Creatinine: 0.9 mg/dL (ref: 0.7-1.3) ✓
• eGFR: 92 mL/min (ref: >60) ✓
• Total Cholesterol: 198 mg/dL (ref: <200) ✓
The A1c and fasting glucose are slightly elevated, suggesting prediabetic range. Want me to check current medications and conditions?

---

**👤 You:**
> "List all active medications for this patient."

**🤖 AI Agent:**
> Active medications for John Smith:
1. Metformin 500mg — 1 tablet twice daily with meals (Dr. Chen, prescribed 2024-11-15)
2. Lisinopril 10mg — 1 tablet daily (Dr. Chen, prescribed 2024-06-02)
3. Atorvastatin 20mg — 1 tablet at bedtime (Dr. Patel, prescribed 2024-03-10)
No known allergies documented. Want me to check the immunization record or upcoming appointments?


## ❓ FAQ

**Q: Can I search for a patient and instantly see their full medical timeline?**
Yes! Use `search_patients` with name or MRN to find the patient, then chain `list_encounters`, `list_conditions`, and `list_medications` to build a full clinical picture. Your agent compiles everything in seconds — no chart-clicking required.

**Q: How do I prepare a patient summary before a care coordination meeting?**
Ask your agent to pull everything at once: 'Show me the full medical history for patient ID abc123.' It will call `get_patient` for demographics, `list_conditions` for active diagnoses, `list_medications` for current prescriptions, and `list_allergies` for safety alerts — delivering a structured briefing ready for your meeting.

**Q: Is this integration read-only? Can it modify patient data?**
This integration is entirely read-only. All 10 tools are query operations — search, list, and retrieve. No tool can create, update, or delete any clinical data. Your Epic FHIR access token controls exactly which patients and resources are visible, enforcing your existing HIPAA access controls.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/epic-fhir](https://vinkius.com/mcp/epic-fhir)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Epic Fhir** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `epic-fhir` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Epic Fhir** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "epic-fhir": {
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
