# License Compatibility Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/license-compatibility-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Audit software licenses and check compatibility between dependencies.

## Description
This MCP server provides a specialized verification engine for auditing software license compatibility. Use `verify_spdx_identifier` to validate SPDX IDs, `check_perm_compatibility` to evaluate conflicts between project and dependency licenses, and `summarize_compliance_risk` to generate a high-level audit report of your entire dependency tree.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **License Compatibility Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is 'MIT' a valid SPDX identifier?"

**🤖 AI Agent:**
> Yes, 'MIT' is a recognized and valid SPDX identifier.

---

**👤 You:**
> "Check compatibility between 'GPL-3.0' and 'Apache-2.0'."

**🤖 AI Agent:**
> The compatibility status is incompatible because GPL-3.0 is a strong copyleft license.

---

**👤 You:**
> "Summarize the risk for an MIT project with dependencies: ['LGPL-2.1', 'Apache-2.0']."

**🤖 AI Agent:**
> The overall risk score is Medium, and active obligations include Attribution requirement and Library-handling obligations.


## ❓ FAQ

**Q: How do I check if a license is valid?**
Use the `verify_spdx_identifier` tool with the SPDX ID you want to validate. Tools available: `your_tool_name`.

**Q: Can it detect GPL conflicts?**
Yes, `check_pair_compatibility` identifies when strong copyleft licenses create incompatibility.

**Q: Does it support bulk analysis?**
Yes, `summarize_compliance_risk` analyzes an entire list of dependencies at once.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/license-compatibility-checker](https://vinkius.com/mcp/license-compatibility-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **License Compatibility Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `license-compatibility-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **License Compatibility Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "license-compatibility-checker": {
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
