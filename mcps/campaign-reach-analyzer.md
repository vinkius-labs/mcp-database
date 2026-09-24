# Campaign Reach Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/campaign-reach-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Aggregate and analyze unique audience reach across marketing campaigns.

## Description
This MCP server provides tools to manage and analyze marketing impact through unique audience metrics. Use `get_campaign_reach` to find the size of a specific campaign, `aggregate_total_reach` to calculate the combined unique audience of multiple campaigns, `calculate_audience_overlap` to identify audience redundancy, and `analyze_saturation_risk` to determine if a target market is reaching its limit.


## Available Tools (4)
- **get_campaign_reach**: 
- **aggregate_total_reach**: 
- **analyze_saturation_risk**: 
- **calculate_audience_overlap**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Campaign Reach Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total unique reach for campaigns C1, C2, and C3?"

**🤖 AI Agent:**
> The total unique reach for campaigns C1, C2, and C3 is 150,000 individuals.

---

**👤 You:**
> "Is the target market of 500,000 people saturated with campaigns C1 and C2?"

**🤖 AI Agent:**
> The current saturation level is 80%, which indicates a High risk of reaching saturation for this target market.

---

**👤 You:**
> "How much overlap is there between campaign Alpha and campaign Beta?"

**🤖 AI Agent:**
> There is an overlap of 5,000 individuals between campaign Alpha and campaign Beta, representing a 5% overlap.


## ❓ FAQ

**Q: How is total reach calculated?**
The `aggregate_total_reach` tool calculates reach by finding the union of all unique individuals across the specified campaigns to prevent double-counting.

**Q: Can I check if my audience is saturated?**
Yes, you can use `analyze_saturation_risk` to compare your current combined reach against the total addressable market size.

**Q: How do I find the overlap between two campaigns?**
Use the `calculate_audience_overlap` tool to determine the number of individuals common to both campaigns and the resulting overlap percentage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/campaign-reach-analyzer](https://vinkius.com/en/ai-agent-connect/campaign-reach-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Campaign Reach Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `campaign-reach-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Campaign Reach Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "campaign-reach-analyzer": {
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
