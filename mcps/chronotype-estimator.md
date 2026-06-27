# Chronotype Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chronotype-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Classifies biological chronotypes and recommends productivity windows based on natural sleep patterns.

## Description
The Chronotype Estimator helps you align your daily schedule with your biological rhythm. By using tools like `estimate_chronotype`, you can identify if you are a Lion, Bear, Wolf, or Dolphin. Once identified, use `get_schedule_recommendations` to find your peak focus windows and `evaluate_sleep_debt` to understand how sleep deprivation impacts your productivity.


## Available Tools (3)
- **estimate_chronotype**: Estimate user chronotype
- **evaluate_sleep_debt**: Evaluate sleep debt impact
- **get_schedule_recommendations**: Get schedule recommendations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chronotype Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I usually wake up at 06:00 and go to bed at 22:00. What is my chronotype?"

**🤖 AI Agent:**
> Based on your early wake time and bedtime, you are likely a Lion.

---

**👤 You:**
> "I am a Wolf. When should I schedule my most important tasks?"

**🤖 AI Agent:**
> As a Wolf, your peak focus windows are typically in the late evening.

---

**👤 You:**
> "How much will 5 hours of sleep affect my productivity if I am a Bear?"

**🤖 AI Agent:**
> With only 5 hours of sleep against your target, you will likely experience a significant impact on your alertness during peak windows.


## ❓ FAQ

**Q: What is a chronotype?**
A chronotype is your body's natural inclination to sleep and wake at certain times, driven by your internal circadian rhythm.

**Q: How can I find my chronotype?**
You can use the `estimate_chronotype` tool by providing your typical wake and bedtime to see which category you fall into.

**Q: Can this tool help me improve my productivity?**
Yes, by using `get_schedule_recommendations`, you can identify the best times for deep work and rest based on your specific biological type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chronotype-estimator](https://vinkius.com/mcp/chronotype-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chronotype Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chronotype-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chronotype Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chronotype-estimator": {
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
