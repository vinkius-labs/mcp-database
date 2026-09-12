# hazard-operability-study MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hazard-operability-study)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

A structured tool for conducting HAZOP studies on industrial processes.

## Description
This MCP server provides a systematic framework for conducting Hazard and Operability (HAZOP) studies. It allows users to initialize study sessions, define process nodes, and document deviations using standard guide words. By using tools like `add_node` and `record_deviation`, engineers can identify potential hazards, assess risks, and generate comprehensive reports to ensure industrial process safety.


## Available Tools (4)
- **add_node**: Defines a specific section (node) of the process to be analyzed
- **create_study_session**: Initializes a new HAZOP study environment based on process documentation
- **generate_study_report**: Aggregates all recorded data into a summary of the study's progress and findings
- **record_deviation**: Documents a specific hazard identified within a node


## 💬 Prompt Examples

Here are some examples of how you can interact with the **hazard-operability-study** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Start a HAZOP study for a Water Treatment Plant named 'WT-01' with a design intent of filtering raw water through sand filters."

**🤖 AI Agent:**
> Study session WT-01 has been initialized successfully.

---

**👤 You:**
> "Add a node called 'Main Feed Line' to my study with parameters Flow and Pressure."

**🤖 AI Agent:**
> Node 'Main Feed Line' has been added to the study session.

---

**👤 You:**
> "Record a deviation for the 'Main Feed Line' where there is MORE Pressure due to a downstream blockage."

**🤖 AI Agent:**
> Deviation 'MORE Pressure' has been recorded with a high risk level.


## ❓ FAQ

**Q: How do I start a new HAZOP study?**
You can start a new study by using the `create_study_session` tool, providing the process name, P&ID data, and the design intent.

**Q: Can I generate a summary of my findings?**
Yes, once you have recorded your deviations, you can use `generate_study_report` to get a summary of nodes, deviations, and high-risk findings.

**Q: What guide words are supported?**
The tool supports standard HAZOP guide words including NO, MORE, LESS, AS_WELL_AS, PART_OF, and REVERSE.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hazard-operability-study](https://vinkius.com/en/ai-agent-connect/hazard-operability-study)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **hazard-operability-study** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hazard-operability-study` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **hazard-operability-study** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hazard-operability-study": {
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
