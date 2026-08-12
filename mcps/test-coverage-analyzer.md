# Test Coverage Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/test-coverage-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automated AST-based test coverage and logic gap analysis for LLM-generated code.

## Description
Test Coverage Analyzer connects AI agents to deep structural analysis of code quality. By parsing source code and test suites into Abstract Syntax Trees (AST), it identifies exactly which logic nodes are exercised and which remain untested. Use `analyze_coverage` to get a high-level overview of coverage and risk, `identify_uncovered_logic` to find specific structural gaps in complex functions, or `validate_test_mapping` to ensure a specific function is being correctly targeted by your tests.


## Available Tools (3)
- **analyze_coverage**: Calculate fundamental coverage metrics for a given pair of code and test strings
- **identify_uncovered_logic**: Provide a deep-dive into specific logic blocks that lack validation
- **validate_test_mapping**: Verify if the provided test suite is actually targeting the intended code structures


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Test Coverage Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the coverage for this code and test suite."

**🤖 AI Agent:**
> The coverage is 85%. The uncovered nodes are at lines 12 (Branch) and 15 (Loop). The critical path risk score is 0.4.

---

**👤 You:**
> "Find the logic gaps in this code where complexity is high."

**🤖 AI Agent:**
> The following gaps were found: function 'processData' (lines 45-60) with a complexity score of 8.5.

---

**👤 You:**
> "Is the function 'calculateTotal' covered by these tests?"

**🤖 AI Agent:**
> Yes, 'calculateTotal' is covered. It has 12 nodes hit out of 12 total nodes.


## ❓ FAQ

**Q: How does the tool calculate coverage?**
The tool uses deterministic AST traversal to map the execution paths of test cases against the set of all executable code nodes in the source code.

**Q: What is Critical Path Risk?**
It is a metric that identifies high-risk areas where complex logic (deep nesting or multiple branches) has zero test coverage.

**Q: Can I check if a specific function is covered?**
Yes, you can use the `validate_test_mapping` tool to verify if a specific target identifier is being exercised by the provided test suite.


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
