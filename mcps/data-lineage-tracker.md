# Data Lineage Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/data-lineage-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [compliance](../categories/compliance.md)

Track the evolution and provenance of data through LLM pipelines.

## Description
Data Lineage Tracker provides a directed acyclic graph (DAG) to monitor how data items evolve through LLM workflows. It ensures auditability and compliance by recording every transformation step with a deterministic hash. Use `trace_transformation` to record new steps, `get_lineage_path` to reconstruct history, `verify_provenance` to confirm source ancestry, and `check_compliance_audit` to validate that required transformations have occurred.


## Available Tools (4)
- **check_compliance_audit**: 
- **get_lineage_path**: 
- **trace_transformation**: 
- **verify_provenance**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Data Lineage Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Record a summarization step for data item 'item_123' using the 'summarize' type."

**🤖 AI Agent:**
> The transformation has been recorded. The new output item ID is 'item_456' with hash 'abc123xyz'.

---

**👤 You:**
> "What is the full history of data item 'item_456'?"

**🤖 AI Agent:**
> The lineage for 'item_456' consists of 2 steps: a 'summarize' transformation and an 'augment' transformation, originating from root item 'item_000'.

---

**👤 You:**
> "Is 'item_000' an ancestor of 'item_456'?"

**🤖 AI Agent:**
> Yes, 'item_000' is an ancestor of 'item_456' with a path length of 2.


## ❓ FAQ

**Q: How do I record a new data transformation?**
You can use the `trace_transformation` tool to record a new step in the data's journey, providing the input ID, transformation type, parameters, and the resulting output data.

**Q: How can I verify if a piece of data is an ancestor of another?**
Use the `verify_provenance` tool to confirm if a specific source item is part of the lineage for a target item.

**Q: Can I check if my data pipeline meets compliance requirements?**
Yes, the `check_compliance_audit` tool allows you to validate that a data item's lineage includes all required transformation steps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/data-lineage-tracker](https://vinkius.com/mcp/data-lineage-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Data Lineage Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `data-lineage-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Data Lineage Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "data-lineage-tracker": {
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
