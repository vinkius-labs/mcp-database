# Textbook Cost Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/textbook-cost-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Compare costs and accessibility for new, used, rental, ebook, and library textbook options.

## Description
This MCP server provides decision support for students and educators to find the most economical way to acquire textbooks. By analyzing various procurement methods, it helps users understand the relationship between price, duration of use, and availability. Use `get_acquisition_options` to see all available formats, `compare_total_costs` to find the lowest monetary outlay for a specific period, `calculate_cost_per_day` to determine the best value efficiency, and `check_library_feasibility` to evaluate if library access is a viable alternative.


## Available Tools (4)
- **calculate_cost_per_day**: Evaluates the value efficiency of different options by determining the daily cost of access
- **check_library_feasibility**: Determines if a library-based acquisition is a viable alternative to purchasing
- **compare_total_costs**: Calculates and ranks the acquisition methods based on the lowest monetary outlay
- **get_acquisition_options**: Retrieves all available procurement methods for a specific textbook


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Textbook Cost Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the different ways I can get the textbook with ISBN 9780134093413?"

**🤖 AI Agent:**
> The available options for ISBN 9780134093413 include buying it new for $150, purchasing a used copy for $85, or renting it for $45 for a 90-day period.

---

**👤 You:**
> "Which is the cheapest option for ISBN 9780134093413 if I only need it for 30 days?"

**🤖 AI Agent:**
> The cheapest option for a 30-day period is the rental at $45.

---

**👤 You:**
> "Is it a good idea to use the library for ISBN 9780134093413 for my upcoming final exam?"

**🤖 AI Agent:**
> Library access for this ISBN is currently viable with an estimated wait time of 2 days and low availability risk.


## ❓ FAQ

**Q: How do I find the cheapest way to buy a book?**
You can use the `compare_total_costs` tool by providing the book's ISBN and the number of days you need it to find the lowest price.

**Q: Can I check if a library book is available for my exams?**
Yes, use the `check_library_feasibility` tool and specify if the book is required for an exam to see if library access is a reliable option.

**Q: What is the difference between total cost and value efficiency?**
Total cost is the absolute amount spent, while value efficiency (calculated via `calculate_cost_per_day`) tells you how much you pay for each day of access.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/textbook-cost-comparator](https://vinkius.com/en/ai-agent-connect/textbook-cost-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Textbook Cost Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `textbook-cost-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Textbook Cost Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "textbook-cost-comparator": {
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
