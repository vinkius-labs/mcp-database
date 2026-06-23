# Social Media Engagement Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/social-media-engagement-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Calculate platform-specific engagement rates for Instagram and LinkedIn and compare them against industry benchmarks.

## Description
This MCP server provides specialized tools to quantify social media performance. Use `compute_instagram_engagement` to calculate engagement rates based on likes, comments, and saves relative to impressions. Use `compute_linkedin_engagement` to determine LinkedIn engagement using likes, comments, and shares. You can also use `retrieve_benchmark_standard` to find the target engagement rate for specific account tiers like Nano, Micro, Macro, or Mega.


## Available Tools (3)
- **retrieve_benchmark_standard**: Retrieves the target engagement benchmark for a specific account size tier
- **compute_instagram_engagement**: Determines the engagement rate for Instagram posts
- **compute_linkedin_engagement**: Determines the engagement rate for LinkedIn posts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Social Media Engagement Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my Instagram engagement rate for a post with 100 likes, 20 comments, 5 saves, and 1000 impressions."

**🤖 AI Agent:**
> The calculated Instagram engagement rate is 12.5%.

---

**👤 You:**
> "What is the benchmark for a Micro account?"

**🤖 AI Agent:**
> The target engagement rate for a Micro account tier is 3.5%.

---

**👤 You:**
> "Check LinkedIn engagement: 50 likes, 10 comments, 5 shares, and 500 impressions."

**🤖 AI Agent:**
> The calculated LinkedIn engagement rate is 13.0%.


## ❓ FAQ

**Q: How is Instagram engagement calculated?**
The `compute_instagram_lag` tool calculates the rate by summing likes, comments, and saves, then dividing that sum by the total number of impressions.

**Q: What is a benchmark standard?**
A benchmark standard is a target engagement rate based on your account size. You can use `retrieve_benchmark_standard` to find the appropriate target for Nano, Micro, Macro, or Mega tiers.

**Q: Does this tool support LinkedIn?**
Yes, the `compute_linkedin_engagement` tool calculates engagement rates for LinkedIn using likes, comments, and shares relative to impressions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/social-media-engagement-calculator](https://vinkius.com/mcp/social-media-engagement-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Social Media Engagement Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `social-media-engagement-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Social Media Engagement Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "social-media-engagement-calculator": {
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
