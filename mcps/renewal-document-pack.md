# Renewal Document Pack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/renewal-document-pack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [insurance](../categories/insurance.md)

Reconcile renewal questionnaires against policy data, asset changes, and evidence files.

## Description
This MCP server provides a specialized mapping engine to automate the renewal process. It reconciles renewal questionnaire requirements against existing policy data, asset updates, and evidentiary files to generate a structured document completion plan. Use `map_questionnaire_fields` to identify satisfied and missing requirements, `validate_asset_consistency` to ensure proposed changes are logically sound, `analyze_evidence_relevance` to verify document sufficiency, and `get_unresolved_gap_analysis` to prioritize missing information.


## Available Tools (4)
- **analyze_evidence_relevance**: Determine if an evidence file satisfies a specific questionnaire field
- **get_unresolved_gap_analysis**: Provide a prioritized list of missing information
- **map_questionnaire_fields**: Reconcile the renewal questionnaire against available data sources
- **validate_asset_consistency**: Ensure proposed asset changes do not contradict existing policy data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Renewal Document Pack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Map the questionnaire for policy ID 123 using these asset changes and evidence files."

**🤖 AI Agent:**
> The mapping is complete. 12 fields are satisfied by existing policy data, 3 fields are satisfied by the uploaded evidence, and 2 fields remain unresolved.

---

**👤 You:**
> "Is the uploaded invoice sufficient for the 'Proof of Address' requirement?"

**🤖 AI Agent:**
> Yes, the document provides sufficient information to satisfy the requirement.

---

**👤 You:**
> "Check if adding a new warehouse location conflicts with my current policy."

**🤖 AI Agent:**
> The proposed change is consistent with the current policy data.


## ❓ FAQ

**Q: How does the mapping process work?**
The engine uses `map_questionnaire_fields` to compare the target questionnaire schema against your current policy data, any asset modifications, and uploaded evidence files to determine what is ready and what is missing.

**Q: Can I validate changes before submitting them?**
Yes, you can use the `validate_asset_consistency` tool to ensure that proposed asset changes do not contradict fundamental policy data or existing records.

**Q: How do I find out what information is still missing?**
After running the mapping tool, you can use `get_unresolved_gap_analysis` to receive a prioritized list of missing information that requires manual intervention.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/renewal-document-pack](https://vinkius.com/en/ai-agent-connect/renewal-document-pack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Renewal Document Pack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `renewal-document-pack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Renewal Document Pack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "renewal-document-pack": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
