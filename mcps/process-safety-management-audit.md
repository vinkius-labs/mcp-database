# Process Safety Management Audit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/process-safety-management-audit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [compliance](../categories/compliance.md)

Automated OSHA 1910.119 compliance auditing for hazardous chemical facilities.

## Description
This MCP server provides a structured framework for evaluating facility compliance against the OSHA 1910.119 Process Safety Management (PSM) standard. It covers all 14 mandatory elements, including Process Safety Information, Process Hazard Analysis, and Mechanical Integrity. Users can use `audit_facility_compliance` to generate a comprehensive compliance profile, `identify_safety_gaps` to pinpoint specific non-compliance areas, and `generate_action_plan` to create prioritized remediation tasks. The tool also provides access to master requirements via `get_element_checklist` to assist in audit preparation.


## Available Tools (4)
- **audit_facility_compliance**: Performs a comprehensive audit of a facility against the 14 PSM elements to generate a compliance profile
- **generate_action_plan**: You can filter by priority.

Converts identified safety gaps into a prioritized list of corrective actions for management
- **get_element_checklist**: Retrieves the master standard requirements for any of the 14 PSM elements
- **identify_safety_gaps**: You can filter by a specific PSM element if needed.

Isolates specific areas of non-compliance to pinpoint where the facility is failing the OSHA standard


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Process Safety Management Audit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run a compliance audit for facility ID 'FAC-9928'."

**🤖 AI Agent:**
> The compliance audit for FAC-9928 is complete. The overall compliance score is 82%, with 4 total gaps identified across Mechanical Integrity and Training.

---

**👤 You:**
> "What are the specific requirements for the Management of Change element?"

**🤖 AI Agent:**
> The Management of Change element requires documented procedures for evaluating changes, technical basis for changes, and authorization protocols.

---

**👤 You:**
> "Show me the prioritized action items for facility 'FAC-9928' with critical priority."

**🤖 AI Agent:**
> The critical action items for FAC-9928 are: 1. Conduct immediate Process Hazard Analysis update. 2. Verify Mechanical Integrity testing records for pressure vessels.


## ❓ FAQ

**Q: What standard does this tool audit against?**
The tool audits against the OSHA 1910.119 Process Safety Management (PSM) standard, covering all 14 mandatory elements.

**Q: How can I find specific compliance failures?**
You can use the `identify_safety_gaps` tool to isolate specific areas of non-compliance and see which PSM elements are affected.

**Q: Can I generate a remediation plan from the audit results?**
Yes, once gaps are identified, you can use `generate_action_plan` to create a prioritized list of corrective actions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/process-safety-management-audit](https://vinkius.com/en/ai-agent-connect/process-safety-management-audit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Process Safety Management Audit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `process-safety-management-audit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Process Safety Management Audit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "process-safety-management-audit": {
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
