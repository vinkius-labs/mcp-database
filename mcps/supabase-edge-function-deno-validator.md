# Supabase Edge Function Deno Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/supabase-edge-function-deno-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [devops](../categories/devops.md)

Detect Node.js incompatibilities in Supabase Edge Functions before deployment.

## Description
Ensure your Supabase Edge Functions are ready for Deno Deploy. This MCP server provides deterministic validation of TypeScript code to prevent runtime failures caused by Node.js-specific patterns. Use `validate_deno_imports` to check for incompatible modules, `audit_node_imports` to identify risky imports like 'node:path', and `check_env_access` to ensure you are using Deno.env instead of process.env.


## Available Tools (3)
- **audit_node_imports**: js specific modules that might not work in Deno environments.

Audits Node.js imports in TypeScript code
- **check_env_access**: env or Deno.env is being used.

Checks for environment variable access in TypeScript code
- **validate_deno_imports**: Validates if TypeScript code is compatible with Deno


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Supabase Edge Function Deno Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this code compatible with Supabase Edge Functions: 'import fs from "node:fs"; console.log(process.env.KEY);'"

**🤖 AI Agent:**
> No, the code contains Node.js violations. It uses 'node:fs' and 'process.env', which are not supported in Deno.

---

**👤 You:**
> "Check if this function is safe for Deno: 'Deno.serve((req) => new Response("Hello"));'"

**🤖 AI Agent:**
> Yes, the code uses Deno.serve and is compatible with the Deno runtime.

---

**👤 You:**
> "Audit this snippet for Node.js imports: 'import path from "node:path";'"

**🤖 AI Agent:**
> The audit identified a violation: the use of 'node:path' is not compatible with Deno.


## ❓ FAQ

**Q: What does this MCP server do?**
It scans your TypeScript code for Node.js-specific patterns that will fail in the Deno runtime used by Supabase Edge Functions.

**Q: How can I check for Node.js imports?**
You can use the `audit_node_imports` tool to identify modules like 'node:fs' or 'node:path' that are not compatible with Deno.

**Q: Does it check environment variables?**
Yes, the `check_env_access` tool analyzes your code to ensure you are using Deno.env instead of the Node-specific process.env.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/supabase-edge-function-deno-validator](https://vinkius.com/ai-agent-connect/supabase-edge-function-deno-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Supabase Edge Function Deno Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `supabase-edge-function-deno-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Supabase Edge Function Deno Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "supabase-edge-function-deno-validator": {
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
