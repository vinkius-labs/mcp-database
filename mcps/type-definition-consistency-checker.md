# Type Definition Consistency Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/type-definition-consistency-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Ensure structural and type-level synchronization between TypeScript interfaces, Zod schemas, and Pydantic models.

## Description
The Type Definition Consistency Checker is a deterministic auditing tool designed to prevent structural drift in full-stack applications. By using AST-based parsing, it identifies discrepancies between frontend and backend schemas, such as missing fields, type mism/matches (e.g., string vs number), and optionality misalignments. Use `inspect_structure` to view parsed metadata, `sync_definitions` to perform a full-suite audit across multiple definitions, or `compare_definitions` for targeted reviews of specific changes.


## Available Tools (3)
- **compare_definitions**: Compare two type definitions
- **inspect_structure**: Inspect the structure of a type definition
- **sync_definitions**: Synchronize multiple type definitions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Type Definition Consistency Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if these two Zod schemas and TypeScript interfaces are in sync."

**🤖 AI Agent:**
> The `sync_definitions` audit is complete. No inconsistencies were detected; all fields, types, and optionality markers match perfectly.

---

**👤 You:**
> "What are the fields in this Pydantic model?"

**🤖 AI Agent:**
> The parsed structure contains the following fields: `user_id` (String-type, required), `email` (String-type, required), and `is_active` (Boolean-type, optional).

---

**👤 You:**
> "Compare this new interface with the existing one."

**🤖 AI Agent:**
> The `compare_definitions` tool identified one change: Field `last_login` was Added to the target definition.


## ❓ FAQ

**Q: What types of definitions can I check?**
The tool supports `typescript_interface`, `zod_schema`, and `pydantic_model` formats.

**Q: How does the tool detect errors?**
It uses deterministic AST parsing to extract field names, types, and optionality markers, then performs set comparison across your provided definitions.

**Q: Can I use this for a single Pull Request review?**
Yes, you can use the `compare_definitions` tool to perform a targeted comparison between a base definition and a target definition.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/type-definition-consistency-checker](https://vinkius.com/mcp/type-definition-consistency-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Type Definition Consistency Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `type-definition-consistency-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Type Definition Consistency Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "type-definition-consistency-checker": {
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
