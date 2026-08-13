# Data Extraction Schema Evolver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/data-extraction-schema-evolver)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-extraction](../categories/data-extraction.md)

Automatically detect schema drift and propose structural updates to JSON schemas.

## Description
The Data Extraction Schema Evolver solves the problem of schema drift in unstructured data extraction. By analyzing discrepancies between existing schemas and new data samples, it identifies new fields, type mismatches, and missing fields. Use `analyze_schema_drift` to detect changes, `propose_schema_evolution` to generate updated schemas with deterministic type inference, and `validate_evolution_safety` to ensure changes maintain structural integrity. This bridge connects your data pipelines to intelligent, self-healing schema management.


## Available Tools (3)
- **analyze_schema_drift**: Identifies discrepancies between a provided JSON schema and a collection of new data examples
- **propose_schema_evolution**: Generates a modified JSON schema based on drift analysis results
- **validate_evolution_safety**: Checks if the proposed schema changes are safe and do not destroy existing functionality


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Data Extraction Schema Evolver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a new set of JSON data. Can you check if it matches my current schema?"

**🤖 AI Agent:**
> I have analyzed the new data using `analyze_schema_drift`. I detected 2 new fields and 1 type mismatch.

---

**👤 You:**
> "Propose a new schema based on these recent data examples."

**🤖 AI Agent:**
> The proposed schema has been generated. It includes the new fields as optional and has updated the 'status' field to a union type.

---

**👤 You:**
> "Is this proposed schema change safe to apply?"

**🤖 AI Agent:**
> Yes, the change is safe. It only adds new optional fields and does not remove any existing mandatory fields.


## ❓ FAQ

**Q: What is schema drift?**
Schema drift occurs when the structure of unstructured data changes over time, causing existing extraction schemas to fail or miss new information.

**Q: How does the tool ensure schema changes are safe?**
You can use the `validate_evolution_safety` tool to verify that proposed changes only add optional fields or expand types, preventing the destruction of existing functionality.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, this MCP server can be connected to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/data-extraction-schema-evolver](https://vinkius.com/mcp/data-extraction-schema-evolver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Data Extraction Schema Evolver** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `data-extraction-schema-evolver` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Data Extraction Schema Evolver** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "data-extraction-schema-evolver": {
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
