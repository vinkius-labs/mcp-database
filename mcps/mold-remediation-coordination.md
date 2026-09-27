# Mold Remediation Coordination MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mold-remediation-coordination)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [project-management](../categories/project-management.md)

Coordinate mold remediation workflows, professional escalations, and document preservation.

## Description
This MCP server provides a specialized coordination engine for managing mold remediation projects. It connects AI agents to critical workflows including `get_provider_clarifications` to identify quote gaps, `coordinate_temporary_access` for site entry logistics, `compare_remediation_options` for contractor analysis, and `generate_preservation_package` to ensure all environmental and legal records are preserved in the mandatory sequence. It is designed to maintain a strict non-diagnostic boundary while managing professional escalations and documentation.


## Available Tools (4)
- **compare_remediation_options**: Generates a structured comparison of various professional quotes
- **coordinate_temporary_access**: Use occupancy status to determine containment and security protocols.

Manages the logistics of granting remediation teams entry to the affected area
- **generate_preservation_package**: Moisture History, 2. Professional Assessment, 3. Quotes, 4. Lease/Insurance Documentation. Never include health diagnoses.

Compiles a legally and insurance-ready set of documents
- **get_provider_clarifications**: Identifies missing or ambiguous information in remediation quotes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mold Remediation Coordination** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare these three remediation quotes for the basement leak."

**🤖 AI Agent:**
> The comparison shows that Provider A has the lowest cost at $1,200, but Provider B offers higher scope coverage for the structural drying requirements identified in the assessment.

---

**👤 You:**
> "Generate a preservation package for the recent moisture event."

**🤖 AI Agent:**
> The preservation package (ID: PK-9928) has been compiled following the mandatory sequence: Moisture History, Professional Assessment, Quotes, and Lease/Insurance Documentation.

---

**👤 You:**
> "What questions should I ask the contractor regarding their quote?"

**🤖 AI Agent:**
> You should ask the contractor if the quote includes localized containment and whether the timeline accounts for the structural drying phase.


## ❓ FAQ

**Q: How does the tool handle contractor quotes?**
You can use `compare_remediation_options` to generate a structured comparison of different quotes based on cost, scope, and risk rating.

**Q: Can this tool provide medical advice?**
No. The server operates under a strict non-diagnostic boundary and is prohibited from generating health or medical diagnoses.

**Q: How is site access managed?**
The `coordinate_temporary_access` tool manages entry logistics based on whether the site is occupied, vacant, or partially occupied.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mold-remediation-coordination](https://vinkius.com/en/ai-agent-connect/mold-remediation-coordination)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mold Remediation Coordination** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mold-remediation-coordination` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mold Remediation Coordination** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mold-remediation-coordination": {
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
