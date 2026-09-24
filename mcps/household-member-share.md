# Household Member Share MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-member-share)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Divides shared household costs equally among members.

## Description
This MCP server provides tools to manage shared household expenses. It allows users to calculate individual shares using `calculate_individual_share`, verify if an expense meets splitting criteria with `validate_expense_eligibility`, generate budget impact summaries via `get_cost_distribution_summary`, and confirm calculation accuracy with `verify_split_accuracy`.


## Available Tools (4)
- **calculate_individual_share**: Calculates how much each person owes for a specific expense
- **get_cost_distribution_summary**: Summarizes the total impact of a new cost on the household budget
- **validate_expense_eligibility**: Validates if a specific cost can be split based on household rules
- **verify_split_accuracy**: Verifies if a manual calculation of a split matches the system calculation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Member Share** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much does each person owe if the total grocery bill is $150.50 and there are 3 members?"

**🤖 AI Agent:**
> Each person owes $50.17.

---

**👤 You:**
> "Is a $50 utility bill eligible to be split if we only have 1 member?"

**🤖 AI Agent:**
> No, the expense is not eligible for splitting because the member count does not meet the minimum threshold.

---

**👤 You:**
> "Give me a summary for a $200 rent payment split among 4 people."

**🤖 AI Agent:**
> The total expense is $200.00 and the per-person impact is $50.00.


## ❓ FAQ

**Q: How do I calculate what each person owes?**
You can use the `calculate_individual_share` tool by providing the total cost and the number of members.

**Q: Can I check if an expense is eligible to be split?**
Yes, use `validate_expense_eligibility` to check if the current member count meets your household's minimum requirements.

**Q: How accurate are the calculations?**
The system ensures accuracy. You can use `verify_split_accuracy` to confirm that a manual calculation matches the system result within one cent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-member-share](https://vinkius.com/en/ai-agent-connect/household-member-share)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Member Share** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-member-share` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Member Share** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-member-share": {
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
