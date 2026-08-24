# Accelerator Founder Coaching Hours MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-founder-coaching-hours)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculates optimal coaching hour distribution and topic prioritization for accelerator founders.

## Description
This MCP server provides a specialized calculation engine for accelerator programs to manage coaching resources. It determines how to distribute available coaching hours among founders using the `get_founder_hour_allocation` tool, which accounts for the number of founders and their experience level. It also helps prioritize learning subjects through `calculate_topic_priority` and evaluates resource efficiency with `compute_effectiveness_ratio`. This ensures that coaching time is aligned with the specific needs of each startup.


## Available Tools (3)
- **compute_effectiveness_ratio**: Evaluates how efficiently the coaching hours are being utilized relative to the needs and experience of the founders
- **get_founder_hour_allocation**: Determines how many hours each founder should receive based on the total pool and company structure
- **calculate_topic_priority**: Ranks the requested coaching topics to ensure critical subjects are addressed first


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Founder Coaching Hours** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many hours should 3 novice founders receive if there are 30 total hours available?"

**🤖 AI Agent:**
> Each founder should receive 12 hours, with a total of 36 hours requested, but since only 30 are available, the allocation will be adjusted to 10 hours per founder.

---

**👤 You:**
> "Prioritize these topics for an expert founder: Product-Market Fit, Fundraising, and Hiring."

**🤖 AI Agent:**
> The prioritized order for an expert founder is: 1. Fundraising, 2. Product-Market Fit, 3. Hiring.

---

**👤 You:**
> "Calculate the effectiveness for 20 hours allocated to 2 topics for an intermediate founder."

**🤖 AI Agent:**
> The effectiveness ratio is 0.85 with an efficiency rating of 'High'.


## ❓ FAQ

**Q: How does the tool determine hour distribution?**
The `get_founder_hour_allocation` tool calculates distribution by considering the total available hours, the number of founders, and their experience level (novice, intermediate, or expert).

**Q: Can I prioritize specific coaching topics?**
Yes, you can use `calculate_topic_priority` to rank requested subjects based on the founders' experience tier.

**Q: How is coaching efficiency measured?**
Efficiency is measured using `compute_effectiveness_ratio`, which evaluates the allocated hours against the number of topics and the founders' experience level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-founder-coaching-hours](https://vinkius.com/ai-agent-connect/accelerator-founder-coaching-hours)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Founder Coaching Hours** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-founder-coaching-hours` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Founder Coaching Hours** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-founder-coaching-hours": {
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
