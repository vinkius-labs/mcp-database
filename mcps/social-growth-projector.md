# Social Growth Projector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/social-growth-projector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Project follower growth using compound monthly percentage and viral spike scenarios.

## Description
The Social Growth Projector allows you to model social media audience progression. Use `predict_standard_growth` for steady baseline projections, or `predict_spike_growth` to simulate the impact of a viral event at a specific month. You can also use `calculate_spike_impact` to quantify exactly how much a one-time follower influx improves your long-term trajectory compared to standard growth.


## Available Tools (3)
- **calculate_spike_impact**: Calculate the impact of a viral spike
- **predict_spike_growth**: Project growth with a viral spike
- **predict_standard_growth**: Project baseline follower growth


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Social Growth Projector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If I have 10,000 followers and grow at 5% per month, how many will I have in 12 months?"

**🤖 AI Agent:**
> After 12 months of 5% monthly growth, your follower count will be approximately 17,958.

---

**👤 You:**
> "What happens if I get 5,000 new followers in month 3 due to a viral post, starting from 10,000 at 5% growth?"

**🤖 AI Agent:**
> With a 5,000 follower spike in month 3, your projected followers after 12 months will be approximately 24,718.

---

**👤 You:**
> "How much does a 2,000 follower spike in month 6 improve my final count after 12 months at 3% growth?"

**🤖 AI Agent:**
> The viral event results in a net gain of 2,000 followers and a percentage improvement of approximately 4.68% at the end of the 12-month period.


## ❓ FAQ

**Q: How does the compounding logic work?**
The tool applies the monthly growth rate to the updated follower count from the previous month, meaning each month's growth is based on the new, larger total.

**Q: Can I simulate a viral post?**
Yes, using `predict_spike_growth`, you can specify the number of followers gained and the exact month the spike occurs.

**Q: How do I compare a spike to my baseline?**
Use the `calculate_spike_impact` tool to see the net follower gain and percentage improvement resulting from a viral event.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/social-growth-projector](https://vinkius.com/mcp/social-growth-projector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Social Growth Projector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `social-growth-projector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Social Growth Projector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "social-growth-projector": {
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
