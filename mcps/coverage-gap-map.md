# Coverage Gap Map MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/coverage-gap-map)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Match insurance expenses against policy terms to identify coverage gaps.

## Description
Coverage Gap Map connects AI agents to insurance policy data. It allows for precise matching of requested expenses against policy clauses, limits, and exclusions. Use `analyze_expense_coverage` to check individual items, `identify_policy_limit_violations` to monitor category caps, `validate_incident_eligibility` to check for exclusions, and `generate_claim_action_summary` to produce final adjuster reports.


## Available Tools (4)
- **analyze_expense_coverage**: Determine if individual expenses are covered by the policy
- **generate_claim_action_summary**: Aggregate findings into a high-level summary for adjusters
- **identify_policy_limit_violations**: Check if total requested amounts exceed policy limits
- **validate_incident_eligibility**: Determine if the incident is excluded by the policy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coverage Gap Map** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these expenses against the policy: items: [{'itemId': '1', 'description': 'Water damage repair', 'amount': 500}], policy: [{'clauseId': 'C1', 'clauseText': 'Covers water damage', 'type': 'coverage', 'limitAmount': 1000}], incident: 'Pipe burst in kitchen'."

**🤖 AI Agent:**
> The expense for water damage repair is covered under clause C1.

---

**👤 You:**
> "Check if the total for 'Mitigation Cost' exceeds the limit of 500. Expenses: [{'itemId': '2', 'category': 'Mitigation Cost', 'amount': 600}]."

**🤖 AI Agent:**
> The total requested amount of 600 for Mitigation Cost exceeds the limit of 500 by 100.

---

**👤 You:**
> "Is a claim for 'Flood damage' eligible if the policy excludes 'Natural disasters'?"

**🤖 AI Agent:**
> No, the claim is not eligible because flood damage falls under the natural disasters exclusion.


## ❓ FAQ

**Q: How does the tool identify coverage gaps?**
The tool uses `analyze_expense_coverage` to compare expense descriptions against policy clauses and incident details to find mismatches or exclusions.

**Q: Can I check if I have exceeded my policy limits?**
Yes, the `identify_policy_limit_violations` tool sums expenses by category and compares them against defined policy limits.

**Q: Does this tool handle incident exclusions?**
Yes, `validate_incident_eligibility` checks the incident description against policy exclusions to determine if the claim is eligible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/coverage-gap-map](https://vinkius.com/en/ai-agent-connect/coverage-gap-map)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coverage Gap Map** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coverage-gap-map` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coverage Gap Map** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coverage-gap-map": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
