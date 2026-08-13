# File Change Impact Assessor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/file-change-impact-assessor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Quantifies the blast radius and risk of file modifications through deterministic dependency tracing.

## Description
The File Change Impact Assessor is a deterministic tool designed to prevent regressions by quantifying the 'blast radius' of any file modification. By parsing import statements and building a dependency graph, it identifies exactly which files are transitively affected when a target is modified, deleted, or renamed. Use `analyze_impact` to determine the risk level and affected files, `get_dependency_graph` to visualize connections, and `identify_test_coverage` to pinpoint the specific tests required to validate a change.


## Available Tools (3)
- **identify_test_coverage**: Pinpoints specific test files that cover the logic of the target file
- **analyze_impact**: Determines the scope and risk of a proposed file change
- **get_dependency_graph**: Retrieves a structural view of how files are connected via imports


## 💬 Prompt Examples

Here are some examples of how you can interact with the **File Change Impact Assessor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the impact of modifying src/engine/index.ts?"

**🤖 AI Agent:**
> The impact radius is 12 files. The risk level is HIGH because src/engine/index.ts is a core module. Affected files include src/agents/tool.ts and several view components.

---

**👤 You:**
> "Show me the dependency connections for the current project."

**🤖 AI Agent:**
> The dependency graph shows a central hub in src/engine/index.js with multiple downstream importers in src/agents/ and src/views/.

---

**👤 You:**
> "Which tests should I run if I change src/agents/tool.ts?"

**🤖 AI Agent:**
> You should run src/agents/tool.test.ts and src/engine/index.test.ts to ensure full coverage.


## ❓ FAQ

**Q: How is the impact radius calculated?**
The impact radius is calculated by counting the unique files in the transitive dependency tree that import the target file or its importers.

**Q: What is the difference between MODIFY, DELETE, and RENAME?**
MODIFY updates content, DELETE removes the file, and RENAME changes the filename. All three trigger dependency checks to ensure importers are updated or accounted for.

**Q: Can I use this to find which tests to run?**
Yes, you can use the `identify_test_coverage` tool to find the specific test files that exercise the logic of your target file.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/file-change-impact-assessor](https://vinkius.com/mcp/file-change-impact-assessor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **File Change Impact Assessor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `file-change-impact-assessor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **File Change Impact Assessor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "file-change-impact-assessor": {
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
