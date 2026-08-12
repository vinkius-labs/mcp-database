# Data Extraction Schema Evolver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/data-extraction-schema-evolver)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-extraction](../categories/data-extraction.md)

Automatically evolves JSON schemas to solve schema drift in LLM data extraction.

## Description
The Data Extraction Schema Evolver bridges the gap between static JSON schemas and the unpredictable nature of LLM outputs. By using `analyze_schema_drift`, it detects new fields and type mismatches. It then uses `propose_schema_evolution` to generate updated schemas via deterministic rules like type unionization and enum discovery. Finally, `validate_evolution_safety` ensures that schema changes remain reliable and don't introduce excessive structural loosening.


## Available Tools (3)
- **analyze_schema_drift**: Identifies structural differences between an existing schema and new observed data examples
- **propose_schema_evolution**: Generates a modified schema based on detected differences and new examples
- **validate_evolution_safety**: Evaluates if proposed schema changes are safe to deploy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Data Extraction Schema Evolver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify the differences between my current schema and these new extraction results."

**🤖 AI Agent:**
> I have detected a new field 'middle_name' and a type mismatch for 'age', which is now appearing as a string in some examples.

---

**👤 You:**
> "Propose a new schema that includes the changes found in the drift analysis."

**🤖 AI Agent:**
> The proposed schema has been updated to include 'middle_name' as an optional field and 'age' as a union of number and string.

---

**👤 You:**
> "Is this proposed schema evolution safe to deploy with strict settings?"

**🤖 AI Agent:**
> Yes, the evolution is safe. The changes only add optional fields and do not remove any required constraints.


## ❓ FAQ

**Q: How does the tool detect changes in my data?**
The `analyze_schema_drift` tool compares your existing schema against new JSON examples to identify new fields, missing fields, or type mismatches.

**Q: Can I control how much the schema changes?**
Yes, you can use `validate_evolution_safety` with a specific risk level (strict or flexible) to control how much structural loosening is permitted.

**Q: What happens if a field type changes from an integer to a string?**
The `propose_schema_evolution` tool will automatically perform type unionization, updating the schema to accept both integers and strings.


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
