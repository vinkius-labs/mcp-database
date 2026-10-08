# Freelance Rate Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/freelance-rate-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate sustainable hourly rates based on income targets, taxes, and overhead.

## Description
This MCP server helps freelancers determine a sustainable hourly rate. It accounts for personal income targets, business overhead, tax obligations, and a profit buffer. Use `get_rate_summary` to see a full breakdown of your required revenue, or `compare_rates` to see how different billable hour scenarios change your rate. It also includes tools like `calculate_overhead_impact` to adjust for rising costs and `estimate_tax_burden` to plan for tax season.


## Available Tools (4)
- **calculate_overhead_impact**: Determines how much the hourly rate must increase to cover a specific change in business expenses
- **compare_rates**: Evaluates how different billable hour scenarios affect the required hourly rate
- **estimate_tax_burden**: Calculates the total amount of money that must be set aside for taxes based on a target gross revenue
- **get_rate_summary**: Provides a complete breakdown of the calculated hourly rate and its component parts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freelance Rate Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to earn $60,000 net per year. I have $5,000 in overhead, 1200 billable hours, and a 25% tax rate. What should my hourly rate be?"

**🤖 AI Agent:**
> To reach a net income of $60,000 with $5,000 in overhead and a 25% tax rate, your required hourly rate is $73.33.

---

**👤 You:**
> "How much tax will I pay if I invoice $100,000 and my tax rate is 30%?"

**🤖 AI Agent:**
> At a 30% tax rate, your tax amount will be $30,000, leaving you with a net of $70,000.

---

**👤 You:**
> "My annual overhead is increasing by $2,000. I currently charge $50/hour and work 1,000 billable hours. How much should I increase my rate?"

**🤖 AI Agent:**
> An increase of $2,000 in annual overhead requires a rate increase of $2.00 per hour, making your new hourly rate $52.00.


## ❓ FAQ

**Q: How do I calculate my target income?**
Define the net amount you need for your lifestyle and personal savings. You can use `get_rate_summary` to see how this target translates into an hourly rate after accounting for taxes and overhead.

**Q: Can I see how changing my billable hours affects my rate?**
Yes, use the `compare_rates` tool. You can provide multiple annual billable hour scenarios to see how each one impacts the required hourly fee.

**Q: How does overhead affect my rate?**
Overhead costs like software or rent must be covered by your revenue. You can use `calculate_overhead_impact` to determine exactly how much your rate needs to increase if your expenses go up.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/freelance-rate-builder](https://vinkius.com/en/ai-agent-connect/freelance-rate-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Freelance Rate Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `freelance-rate-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Freelance Rate Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "freelance-rate-builder": {
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
