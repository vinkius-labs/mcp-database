# AST Cyclomatic Complexity Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ast-cyclomatic-complexity-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Measure code maintainability by calculating exact cyclomatic complexity using regex-based decision point counting.

## Description
The AST Cyclomatic Complexity Calculator provides a deterministic way to audit code maintainability. By scanning source code for specific control flow keywords and logical operators, it calculates the number of independent paths through each function. Use `analyze_complexity` to get a full breakdown of functions, `identify_refactor_candidates` to find high-risk functions exceeding the complexity threshold, or `compare_complexity_impact` to detect regressions between code versions.


## Available Tools (3)
- **analyze_complexity**: Analyze the cyclomatic complexity of source code
- **compare_complexity_impact**: Compare complexity between two versions of code
- **identify_refactor_candidates**: Identify functions that need refactoring


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AST Cyclomatic Complexity Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this function for complexity: 'function test(a) { if (a) { return true; } else { return false; } }'"

**🤖 AI Agent:**
> { "functions": [{"functionName": "test", "complexity": 2, "lineNumber": 1}], "totalComplexity": 2 }

---

**👤 You:**
> "Identify refactor candidates in this code: 'function heavy(x) { if (x) { if (x) { if (x) { if (x) { if (x) { if (x) { if (x) { if (x) { if (x) { if (x) { return 1; } } } } } } } } } }'"

**🤖 AI Agent:**
> { "highComplexityFunctions": [{"functionName": "heavy", "complexity": 11, "lineNumber": 1}] }

---

**👤 You:**
> "Compare the complexity of these two versions: 'function a() { return 1; }' and 'function b() { if (true) { return 1; } }'"

**🤖 AI Agent:**
> { "complexityDelta": 1, "isRegression": true, "newHighComplexityFunctionsCount": 0 }


## ❓ FAQ

**Q: How is complexity calculated?**
The tool counts decision points like `if`, `for`, `while`, and logical operators (`&&`, `||`) within a function, then adds 1 to the total count.

**Q: What does it mean if a function is a refactor candidate?**
A function is flagged via `identify_refactor_candidates` when its complexity score exceeds 10, indicating it has too many execution paths and is difficult to maintain.

**Q: Can I use this to check for regressions?**
Yes, the `compare_complexity_impact` tool allows you to compare two code snippets and see if changes increased the complexity or introduced a regression.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ast-cyclomatic-complexity-calculator](https://vinkius.com/mcp/ast-cyclomatic-complexity-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AST Cyclomatic Complexity Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ast-cyclomatic-complexity-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AST Cyclomatic Complexity Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ast-cyclomatic-complexity-calculator": {
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
