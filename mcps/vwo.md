# VWO MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vwo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage A/B tests, feature flags, and conversion goals on VWO — the leading experience optimization platform.

## Description
Connect your **VWO (Visual Website Optimizer)** account to any AI agent and take control of your experimentation and feature rollout workflows through natural conversation.

### What you can do

- **Optimization Campaigns** — List and monitor active A/B tests and personalization campaigns directly from your agent
- **Feature Management** — List all feature flags and toggle their status across different environments for instant rollouts
- **Experiment Results** — Retrieve statistical results for any campaign, including performance metrics and significance levels
- **Conversion Tracking** — Browse conversion goals and KPIs being tracked to understand your optimization impact
- **Audience Segmentation** — List pre-defined segments to see how you are targeting different user groups
- **Environment Control** — Manage features across staging, production, and other configured VWO environments

### How it works

1. Subscribe to this server
2. Enter your VWO API Token and Account ID
3. Start managing your experiments and feature flags through Claude, Cursor, or any MCP-compatible client

No more jumping between experiment dashboards to check test results. Your AI agent becomes your optimization engine.

### Who is this for?

- **Growth Managers** — monitor experiment results and statistical significance without manual data exports
- **Product Managers** — manage feature rollouts and toggle flags across environments during launches
- **Data Analysts** — quickly surface conversion goal metrics and audience segment performance
- **CRO Specialists** — audit active campaigns and identify optimization opportunities through simple chat commands


## Available Tools
- **get_vwo_account_info**: Retrieves details about the authenticated VWO account
- **get_campaign_details**: Retrieves details for a specific VWO campaign
- **get_feature_flag_details**: Retrieves configuration for a specific VWO feature flag
- **get_campaign_results**: Retrieves statistical results for a VWO campaign
- **list_optimization_campaigns**: Lists all VWO A/B test and personalization campaigns
- **list_vwo_environments**: g. Production, Staging) for feature flag management.

Lists all configured VWO environments
- **list_feature_flags**: Lists all VWO feature flags
- **list_conversion_goals**: g. clicks, revenue) are being tracked.

Lists all conversion goals and metrics
- **list_audience_segments**: Lists all audience segments
- **toggle_feature_flag**: Provide the feature ID and the desired enabled status (true/false).

Enables or disables a VWO feature flag


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VWO** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active A/B testing campaigns."

**🤖 AI Agent:**
> I found 4 active campaigns: 'Homepage Redesign' (ID: camp-101), 'Checkout Flow Optimization' (ID: camp-102), 'Pricing Page Test' (ID: camp-103), and 'Newsletter Signup Personalization' (ID: camp-104). Which one would you like to review?

---

**👤 You:**
> "What are the results for the 'Checkout Flow Optimization' campaign?"

**🤖 AI Agent:**
> Results for camp-102: Variation B is the winner with 98% statistical significance. It shows a 14.5% improvement in conversion rate compared to the control. Variation A showed no significant change. Would you like me to pull more detailed metrics?

---

**👤 You:**
> "Disable the feature flag for 'new_payment_gateway'."

**🤖 AI Agent:**
> I've disabled the feature flag 'new_payment_gateway' (ID: feat-555) as requested. The status has been updated successfully across all environments. Is there anything else you need me to adjust?


## ❓ FAQ

**Q: Can I check the winning variation of an A/B test through the agent?**
Yes. The `get_campaign_results` tool allows your AI agent to pull detailed performance metrics for any experiment, showing improvement percentages and statistical significance for each variation compared to the control.

**Q: Is it possible to enable or disable feature flags via chat?**
Absolutely. Using the `toggle_feature_flag` tool, you can instruct your agent to enable or disable any feature flag for a specific rollout or emergency kill-switch scenario, ensuring fast control without opening the VWO dashboard.

**Q: How can I see what conversion goals are being tracked for my campaigns?**
You can use the `list_conversion_goals` tool to retrieve all metrics and KPIs (like clicks, form submissions, or revenue) currently being monitored in your VWO account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vwo](https://vinkius.com/mcp/vwo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **VWO** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `vwo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **VWO** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vwo": {
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
