# Family Screen Time Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-screen-time-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Aggregate and analyze screen time usage for family members to monitor digital wellness.

## Description
This MCP server provides tools to monitor and manage digital wellness within a household. It allows for calculating individual usage via `calculate_individual_total`, viewing the total family usage with `calculate_family_aggregate`, checking if members have exceeded their daily limits using `check_limit_compliance`, and analyzing usage patterns through `get_usage_trends`.


## Available Tools (4)
- **calculate_family_aggregate**: What is the combined screen time for everyone in the family today?
- **calculate_individual_total**: How much total screen time did a specific family member use today?
- **check_limit_compliance**: Has a specific family member exceeded their daily screen time limit?
- **get_usage_trends**: Is the screen time increasing or decreasing over the last few days?


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Screen Time Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much screen time did Alex use today?"

**🤖 AI Agent:**
> Alex used a total of 2h 15m of screen time today.

---

**👤 You:**
> "Did Sam exceed the 60 minute limit today?"

**🤖 AI Agent:**
> No, Sam is compliant with the 60 minute limit.

---

**👤 You:**
> "What was the total family screen time for 2024-05-20?"

**🤖 AI Agent:**
> The total family screen time for May 20th, 2024 was 450 minutes.


## ❓ FAQ

**Q: How can I check if my child exceeded their screen time limit?**
You can use the `check_limit_compliance` tool by providing the member's name, the date, and the specific minute threshold you want to enforce.

**Q: Can I see the total usage for the whole family at once?**
Yes, the `calculate_family_aggregate` tool provides the total combined minutes for all family members on a specific date, along with a breakdown per person.

**Q: How do I know if screen time is increasing for a specific person?**
Use the `get_usage_trends` tool to analyze the trend direction and daily history for a specific member over a set number of days.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-screen-time-total](https://vinkius.com/en/ai-agent-connect/family-screen-time-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Screen Time Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-screen-time-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Screen Time Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-screen-time-total": {
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
