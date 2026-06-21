# Nubarium MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nubarium)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access Mexican identity and corporate data — audit RFC, CURP, and companies via AI.

## Description
Empower your AI agent to orchestrate your entire Mexican identity and corporate research workflow with **Nubarium**, the leading platform for Mexican data intelligence. By connecting Nubarium to your agent, you transform complex national lookups into a natural conversation. Your agent can instantly validate RFC (Tax ID) and CURP (Identity ID) records, audit company profiles, and verify legal representative status without you ever touching a manual portal. Whether you are conducting KYC checks or regional due diligence, your agent acts as a real-time institutional analyst, ensuring your Mexican data is always verified and up-to-date.

### What you can do

- **Identity Auditing** — Validate Mexican CURP records and retrieve detailed personal metadata, including names and birth details.
- **Tax Oversight** — Verify RFC registration status and retrieve comprehensive tax profiles for individuals and businesses.
- **Corporate Discovery** — Search for Mexican companies by name and retrieve detailed dossiers to understand organizational status.
- **Compliance Intelligence** — Verify the link between legal representatives and companies to assist in due diligence.
- **Operational Monitoring** — Check API usage metadata to maintain strict control over your research volume.

### How it works

1. Subscribe to this server
2. Enter your Nubarium API Key
3. Start managing your Mexican intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Compliance Officers** — monitor identity validation and retrieve official metadata straight from your workflow.
- **Risk Managers** — verify corporate backgrounds and audit legal representatives in Mexico without manual searching.
- **Data Analysts** — perform rapid audits of regional tax IDs and identify registration markers through natural language.
- **Operations Leads** — automate Mexican data querying to orchestrate cross-functional teams in the region smoothly.


## Available Tools (6)
- **validate_mex_curp**: Validate a Mexican CURP (identity ID) and retrieve details
- **validate_mex_rfc**: Validate a Mexican RFC (tax ID) and retrieve details
- **get_mex_company_details**: Get full details for a Mexican company by ID
- **get_api_usage**: Get current API usage metadata from Nubarium
- **search_mex_companies**: Search for companies in Mexico by name
- **validate_mex_legal_representative**: Verify the legal representative status for an RFC and CURP


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nubarium** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate the Mexican RFC 'ABC123456XYZ' using Nubarium."

**🤖 AI Agent:**
> RFC validated! The tax ID is active and associated with a registered entity in Mexico. Would you like to see the associated address or tax regime metadata?

---

**👤 You:**
> "Check the Mexican CURP for 'John Doe'."

**🤖 AI Agent:**
> I've retrieved the CURP details! The ID is valid and corresponds to the provided name. It identifies a birth record in Mexico City. Would you like the full identity metadata?

---

**👤 You:**
> "Find companies in Mexico with name 'Soluciones Tech'."

**🤖 AI Agent:**
> I've identified several companies named Soluciones Tech. Notable entries include entities in Guadalajara and Monterrey. Would you like the ID for any specific match to retrieve full dossiers?


## ❓ FAQ

**Q: How do I find my Nubarium API Key?**
Log in to your [**Nubarium dashboard**](https://nubarium.com/), and you will find your API Key under the 'API Settings' or 'My Keys' section. Copy and paste it below.

**Q: Can the agent validate Mexican tax IDs (RFC)?**
Yes. Use the `validate_mex_rfc` tool providing the RFC string. Your agent will verify its status with official sources instantly.

**Q: Is CURP validation supported for individuals?**
Yes. The `validate_mex_curp` tool allows your agent to check the identity status of individuals in Mexico using their unique CURP ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nubarium](https://vinkius.com/mcp/nubarium)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nubarium** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nubarium` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nubarium** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nubarium": {
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
