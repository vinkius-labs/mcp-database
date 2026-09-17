# Wine Social Media ROI Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-social-media-roi-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Analyze social media marketing efficiency and ROI for wineries.

## Description
This MCP server provides specialized tools for wineries to evaluate their social media marketing performance. By connecting your AI agent to Vinkius Edge, you can use `analyze_platform_efficiency` to determine cost per engagement and visit, `calculate_conversion_metrics` to find acquisition costs, and `calculate_marketing_roi` to measure total financial return including brand awareness value. It also includes `get_attribution_summary` to identify which platforms act as brand assisters versus direct closers in the sales funnel.


## Available Tools (4)
- **calculate_conversion_metrics**: What is the direct cost of acquiring customers via social media?
- **calculate_marketing_roi**: What is the total financial return of my social media investment, including brand value?
- **get_attribution_summary**: Which platforms are acting as "assistants" versus "closers" in the sales funnel?
- **analyze_platform_efficiency**: How efficiently is each platform converting spend into engagement and traffic?


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Social Media ROI Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How efficient was our Instagram spend? We spent $500 and got 200 engagements and 50 clicks."

**🤖 AI Agent:**
> Your Instagram engagement cost is $2.50 per interaction and your cost per visit is $10.00.

---

**👤 You:**
> "What is the ROI for our Facebook campaign if we spent $1000, made $3000 in sales, and the brand value is $500?"

**🤖 AI Agent:**
> The total return for your Facebook campaign is $3500, resulting in an ROI of 250%.

---

**👤 You:**
> "Calculate the acquisition cost for Pinterest. We spent $200 and had 5 direct conversions and 10 assisted conversions."

**🤖 AI Agent:**
> The cost per acquisition for Pinterest is $40.00, with an assisted conversion rate of 66.67%.


## ❓ FAQ

**Q: How does this tool calculate ROI?**
The `calculate_marketing_roi` tool calculates ROI by summing direct revenue and the estimated brand awareness value, then comparing that total against the initial spend.

**Q: Can I see which platforms drive the most direct sales?**
Yes, you can use `get_attribution_summary` to identify the 'topCloser' platform, which is the one with the highest number of direct conversions.

**Q: What metrics can I track for a specific platform?**
Using `analyze_platform_efficiency`, you can track cost per engagement, cost per visit, and the engagement rate for any platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-social-media-roi-calculator](https://vinkius.com/en/ai-agent-connect/wine-social-media-roi-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Social Media ROI Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-social-media-roi-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Social Media ROI Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-social-media-roi-calculator": {
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
