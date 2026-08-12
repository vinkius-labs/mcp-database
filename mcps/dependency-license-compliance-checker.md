# Dependency License Compliance Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dependency-license-compliance-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Validates software dependencies against approved SPDX license identifiers.

## Description
This MCP server provides tools to ensure software supply-chain security by validating dependency licenses. Use `check_license_compliance` to verify a list of packages against a policy, `get_dependency_license` to look up a specific package's SPDX identifier, or `list_allowed_license_templates` to see common permitted licenses. It helps maintain compliance by flagging non-permitted licenses automatically.


## Available Tools (3)
- **check_license_compliance**: 
- **get_dependency_license**: 
- **list_allowed_license_templates**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dependency License Compliance Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are these dependencies compliant with MIT and Apache-2.0 licenses: npm:lodash@4.17.21, npm:react@18.2.0?"

**🤖 AI Agent:**
> Yes, both dependencies are compliant with the specified licenses.

---

**👤 You:**
> "What is the license for npm:react@18.2.0?"

**🤖 AI Agent:**
> The license for npm:react@18.2.0 is MIT.

---

**👤 You:**
> "Check if npm:express@4.17.1 is compliant with MIT."

**🤖 AI Agent:**
> Yes, npm:express@4.17.1 is compliant with the MIT license.


## ❓ FAQ

**Q: How do I check if my dependencies are compliant?**
You can use the `check_license_compliance` tool by providing a list of dependency strings and your list of allowed SPDX identifiers.

**Q: What is an SPDX identifier?**
An SPDX identifier is a standardized short-form text string used to identify software licenses, such as 'MIT' or 'Apache-2.0'.

**Q: Can I see a list of common licenses?**
Yes, use the `list_allowed_license_templates` tool to retrieve a reference list of widely accepted SPDX license identifiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dependency-license-compliance-checker](https://vinkius.com/mcp/dependency-license-compliance-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dependency License Compliance Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dependency-license-compliance-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dependency License Compliance Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dependency-license-compliance-checker": {
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
