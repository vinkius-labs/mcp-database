# Sleep Satisfaction Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sleep-satisfaction-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantifies subjective sleep quality by analyzing questionnaire responses and expectation gaps.

## Description
This MCP server provides a specialized engine to quantify how well a user slept. By analyzing qualitative questionnaire ratings for quality, depth, and continuity, it calculates a holistic satisfaction score. It also identifies the primary drivers and inhibitors of sleep quality, quantifies the psychological impact of missing sleep goals via the expectation gap, and provides actionable improvement areas to help users close the gap between their actual sleep and their target duration. Use `calculate_satisfaction_score` to get the primary score, `identify_influencing_factors` to find what helped or hindered sleep, `analyze_expectation_gap` to understand the impact of missed goals, and `suggest_improvement_areas` for actionable advice.


## Available Tools (4)
- **analyze_expectation_gap**: Quantifies the psychological impact of missing sleep goals
- **calculate_satisfaction_score**: Provides the primary holistic score for a single sleep session
- **identify_influencing_factors**: Determines which specific aspects of sleep contributed most to the overall feeling
- **suggest_improvement_areas**: Provides actionable categories for the user to improve their sleep quality


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sleep Satisfaction Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my sleep satisfaction score. I rated quality as 8, depth as 7, and continuity as 9. I expected 8 hours but slept 7 hours."

**🤖 AI Agent:**
> Your satisfaction score is 7.5. You had a 1-hour expectation gap, which slightly lowered your score despite high continuity.

---

**👤 You:**
> "What were the main factors affecting my sleep? My ratings were quality: 4, depth: 5, continuity: 8, and my satisfaction score was 5."

**🤖 AI Agent:**
> The primary inhibitors for your sleep were low quality and depth ratings, while high continuity was a positive driver.

---

**👤 You:**
> "I slept 6 hours but wanted 8. My quality was 7, depth 6, and continuity 7. How much did missing my goal impact me?"

**🤖 AI Agent:**
> The 2-hour expectation gap resulted in a moderate psychological impact, reducing your perceived satisfaction significantly.


## ❓ FAQ

**Q: How is the satisfaction score calculated?**
The score is a weighted synthesis of your qualitative ratings for sleep quality, depth, and continuity, combined with how closely your actual sleep duration matched your expected duration.

**Q: What is the expectation gap?**
The expectation gap is the difference between your target sleep duration and your actual sleep duration. This tool uses `analyze_expectation_gap` to determine how this difference impacts your overall satisfaction.

**Q: Can I get advice on how to sleep better?**
Yes, you can use `suggest_improvement_areas` to receive specific, actionable categories for improvement based on your sleep data and expectation gap.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sleep-satisfaction-scorer](https://vinkius.com/en/ai-agent-connect/sleep-satisfaction-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sleep Satisfaction Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sleep-satisfaction-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sleep Satisfaction Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sleep-satisfaction-scorer": {
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
