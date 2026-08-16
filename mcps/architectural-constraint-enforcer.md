# Architectural Constraint Enforcer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/architectural-constraint-enforcer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Enforce project architecture and dependency rules via deterministic AST analysis.

## Description
Maintain structural integrity in your codebase with the Architectural Constraint Enforcer. This MCP server uses deterministic AST (Abstract Syntax Tree) analysis and dependency graph traversal to validate that code changes adhere to your specific project rules. It prevents 'spaghetti code' by enforcing layer boundaries, detecting circular dependencies, and validating naming conventions. Use `validate_file_compliance_tool` to check specific files, `check_module_relationships_tool` for direct dependency checks, or `get_project_compliance_summary_tool` for a high-level health report of your entire project.


## Available Tools (3)
- **validate_file_compliance_tool**: Checks if a specific file or a set of changed files adheres to the provided architectural rules
- **check_module_relationships_tool**: Answers if a specific relationship between two modules is permitted under the current architecture
- **get_project_compliance_summary_tool**: Provides a high-level overview of the entire project's health against the defined constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Architectural Constraint Enforcer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the current file follows our architectural rules."

**🤖 AI Agent:**
> The file is compliant with all defined layer boundaries and naming conventions.

---

**👤 You:**
> "Is there a circular dependency between the API and the Database layers?"

**🤖 AI Agent:**
> No circular dependencies were detected between the API and Database layers.

---

**👤 You:**
> "Give me a summary of the project's compliance score."

**🤖 AI Agent:**
> The project has an aggregate compliance score of 0.95 with 2 minor violations found in the test directory.


## ❓ FAQ

**Q: How does the tool detect circular dependencies?**
The tool builds a mathematical dependency graph from your source code and uses cycle detection algorithms to identify any loops where modules depend on each other.

**Q: Can I enforce specific naming conventions?**
Yes, you can use the structural tier rules to enforce conventions like PascalCase for components or specific file-system organization.

**Q: What is the difference between the validation tools?**
Use `validate_file_compliance_tool` for granular file checks, `check_module_relationships_tool` for testing a single dependency link, and `get_project_compliance_summary_tool` for a full project overview.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/architectural-constraint-enforcer](https://vinkius.com/ai-agent-connect/architectural-constraint-enforcer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Architectural Constraint Enforcer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `architectural-constraint-enforcer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Architectural Constraint Enforcer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "architectural-constraint-enforcer": {
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
