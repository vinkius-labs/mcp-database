# Dependency License Compliance Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dependency-license-compliance-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Audit software dependencies against approved SPDX license identifiers to ensure supply-chain compliance.

## Description
This MCP server provides essential tools for securing the software supply chain by auditing dependency licenses. Use `audit_dependencies` to verify if a list of packages complies with your organization's whitelist, or use `get_dependency_license` to retrieve the specific SPDX identifier for a single package. The `validate_license_format` tool ensures that license strings are recognized SPDX identifiers. It acts as a bridge between your AI agent and your compliance policy, ensuring every dependency is vetted against your approved list.


## Available Tools (3)
- **audit_dependencies**: 
- **get_dependency_license**: 
- **validate_license_format**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dependency License Compliance Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are the dependencies npm:lodash@4.17.21 and npm:react@18.2.0 compliant with the MIT and Apache-2.0 licenses?"

**🤖 AI Agent:**
> Yes, both dependencies are compliant with the provided license list.

---

**👤 You:**
> "What is the license for npm:lodash@4.17.21?"

**🤖 AI Agent:**
> The license for npm:lodash@4.17.21 is MIT.

---

**👤 You:**
> "Is 'GPL-3.0' a valid SPDX identifier?"

**🤖 AI Agent:**
> Yes, 'GPL-3.0' is a valid and recognized SPDX identifier.


## ❓ FAQ

**Q: How do I check if my dependencies are compliant?**
You can use the `audit_dependencies` tool by providing a list of dependency strings and your list of allowed SPDX identifiers.

**Q: What is an SPDX identifier?**
An SPDX identifier is a standardized short-form name for a software license, such as MIT or Apache-2.0, used for precise matching.

**Q: Can I check a single package's license?**
Yes, use the `get_dependency_license` tool to find the specific SPDX identifier for any individual dependency string.


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
