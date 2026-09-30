# School Snack Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/school-snack-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Plan nutritious snack distributions for students while managing budgets and dietary restrictions.

## Description
The School Snack Planner connects AI agents to school inventory and nutritional management. Use `calculate_snack_needs` to determine exact quantities for student groups, `validate_snack_plan` to ensure dietary compliance and budget adherence, `check_stock_availability` to verify inventory, and `optimize_snack_selection` to find the most cost-effective snack combinations for your students.


## Available Tools (4)
- **calculate_snack_needs**: Determines the total quantity of specific snacks required
- **optimize_snack_selection**: Suggests a combination of snacks that maximizes the number of students fed
- **check_stock_availability**: Verifies if the requested quantities of snacks are available in the current inventory
- **validate_snack_plan**: Checks a proposed list of snacks against dietary exclusions, budget, and shelf life


## 💬 Prompt Examples

Here are some examples of how you can interact with the **School Snack Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many units of snack 'apple_slices_01' do I need for 50 students over 5 days?"

**🤖 AI Agent:**
> To feed 50 students for 5 days, you will need 250 units of apple slices.

---

**👤 You:**
> "Is my snack plan valid if I have a budget of $100 and want to include 'peanut_butter_01' which is on my exclusion list?"

**🤖 AI Agent:**
> No, the plan is invalid because 'peanut_butter_01' is included in the excluded snack IDs.

---

**👤 You:**
> "Find the best snack combination for 100 students for 3 days with a $150 budget, avoiding 'dairy_free_01'."

**🤖 AI Agent:**
> The optimized selection includes 300 units of 'granola_bars_02' and 300 units of 'juice_box_05' for a total cost of $135.00.


## ❓ FAQ

**Q: How do I ensure my snack plan stays within budget?**
You can use the `optimize_snack_selection` tool to automatically find a combination of snacks that maximizes student coverage while staying under your specified `budgetLimit`.

**Q: Can I exclude specific snacks due to allergies?**
Yes. When using `validate_snack_plan` or `optimize_snack_selection`, you can provide a list of `excludedSnackIds` to ensure forbidden items are never included in the plan.

**Q: How does the system handle food shelf life?**
The `validate_snack_plan` tool checks the remaining shelf life of every item against the `daysToCover` to ensure all snacks remain safe for the entire duration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/school-snack-planner](https://vinkius.com/en/ai-agent-connect/school-snack-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **School Snack Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `school-snack-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **School Snack Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "school-snack-planner": {
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
