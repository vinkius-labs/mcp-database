# SemVer Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/semver-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Validate, compare, and manipulate Semantic Versioning 2.0.0 strings.

## Description
The SemVer Calculator provides a set of tools to handle Semantic Versioning 2.0.0 operations with precision. You can use `validate_version` to ensure strings follow the spec, `compare_versions` to determine precedence between two versions, and `calculate_next_version` to automate bumps for major, minor, or patch changes. Additionally, it supports checking compatibility via `check_range_satisfaction` and ordering lists with `sort_version_list`.


## Available Tools (5)
- **sort_version_list**: Orders an array of version strings from lowest precedence to highest precedence
- **calculate_next_version**: Computes a new version string based on an existing version and a requested change type
- **check_range_satisfaction**: 2.3 or ~1.2.0.

Checks if a single version string falls within a defined range of allowed versions
- **compare_versions**: Determines the precedence relationship between two specific version strings
- **validate_version**: Verifies that a given string strictly adheres to the SemVer 2.0.0 syntax


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SemVer Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is '1.2.3-alpha.1' a valid version?"

**🤖 AI Agent:**
> Yes, '1.2.3-alpha.1' is a valid SemVer 2.0.0 string.

---

**👤 You:**
> "Which version is higher: 2.0.0 or 1.9.9?"

**🤖 AI Agent:**
> Version 2.0.0 is greater than 1.9.9.

---

**👤 You:**
> "What is the next version after 1.5.2 if I apply a minor bump?"

**🤖 AI Agent:**
> The next version after 1.5.2 with a minor bump is 1.6.0.


## ❓ FAQ

**Q: What is Semantic Versioning?**
Semantic Versioning (SemVer) is a convention for version numbers that uses MAJOR.MINOR.PATCH format to communicate breaking changes, features, and bug fixes.

**Q: How can I check if a version is valid?**
You can use the `validate_version` tool to verify that any string strictly adheres to the SemVer 2.0.0 syntax.

**Q: Can I automate version increments?**
Yes, the `calculate_next_version` tool allows you to compute the next version based on a major, minor, or patch bump.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/semver-calculator](https://vinkius.com/mcp/semver-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SemVer Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `semver-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SemVer Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "semver-calculator": {
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
