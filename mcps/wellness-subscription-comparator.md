# Wellness Subscription Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wellness-subscription-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Evaluate the true cost and utility of wellness memberships.

## Description
This MCP server helps you find the best value for your wellness routine. It analyzes gym, studio, and digital memberships by calculating effective cost per visit, usage efficiency, cancellation risks, and the hidden cost of travel time. Use `compare_subscriptions` to find new options, `analyze_usage_efficiency` to see if you are overpaying, `get_cancellation_risk` to check exit terms, and `calculate_travel_impact` to understand the time commitment of physical locations.


## Available Tools (4)
- **calculate_travel_impact**: Calculate the total monthly time investment required for travel to a physical membership
- **get_cancellation_risk**: Evaluate the financial and temporal risk of cancelling a membership
- **analyze_usage_efficiency**: Analyze the usage efficiency and cost-effectiveness of a specific membership
- **compare_subscriptions**: Compare wellness memberships based on type, expected visits, and optional travel time limit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wellness Subscription Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which gym memberships offer the best value if I plan to visit 8 times a month?"

**🤖 AI Agent:**
> The best value memberships for 8 visits per month are 'City Fitness' at $12.50 per visit and 'Zen Studio' at $15.00 per visit.

---

**👤 You:**
> "Am I overpaying for my current membership with ID 'gym_123' if I only went twice last month?"

**🤖 AI Agent:**
> Yes, with only 2 visits last month, your cost per visit is significantly higher than the category average, indicating you are overpaying.

---

**👤 You:**
> "How much time will I spend traveling per month if I visit 'YogaFlow' 3 times a week?"

**🤖 AI Agent:**
> You will spend a total of 120 minutes (2 hours) traveling to 'YogaFlow' per month.


## ❓ FAQ

**Q: How is the effective cost calculated?**
The effective cost is calculated by dividing the total monthly price of a membership by the number of expected or actual visits.

**Q: Can I compare digital apps and physical gyms?**
Yes, you can use `compare_subscriptions` to evaluate different categories like 'gym', 'studio', or 'digital' to find the best value.

**Q: What does the efficiency score mean?**
The efficiency score indicates how much value you are getting from your subscription relative to its cost. A higher score means better value.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wellness-subscription-comparator](https://vinkius.com/en/ai-agent-connect/wellness-subscription-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wellness Subscription Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wellness-subscription-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wellness Subscription Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wellness-subscription-comparator": {
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
