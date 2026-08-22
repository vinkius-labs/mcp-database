# Side Hustle Viability Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/side-hustle-viability-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Deterministic financial feasibility analysis for side hustles in Singapore.

## Description
This MCP server provides precise financial modeling for young professionals in Singapore looking to start a side hustle. By using `calculate_viability`, users can determine if their intended venture--whether it be freelance work, e-commerce, or ride-hailing--is truly worth the time investment. The tool calculates gross hourly rates, effective hourly rates after platform fees and taxes, and the opportunity cost relative to a primary job. You can also use `simulate_profit_scenarios` to run 'what-if' analyses on different income targets and weekly hours to find the optimal path to profitability.


## Available Tools (3)
- **calculate_viability**: Determines if a specific side hustle is financially worth the time investment relative to a user's current employment
- **get_side_hustle_profiles**: Provides a list of available side hustle types
- **simulate_profit_scenarios**: Compares how changing effort or income targets affects viability and break-even point


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Side Hustle Viability Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is a freelance gig earning 2000 SGD a month for 15 hours a week worth it if my main job pays 30 SGD per hour? My startup costs are 500 SGD."

**🤖 AI Agent:**
> The effective hourly rate is approximately 22.50 SGD. Since this is less than 50% of your main job's rate, the viability score is 'Not Worth It'. You will break even in 2.22 months.

---

**👤 You:**
> "Calculate the viability of an e-commerce business earning 4000 SGD monthly with 20 hours of work per week. My main job pays 40 SGD/hour and startup costs are 2000 SGD."

**🤖 AI Agent:**
> The effective hourly rate is 45.00 SGD. Since this exceeds your main job's rate, the viability score is 'Highly Viable'. You will break even in 1.11 months.

---

**👤 You:**
> "What are the available side hustle types I can calculate?"

**🤖 AI Agent:**
> The supported side hustle types are freelance, e-commerce, tutoring, content_creation, and ride_hailing.


## ❓ FAQ

**Q: How is the effective hourly rate calculated?**
The effective hourly rate is the take-home pay per hour after deducting 20% for platform fees, 15% for taxes, and equipment amortization from the gross monthly income.

**Q: What does a 'Highly Viable' score mean?**
A 'Highly Viable' score indicates that the side hustle's effective hourly rate is higher than your current main job's hourly rate.

**Q: Can I test different scenarios?**
Yes, you can use the `simulate_profit_scenarios` tool to compare how changes in your weekly hours or expected income affect your viability and break-even period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/side-hustle-viability-calculator](https://vinkius.com/ai-agent-connect/side-hustle-viability-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Side Hustle Viability Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `side-hustle-viability-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Side Hustle Viability Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "side-hustle-viability-calculator": {
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
