# Test Coverage Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/test-coverage-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Analyze test coverage and identify high-risk untested code using AST analysis.

## Description
Test Coverage Analyzer provides deep visibility into how well your test suites exercise agent-generated code. By using deterministic Abstract Syntax Tree (AST) traversal, it identifies exactly which functions and classes are covered and which remain untested. Use `analyze_code_coverage` to get a full coverage percentage and a list of uncovered nodes. Use `identify_uncovered_complex_logic` to pinpoint high-risk areas where complex logic lacks verification. You can also use `map_test_targets` to confirm which specific code elements are being exercised by your tests. This tool helps ensure the auditability and reliability of LLM-generated workflows.


## Available Tools (3)
- **analyze_code_coverage**: Provides a complete overview of how well the provided test suite exercises the source code
- **identify_uncovered_complex_logic**: Specifically pinpoints high-risk areas where complex logic is completely unverified
- **map_test_targets**: Determines exactly which functions and classes are being targeted by the provided test suite


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Test Coverage Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the test coverage for this code?"

**🤖 AI Agent:**
> The current test coverage is 85%. There are 2 uncovered nodes at lines 12 and 45.

---

**👤 You:**
> "Are there any high-risk areas in my code?"

**🤖 AI Agent:**
> Yes, the function `process_data_stream` at line 50 is high risk due to its high complexity and zero test coverage.

---

**👤 You:**
> "Which functions are being tested by this suite?"

**🤖 AI Agent:**
> The test suite targets the following: `calculate_total` (covered) and `validate_user` (uncovered).


## ❓ FAQ

**Q: How is coverage calculated?**
Coverage is calculated by comparing the set of all executable nodes in the source AST against the set of nodes traversed during the test execution simulation.

**Q: What is a critical path risk score?**
It is a metric representing the danger level of untested code, weighted by the logical complexity of the functions left uncovered.

**Q: Can I use this with any programming language?**
The tool uses AST traversal, so its support depends on the specific language parsers implemented in the engine.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/test-coverage-analyzer](https://vinkius.com/mcp/test-coverage-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Test Coverage Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `test-coverage-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Test Coverage Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "test-coverage-analyzer": {
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
