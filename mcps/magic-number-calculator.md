# Magic Number Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/magic-number-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate and analyze Go-To-Market efficiency using the Magic Number ratio.

## Description
The Magic Number Calculator is a specialized tool for evaluating Go-To-Market (GTM) efficiency. By comparing your Net New ARR from the current quarter against your Sales and Marketing (S&M) spend from the previous quarter, it calculates the Magic Number ratio to determine if your growth engine is inefficient, healthy, or excellent. Use `calculate_magic_number` to get the raw ratio, `get_efficiency_rating` to categorize performance tiers, and `evaluate_gtm_health_summary` for a comprehensive diagnostic of your business scaling efficiency.


## Available Tools
- **calculate_magic_number**: Calculate the Magic Number ratio
- **evaluate_gtm_health_summary**: Provide a holistic diagnostic of the GTM engine
- **get_efficiency_rating**: 5, 0.75, 1.0).

Categorize a Magic Number into its performance tier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Magic Number Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my Magic Number with $500,000 Net New ARR and $400,000 S&M spend."

**🤖 AI Agent:**
> Your Magic Number is 1.25, which indicates an excellent level of efficiency.

---

**👤 You:**
> "What is the efficiency rating for a magic number of 0.4?"

**🤖 AI Agent:**
> A Magic Number of 0.4 falls into the Inefficient tier, suggesting that your cost to acquire revenue is currently too high.

---

**👤 You:**
> "Evaluate my GTM health: $200,000 Net New ARR and $300,000 S&M spend."

**🤖 AI Agent:**
> Your GTM health status is Inefficient. The current ratio of 0.67 suggests your growth engine needs optimization to improve capital efficiency.


## ❓ FAQ

**Q: What is the Magic Number?**
The Magic Number is a SaaS metric that measures the efficiency of your Sales and Marketing spending relative to the revenue growth it generates.

**Q: How do I interpret the results?**
A ratio below 0.5 is considered inefficient, a ratio of 0.75 or higher is healthy, and a ratio of 1.0 or greater is excellent.

**Q: What inputs are required for the calculation?**
You need to provide your Net New ARR from the current quarter and your Sales and Marketing spend from the previous quarter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/magic-number-calculator](https://vinkius.com/mcp/magic-number-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Magic Number Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `magic-number-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Magic Number Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "magic-number-calculator": {
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
