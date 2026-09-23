# Study Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/study-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate cumulative expenditures for courses, books, and study materials.

## Description
This MCP server provides tools to aggregate the total cost of educational resources. It allows AI agents to calculate specific costs for courses using `get_course_costs`, reading lists via `get_book_costs`, and physical supplies with `get_material_costs`. For a complete financial overview, use `calculate_total_study_expenditure` to get a grand total and a detailed breakdown of all study-related expenses.


## Available Tools (4)
- **calculate_total_study_expenditure**: 
- **get_book_costs**: 
- **get_course_costs**: 
- **get_material_costs**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Study Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost for courses C1, C2 and books B1?"

**🤖 AI Agent:**
> The total cost for the selected courses and books is $150.00.

---

**👤 You:**
> "Calculate the full study expenditure for courses [C1], books [B1], and materials [M1]."

**🤖 AI Agent:**
> The grand total is $210.00, consisting of $100.00 for courses, $80.00 for books, and $30.00 for materials.

---

**👤 You:**
> "How much will the required materials cost for these IDs: M1, M2?"

**🤖 AI Agent:**
> The total cost for the requested materials is $45.00.


## ❓ FAQ

**Q: How do I calculate the total cost of my entire study plan?**
You can use the `calculate_total_study_expenditure` tool, providing the IDs for your courses, books, and materials to get a complete breakdown.

**Q: Can I get the cost for just the books?**
Yes, use the `get_book_costs` tool by providing the list of book IDs.

**Q: What happens if a course ID is not found?**
If a course ID does not exist in the catalog, it is simply ignored in the total sum.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/study-cost-calculator](https://vinkius.com/en/ai-agent-connect/study-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Study Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `study-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Study Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "study-cost-calculator": {
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
