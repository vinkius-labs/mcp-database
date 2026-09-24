# City Pass Value Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/city-pass-value-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate savings and find the best value City Pass for your planned attractions.

## Description
This MCP server connects your AI assistant to city attraction pricing data. Use `calculate_potential_savings` to see how much you save on specific trips, `find_break_even_attractions` to identify the minimum visits needed to justify a pass, or `evaluate_pass_efficiency` to compare different City Pass options for your selected attractions.


## Available Tools (4)
- **calculate_potential_savings**: Calculate savings from a City Pass
- **evaluate_pass_efficiency**: Compare different City Passes
- **find_break_even_attractions**: Find the break-even point for a City Pass
- **get_attraction_details**: Retrieve individual pricing for specific attractions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **City Pass Value Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will I save if I buy the Explorer Pass and visit the Museum, the Zoo, and the Aquarium?"

**🤖 AI Agent:**
> By purchasing the Explorer Pass for these three attractions, you will save $45.00.

---

**👤 You:**
> "Which attractions do I need to visit to make the Essential Pass worth the price?"

**🤖 AI Agent:**
> To reach the break-even point for the Essential Pass, you need to visit the Botanical Garden and the History Museum.

---

**👤 You:**
> "Compare the different passes for the Eiffel Tower and the Louvre."

**🤖 AI Agent:**
> The Ultimate Pass offers the highest savings for these attractions, providing a savings ratio of 2.5x.


## ❓ FAQ

**Q: How do I know if a City Pass is worth it?**
You can use the `calculate_potential_savings` tool to compare the total cost of individual tickets against the price of a City Pass.

**Q: Can I compare multiple passes at once?**
Yes, the `evaluate_pass_efficiency` tool allows you to compare different City Pass options for a specific list of attractions to find the best value.

**Q: What is the break-even point?**
The break-even point is the set of attractions where the individual ticket prices equal the cost of the City Pass. You can find this using `find_break_even_attractions`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/city-pass-value-calculator](https://vinkius.com/en/ai-agent-connect/city-pass-value-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **City Pass Value Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `city-pass-value-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **City Pass Value Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "city-pass-value-calculator": {
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
