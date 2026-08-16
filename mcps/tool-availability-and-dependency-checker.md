# Tool Availability and Dependency Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/tool-availability-and-dependency-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Audits tool environments for availability, version compatibility, and recursive dependency chains.

## Description
This MCP server provides a validation engine to prevent runtime execution failures in AI agent frameworks. It performs deep audits of the tool environment by verifying that all required tools are present, their versions satisfy specific constraints, and all recursive dependency chains are fully satisfied. Use `check_tool_readiness` to get a comprehensive readiness score, `validate_version_constraint` for specific version checks, or `resolve_dependency_tree` to map out deep-level requirements.


## Available Tools (3)
- **validate_version_constraint**: Determine if a specific version of a tool satisfies a provided version constraint
- **check_tool_readiness**: Perform a complete audit of the environment against a specific set of required tools
- **resolve_dependency_tree**: Map out the full chain of requirements for a specific tool to ensure no deep-level dependencies are missing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tool Availability and Dependency Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if my environment is ready for execution with these required tools."

**🤖 AI Agent:**
> The environment is ready. All required tools are ACTIVE and all version constraints and dependencies are satisfied with a readiness score of 1.0.

---

**👤 You:**
> "Is version 2.1.0 compatible with the constraint '^2.0.0'?"

**🤖 AI Agent:**
> Yes, version 2.1.0 satisfies the constraint '^2.0.0'.

---

**👤 You:**
> "Map out the dependencies for the primary tool."

**🤖 AI Agent:**
> The dependency tree for the primary tool is fully resolved and all nested requirements are present in the environment.


## ❓ FAQ

**Q: What does the readiness score represent?**
The readiness score is a value between 0.0 and 1.0 representing the proportion of satisfied requirements, including availability, versioning, and dependencies.

**Q: How does it handle tool dependencies?**
It uses recursive resolution. When you run `check_tool_readiness`, the engine ensures that if a tool requires another, that dependency is also checked for status and version compatibility.

**Q: Can I use this to check version ranges?**
Yes, the `validate_version_constraint` tool supports exact matches, minimum version thresholds, and range patterns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/tool-availability-and-dependency-checker](https://vinkius.com/ai-agent-connect/tool-availability-and-dependency-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tool Availability and Dependency Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tool-availability-and-dependency-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tool Availability and Dependency Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tool-availability-and-dependency-checker": {
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
