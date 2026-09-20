# Sleep Hygiene Score MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sleep-hygiene-score)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Assess your sleep quality through scientific hygiene scoring.

## Description
This MCP server provides a scientific approach to evaluating sleep quality using the Sleep Hygiene Index methodology. It connects AI agents to specialized tools that analyze sleep environments, behavioral habits, and substance impacts. Users can use `calculate_sleep_hygiene_score` to receive a complete profile including total scores and prioritized wellness recommendations. For deeper insights, the server offers `evaluate_environment_quality` to analyze physical surroundings and `get_substance_impact_profile` to understand how caffeine, alcohol, or nicotine affect sleep maintenance. It is compatible with Cursor, VS Code, Claude Desktop, Windsurf, and any MCP-compatible client via Vinkius Edge.


## Available Tools (4)
- **get_substance_impact_profile**: Analyzes how timing and quantity of substances affect sleep maintenance
- **evaluate_environment_quality**: Provides a deep-dive analysis of the physical sleep setting
- **calculate_sleep_hygiene_score**: Computes the complete sleep hygiene profile including total score, category breakdowns, and advice
- **get_hygiene_item_definitions**: Retrieves the descriptive text and domain classification for every item in the hygiene questionnaire


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sleep Hygiene Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my sleep hygiene score based on these responses: {"light_level": "suboptimal", "caffeine_intake": "poor", "bedtime_consistency": "optimal"}"

**🤖 AI Agent:**
> Your total sleep hygiene score is 65 (Fair). Your habits are excellent, but your caffeine intake and light levels are suboptimal. We recommend reducing caffeine consumption in the afternoon and ensuring your room is dark for better sleep.

---

**👤 You:**
> "Analyze my sleep environment: {"noise_level": "high", "temperature": "optimal", "light_level": "optimal"}"

**🤖 AI Agent:**
> Your environment score is 40. The primary disruptor is high noise levels. We recommend using white noise or earplugs to mitigate this interference.

---

**👤 You:**
> "What is the impact of my alcohol consumption on sleep?"

**🤖 AI Agent:**
> Your substance impact level is High. It is estimated that you need a 4-hour recovery window after your last drink to return to baseline sleep quality.


## ❓ FAQ

**Q: How is the sleep score calculated?**
The score is calculated using the Sleep Hygiene Index methodology, which evaluates environmental factors, behavioral habits, and substance use through `calculate_sleep_hygiene_score`.

**Q: Can I analyze my bedroom environment specifically?**
Yes, you can use the `evaluate_environment_quality` tool to get a deep-dive analysis of light, noise, temperature, and comfort levels.

**Q: How does caffeine affect my score?**
The `get_substance_impact_profile` tool analyzes how the timing and quantity of caffeine consumption impact your sleep maintenance and recovery window.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sleep-hygiene-score](https://vinkius.com/en/ai-agent-connect/sleep-hygiene-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sleep Hygiene Score** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sleep-hygiene-score` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sleep Hygiene Score** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sleep-hygiene-score": {
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
