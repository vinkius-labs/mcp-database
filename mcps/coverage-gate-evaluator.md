# Coverage Gate Evaluator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coverage-gate-evaluator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [quality-assurance](../categories/quality-assurance.md)

Enforce strict code coverage thresholds using deterministic integer math.

## Description
The Coverage Gate Evaluator MCP server provides a precise way to validate test coverage reports against predefined quality gates. By using deterministic integer arithmetic, it ensures that coverage percentages are calculated consistently across all environments. Use `parse_rule_tool` to decompose rule strings, `evaluate_report_tool` to check if your current covered and missed counts meet the required thresholds, and `calculate_shortfall_tool` to determine exactly how much more coverage is needed to pass a gate.


## Available Tools (3)
- **calculate_threshold_shortfall**: Calculates how much more coverage is needed to meet a threshold
- **evaluate_coverage_report**: g., ["line_coverage >= 80", "branch_coverage >= 70"]).

Evaluates a coverage report against a set of threshold rules
- **parse_coverage_rule**: Parses a single threshold rule string into its constituent parts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coverage Gate Evaluator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if my coverage report passes the threshold: 80 lines covered, 20 missed, with a rule of 'line_coverage >= 80'."

**🤖 AI Agent:**
> The coverage gate passed. Your line coverage is exactly 80%.

---

**👤 You:**
> "Parse this rule: 'branch_coverage >= 70'."

**🤖 AI Agent:**
> The rule has been parsed into metric: branch_coverage, operator: >=, and threshold: 70.

---

**👤 You:**
> "I have 65% coverage but I need 80%. How much more do I need?"

**🤖 AI Agent:**
> You need an additional 15% coverage to reach your target threshold of 80%.


## ❓ FAQ

**Q: How does the server calculate coverage percentages?**
The server uses deterministic integer math. It calculates the percentage by determining how many times the total number of units fits into the covered count, scaled to a base of one hundred.

**Q: Can I use this with my existing CI/CD pipeline?**
Yes. You can integrate the `evaluate_report_tool` into your CI/CD workflows to automatically fail builds if coverage falls below your specified thresholds.

**Q: What happens if the total number of units is zero?**
If the sum of covered and missed units is zero, the tool will return an error to prevent division by zero errors during calculation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coverage-gate-evaluator](https://vinkius.com/mcp/coverage-gate-evaluator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coverage Gate Evaluator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coverage-gate-evaluator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coverage Gate Evaluator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coverage-gate-evaluator": {
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
