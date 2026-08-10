# Semantic Versioning Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/semantic-versioning-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

A high-precision engine for validating and comparing Semantic Versioning 2.0.0 strings.

## Description
This MCP server provides precise tools for working with Semantic Versioning 2.0.0. It allows AI agents to validate version strings using `parse_version`, determine precedence between two versions with `compare_versions`, or sort a list of versions using `list_precedence_order`. It strictly adheres to SemVer rules, including pre-release precedence and build metadata handling.


## Available Tools (3)
- **compare_versions**: 0.0 rules. Build metadata is ignored.

Determines the precedence relationship between two SemVer versions
- **list_precedence_order**: Returns a sorted list of unique version strings based on SemVer precedence
- **parse_version**: Validates a SemVer 2.0.0 string and extracts its components


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Semantic Versioning Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is '1.0.0-beta.1' a valid SemVer string?"

**🤖 AI Agent:**
> Yes, '1.0.0-beta.1' is a valid Semantic Versioning 2.0.0 string.

---

**👤 You:**
> "Which version is higher: 1.2.3 or 1.2.3-rc.1?"

**🤖 AI Agent:**
> 1.2.3 is higher than 1.2.3-rc.1.

---

**👤 You:**
> "Sort these versions: 2.0.0, 1.0.0, 1.0.0-alpha"

**🤖 AI Agent:**
> 1.0.0-alpha, 1.0.0, 2.0.0


## ❓ FAQ

**Q: Does this tool support build metadata?**
Yes, `parse_version` extracts build metadata, though it is ignored during precedence comparisons as per the SemVer 2.0.0 specification.

**Q: How are pre-release versions handled?**
Pre-release versions are handled according to strict SemVer rules. For example, `1.0.0-alpha` is considered lower precedence than `1.0.0` when using `compare_versions`.

**Q: Can I sort multiple versions at once?**
Yes, you can use `list_precedence_order` to provide an array of version strings and receive them sorted from lowest to highest precedence.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/semantic-versioning-checker](https://vinkius.com/mcp/semantic-versioning-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Semantic Versioning Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `semantic-versioning-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Semantic Versioning Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "semantic-versioning-checker": {
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
