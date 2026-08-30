# SDS Hazard Communication Evaluator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sds-hazard-communication-evaluator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [compliance](../categories/compliance.md)

Evaluates Safety Data Sheet (SDS) compliance against GHS and OSHA HCS standards.

## Description
This MCP server provides specialized tools to ensure Safety Data Sheets (SDS) meet global and regional regulatory requirements. Use `analyze_sds_completeness` to verify all mandatory sections are present for specific jurisdictions like the USA or EU. Use `evaluate_hazard_classification` to cross-reference hazard statements with chemical properties. You can also `generate_compliance_checklist` for a detailed pass/fail report and `recommend_improvements` to receive actionable steps for correcting compliance gaps.


## Available Tools (4)
- **analyze_sds_completeness**: g., USA or EU).

Determines if all mandatory sections required by a specific jurisdiction are present in the provided SDS
- **evaluate_hazard_classification**: Validates if the hazard classifications in the SDS align with the chemical properties described
- **generate_compliance_checklist**: Produces a granular, itemized checklist of regulatory requirements that have been met or failed
- **recommend_improvements**: Provides actionable advice to correct identified compliance gaps and improve hazard communication


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SDS Hazard Communication Evaluator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this SDS is complete for the USA: [SDS Text Content]"

**🤖 AI Agent:**
> The SDS is incomplete. Missing sections: 2 (Hazard Identification) and 15 (Regulatory Information).

---

**👤 You:**
> "Does this SDS hazard classification match these properties: Highly flammable liquid, clear liquid, colorless? [SDS Text Content]"

**🤖 AI Agent:**
> The classification matches the described properties.

---

**👤 You:**
> "Generate a compliance checklist for this SDS for the EU: [SDS Text Content]"

**🤖 AI Agent:**
> Compliance Score: 85%. Passed: Section 1, 3, 4. Failed: Section 2 (Missing pictogram for flammability).


## ❓ FAQ

**Q: Which jurisdictions are supported?**
The server supports major regulatory frameworks including GHS, USA (OSHA HCS), and EU (CLP/REACH).

**Q: Can I use this to find missing sections in my SDS?**
Yes, the `analyze_sds_completeness` tool specifically identifies which mandatory sections are missing based on the selected jurisdiction.

**Q: How do I get advice on fixing errors?**
You can use the `recommend_improvements` tool by providing the output from a completeness or checklist analysis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sds-hazard-communication-evaluator](https://vinkius.com/ai-agent-connect/sds-hazard-communication-evaluator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SDS Hazard Communication Evaluator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sds-hazard-communication-evaluator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SDS Hazard Communication Evaluator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sds-hazard-communication-evaluator": {
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
