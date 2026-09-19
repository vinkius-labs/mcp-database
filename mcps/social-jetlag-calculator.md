# Social Jetlag Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/social-jetlag-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze circadian misalignment and sleep patterns.

## Description
This MCP server provides tools to quantify social jetlag, the physiological discrepancy between biological rhythms and social obligations. Use `get_social_jetlag_metrics` to calculate jetlag hours and misalignment scores, `get_health_risk_assessment` to understand potential physiological impacts, `get_adjustment_strategies` for lifestyle interventions, and `get_circadian_alignment_profile` to determine your phase shift type.


## Available Tools (4)
- **get_adjustment_strategies**: Recommends specific lifestyle interventions to reduce circadian misalignment
- **get_circadian_alignment_profile**: Answers how well a user's current social life aligns with a theoretical biological rhythm
- **get_health_risk_assessment**: Provides a detailed qualitative description of the health risks associated with a specific jetlag value
- **get_social_jetlag_metrics**: Calculates the primary quantitative measures of social jetlag for a user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Social Jetlag Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my social jetlag metrics. I sleep at 07:00 on weekdays and 10:00 on weekends, and I have low schedule flexibility."

**🤖 AI Agent:**
> Your jetlag is 3.0 hours with a high misalignment score. This indicates a significant physiological strain due to your rigid schedule.

---

**👤 You:**
> "What are the health risks for 4 hours of social jetlag?"

**🤖 AI Agent:**
> A 4-hour jetlag level falls into the elevated risk category, which may lead to metabolic and sleep-related stressors.

---

**👤 You:**
> "How can I adjust my sleep if I have 2 hours of jetlag and high flexibility?"

**🤖 AI Agent:**
> The primary strategy is light exposure management. You can also try consistent wake times and gradual sleep shifts.


## ❓ FAQ

**Q: What is social jetlag?**
Social jetlag is the difference between your biological clock and your social schedule, such as the shift between weekday and weekend sleep times.

**Q: How can I reduce my misalignment?**
You can use `get_adjustment_strategies` to receive specific recommendations like light exposure management based on your jetlag hours.

**Q: Can I assess my health risks?**
Yes, by using `get_health_risk_assessment`, you can get a qualitative description of the risks associated with your specific jetlag value.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/social-jetlag-calculator](https://vinkius.com/en/ai-agent-connect/social-jetlag-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Social Jetlag Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `social-jetlag-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Social Jetlag Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "social-jetlag-calculator": {
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
