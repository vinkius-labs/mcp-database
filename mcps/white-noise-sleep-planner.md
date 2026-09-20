# White Noise Sleep Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/white-noise-sleep-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimizes white noise volume, duration, and sound type for better sleep.

## Description
This MCP server helps you plan your sleep environment using sound masking principles. It calculates the ideal volume and sound type to mask disturbances, creates duration schedules with fade-out plans, and provides weaning strategies to prevent sudden silence. You can use `get_masking_parameters` to find the best sound for your environment, `get_duration_schedule` for timing, `get_weaning_strategy` for volume reduction, and `get_device_optimization` to adjust settings for your specific hardware.


## Available Tools (4)
- **get_device_optimization**: Adjusts recommendations based on the technical limitations of the playback hardware
- **get_duration_schedule**: Calculates how long the noise should play and how it should fade
- **get_masking_parameters**: Determines the ideal volume and sound type to mask the current environment
- **get_weaning_strategy**: Provides a step-by-step plan for reducing volume to prevent sudden silence


## 💬 Prompt Examples

Here are some examples of how you can interact with the **White Noise Sleep Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I live in a noisy city and have high sensitivity to sound. What white noise settings should I use on my smartphone?"

**🤖 AI Agent:**
> For a noisy city environment and high sensitivity using a smartphone, you should use Brown noise at a volume of 55dB. Since smartphones have limited low-frequency response, it is recommended to increase the volume slightly to compensate.

---

**👤 You:**
> "Plan a 7-hour sleep schedule with a fade-out."

**🤖 AI Agent:**
> For a 420-minute sleep duration, the noise should play for the full duration, with the fade-out starting at minute 315 and lasting for 105 minutes.

---

**👤 You:**
> "How can I gradually reduce the volume of my white noise?"

**🤖 AI Agent:**
> To reduce volume from 60dB in 3 steps, you should follow this plan: Step 1: 45dB, Step 2: 30dB, Step 3: 15dB.


## ❓ FAQ

**Q: How do I know which sound type to use?**
You can use the `get_masking_parameters` tool. It analyzes your noise environment and sensitivity to recommend white, pink, or brown noise.

**Q: Can I optimize settings for my smartphone?**
Yes, the `get_device_optimization` tool provides specific adjustments for smartphones, dedicated machines, or speakers.

**Q: What is a weaning strategy?**
A weaning strategy, provided by `get_weaning_strategy`, is a gradual volume reduction plan that prevents sudden silence from waking you up.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/white-noise-sleep-planner](https://vinkius.com/en/ai-agent-connect/white-noise-sleep-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **White Noise Sleep Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `white-noise-sleep-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **White Noise Sleep Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "white-noise-sleep-planner": {
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
