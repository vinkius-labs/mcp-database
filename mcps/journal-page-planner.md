# Journal Page Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/journal-page-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Divide journal pages among sections using precise percentage weights.

## Description
Journal Page Planner is a precision utility for partitioning journal page counts across various content sections. By assigning percentage weights to different parts of a journal, you can automatically calculate exact page allocations. The tool handles the mathematical complexity of rounding remainders to ensure the total page count is always fully accounted for. Use `get_section_distribution` to calculate allocations, `validate_weight_configuration` to ensure your weights sum to 100%, and `simulate_weight_adjustment` to predict how changes affect your layout.


## Available Tools (4)
- **get_distribution_summary**: Provides a high-level overview of a completed distribution plan
- **get_section_distribution**: Calculates how many pages should be allocated to each section based on their assigned weights
- **simulate_weight_adjustment**: Predicts how changing a section's weight will impact the page count distribution
- **validate_weight_configuration**: Verifies if a set of proposed section weights is mathematically valid for a full distribution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Journal Page Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Divide 200 pages among three sections: Daily Logs (60%), Weekly Reviews (30%), and Notes (10%)."

**🤖 AI Agent:**
> Daily Logs: 120 pages, Weekly Reviews: 60 pages, Notes: 20 pages. Total: 200 pages.

---

**👤 You:**
> "I have 150 pages. If I change the 'Notes' section from 5% to 10%, how many pages will it get?"

**🤖 AI Agent:**
> The 'Notes' section will now be allocated 15 pages.

---

**👤 You:**
> "Check if weights of 50%, 25%, and 20% are valid."

**🤖 AI Agent:**
> The weights are invalid because they sum to 95% instead of 100%.


## ❓ FAQ

**Q: How do I ensure all pages are accounted for?**
The `get_section_distribution` tool automatically calculates a remainder to ensure the sum of all section pages matches your total page count.

**Q: What happens if my weights don't add up to 100%?**
You can use `validate_weight_configuration` to check your weights. The tool will return an error if the total weight does not equal exactly 100.

**Q: Can I test changes before finalizing my plan?**
Yes, use `simulate_weight_adjustment` to see how changing a specific section's weight will impact its page count and the overall remainder.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/journal-page-planner](https://vinkius.com/en/ai-agent-connect/journal-page-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Journal Page Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `journal-page-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Journal Page Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "journal-page-planner": {
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
