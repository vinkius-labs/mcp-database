# Environment Variable Usage Auditor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/environment-variable-usage-auditor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Cross-references environment variable usage against declaration files to find missing or unused keys.

## Description
The Environment Variable Usage Auditor prevents production crashes by ensuring your application code and configuration files are in sync. It identifies 'Ghost Variables' (used in code but missing from .env) and 'Dead Configuration' (declared in .cdotenv but never used). By using `extract_keys` to scan `.env`, `docker-compose.yml`, or Kubernetes ConfigMaps, and `extract_used_keys` to analyze your source code, you can then run `audit_consistency` to generate a complete parity report.


## Available Tools (3)
- **audit_consistency**: env) against a list of used keys (from code).

Audits consistency between declared and used environment variables
- **extract_keys**: Extracts keys from file contents (e.t. .env, docker-compose)
- **extract_used_keys**: g., .js, .ts, .py).

Extracts used environment variable keys from code contents


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Environment Variable Usage Auditor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if my environment variables are consistent for this project."

**🤖 AI Agent:**
> The audit is complete. The `isConsistent` status is true, meaning all declared keys match the used keys with no discrepancies found.

---

**👤 You:**
> "I have a list of keys from my .env file and a list from my code. Can you audit them?"

**🤖 AI Agent:**
> Yes, please provide the JSON arrays for both sets of keys, and I will use `audit_consistency` to identify any mismatches.

---

**👤 You:**
> "Extract all variable names from this .env content: 'PORT=3000
DB_URL=postgres://localhost'"

**🤖 AI Agent:**
> The extracted keys are: `PORT`, `DB_URL`.


## ❓ FAQ

**Q: What files does the auditor scan for declarations?**
It scans files like `.env`, `.env.example`, `docker-compose.yml`, and Kubernetes ConfigMaps using the `extract_keys` tool.

**Q: How can I find variables used in my TypeScript code?**
Use the `extract_used_keys` tool by providing the contents of your `.ts` or `.js` files.

**Q: What does a 'missing' variable mean?**
A missing variable is one that your code attempts to access (e.g., `process.env.API_KEY`) but which was not found in any of your declaration files.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/environment-variable-usage-auditor](https://vinkius.com/mcp/environment-variable-usage-auditor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Environment Variable Usage Auditor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `environment-variable-usage-auditor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Environment Variable Usage Auditor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "environment-variable-usage-auditor": {
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
