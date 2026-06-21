# Optum Eligibility MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/optum-eligibility)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Verify patient active healthcare coverage, extract deductibles, and run real-time UHG demographics.

## Description
### What you can do

Take complete proxy control over your Medical Front-Desk operations, accelerating the intake of patients with automated real-time checks acting securely under Optum APIs:

- **Check Active Eligibility:** Run advanced X12 270/271 mappings extracting if a patient holds an active healthcare policy seamlessly.
- **Verify Deductibles:** Quickly identify out-of-pocket limits and met thresholds for an individual efficiently.
- **Check Provider Network:** Look up if a specific doctor or facility operates strictly 'In-Network'.

### How it works

1. **High Security & Compliance:** Engineered entirely to handle Front-Desk requests (Reading PHI Demographics/Status only). This architecture deliberately excludes Financial/Claim mutations.
2. **Engage OAuth Protocol:** Authorize directly substituting your institutional `CLIENT_ID` securely within the runtime module.
3. **Deploy:** Offload reception verification workflows immediately.

### Who is this for?

Specifically built for **Hospital Receptionists**, **Clinic Managers**, and **Healthcare Tech Integrators**.


## Available Tools
- **opt_check_eligibility**: Verify if a patient has active healthcare coverage. Maps to X12 270/271 EDI transactions securely
- **opt_get_benefit_details**: Pulls granular coverage rules indicating if a specific medical service requires prior authorization
- **opt_get_deductibles**: Extract remaining out-of-pocket maximums and deductibles for a specific health plan member
- **opt_search_patient_demographics**: Search the healthcare database for a patient record matching specific demographic parameters securely
- **opt_verify_provider_network**: Checks if a specific doctor or medical facility is In-Network for the given patient policy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Optum Eligibility** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the remaining deductibles and out-of-pocket maximum amounts for patient ID 99281."

**🤖 AI Agent:**
> Query completed. Patient 99281 has a remaining active deductible of $1,250 towards an annual ceiling.

---

**👤 You:**
> "Find if John Doe is currently eligible for an MRI under policy HDHP-77."

**🤖 AI Agent:**
> Eligibility verified. John Doe is active under HDHP-77 but MRIs require prior authorization before service delivery.

---

**👤 You:**
> "List all dependents covered under Member ID UB-11202."

**🤖 AI Agent:**
> Located dependents under subscriber UB-11202: 1 Spouse (Active) and 2 Toddler dependents (Active) currently attached.


## ❓ FAQ

**Q: Can this Optum Server submit medical claims or process remittances automatically?**
Absolutely strictly not. Per rigorous Least Privilege modeling common to US Healthcare operations, Front-Desk tasks (Eligibility) are decoupled natively from Back-Office operations. For submitting medical claims, integrate the `optum-claims-mcp` array safely.

**Q: How does the agent handle HIPAA compliance for patient data?**
The MCP server transmits data directly via secure Optum APIs over TLS. No PHI (Protected Health Information) is cached locally, ensuring full compliance with HIPAA regulations.

**Q: Can I check out-of-network benefits?**
Yes. The eligibility payload returns detailed tiered benefits including deductibles and coinsurance for out-of-network services based on the specific policy details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/optum-eligibility](https://vinkius.com/mcp/optum-eligibility)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Optum Eligibility** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `optum-eligibility` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Optum Eligibility** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "optum-eligibility": {
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
