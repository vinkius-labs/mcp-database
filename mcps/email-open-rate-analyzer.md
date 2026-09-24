# Email Open Rate Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/email-open-rate-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Calculate and analyze email campaign engagement via open rates and performance tiers.

## Description
This MCP server provides a suite of tools to measure email marketing success. You can use `calculate_open_rate` to find the percentage of opened emails, `get_engagement_tier` to categorize performance, `analyze_campaign_performance` for a full diagnostic summary, and `get_volume_adjusted_benchmark` to find target rates based on delivery volume.


## Available Tools (4)
- **analyze_campaign_performance**: Provides a comprehensive summary of a campaign by combining raw counts and calculated rates
- **calculate_open_rate**: Determines the percentage of emails opened relative to the number of emails successfully delivered
- **get_engagement_tier**: Categorizes a specific open rate into a qualitative performance tier
- **get_volume_adjusted_benchmark**: Returns an expected "good" open rate threshold that accounts for the size of the email list


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Email Open Rate Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the open rate for my 'Summer Sale' campaign with 500 opens and 2500 deliveries?"

**🤖 AI Agent:**
> The open rate for the 'Summer Sale' campaign is 20%.

---

**👤 You:**
> "Is an open rate of 35% considered good?"

**🤖 AI Agent:**
> Yes, a 35% open rate is categorized as High engagement.

---

**👤 You:**
> "What is the target open rate for a campaign that delivered 10,000 emails?"

**🤖 AI Agent:**
> For a volume of 10,000 deliveries, the target open rate is 15%.


## ❓ FAQ

**Q: How do I calculate my campaign's open rate?**
You can use the `calculate_open_rate` tool by providing the total number of opens and the total number of delivered emails.

**Q: What determines an engagement tier?**
The `get_engagement_tier` tool compares your open rate against industry benchmarks to classify it as High, Average, or Low.

**Q: Can I get a full report for a specific campaign?**
Yes, use `analyze_campaign_performance` with the campaign name, total opens, and delivered count to get a complete diagnostic view.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/email-open-rate-analyzer](https://vinkius.com/en/ai-agent-connect/email-open-rate-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Email Open Rate Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `email-open-rate-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Email Open Rate Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "email-open-rate-analyzer": {
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
