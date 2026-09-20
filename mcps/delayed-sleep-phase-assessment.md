# Delayed Sleep Phase Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/delayed-sleep-phase-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Assess circadian misalignment and get chronotherapy guidance.

## Description
This MCP server provides clinical assessment tools for Delayed Sleep Phase Syndrome (DSPS). It allows AI agents to evaluate circadian misalignment using `analyze_dsps_status`, recommend optimal light therapy windows via `calculate_chronotherapy_window`, provide lifestyle suggestions with `get_severity_guidance`, and quantify social constraints through `evaluate_social_misalignment`.


## Available Tools (4)
- **analyze_dsps_status**: Evaluates the user's sleep data to determine if they meet clinical indicators for DSPS and calculates the severity
- **calculate_chronotherapy_window**: Recommends the optimal time for light therapy to help advance the sleep phase
- **evaluate_social_misalignment**: Quantifies the impact of social constraints on the user's biological rhythm
- **get_severity_guidance**: g., Mild, Moderate, Severe).

Provides behavioral and lifestyle suggestions based on the calculated severity of the phase delay


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Delayed Sleep Phase Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I naturally fall asleep at 03:00 but need to be in bed by 23:00. My wake difficulty is 8. What is my status?"

**🤖 AI Agent:**
> Your phase delay is 4 hours, and your DSPS status is classified as Severe due to the high wake difficulty.

---

**👤 You:**
> "I fall asleep at 02:00 and want to start falling asleep at 23:00. When should I use light therapy?"

**🤖 AI Agent:**
> The recommended light exposure window is between 06:00 and 08:00 to effectively advance your circadian rhythm.

---

**👤 You:**
> "I naturally wake up at 10:00 but have to wake up at 07:00 for work. How much misalignment is this?"

**🤖 AI Agent:**
> You have a 3-hour social misalignment, which creates a significant circadian conflict.


## ❓ FAQ

**Q: How does this tool help with sleep issues?**
It uses `analyze_dsps_status` to determine if your sleep patterns match DSPS criteria and provides specific chronotherapy timing.

**Q: Can I get light therapy recommendations?**
Yes, the `calculate_chronotherapy_window` tool identifies the best time for light exposure to advance your biological clock.

**Q: What is social misalignment?**
It is the conflict between your natural wake time and the time you must wake up for work or school, which can be measured using `evaluate_social_misalignment`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/delayed-sleep-phase-assessment](https://vinkius.com/en/ai-agent-connect/delayed-sleep-phase-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Delayed Sleep Phase Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `delayed-sleep-phase-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Delayed Sleep Phase Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "delayed-sleep-phase-assessment": {
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
