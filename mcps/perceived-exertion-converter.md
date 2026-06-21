# Perceived Exertion Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/perceived-exertion-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Convert RPE (Borg 6-20 and CR10) to estimated heart rate and training zones.

## Description
The Perceived Exertion Converter bridges the gap between subjective effort and objective physiological metrics. Using the `convert_borg_6_20_scale` and `convert_cr10_scale` tools, athletes can translate their Rate of Perceived Exertion (RPE) into estimated heart rate, percentage of maximum capacity, and specific training zones like Aerobic or Threshold. This is ideal for training without a continuous heart rate monitor. Additionally, use `get_training_guidance` to receive qualitative intensity descriptions and practical coaching advice based on your effort level.


## Available Tools
- **convert_cr10_scale**: Converts CR10 scale RPE to physiological metrics
- **get_training_guidance**: Provides qualitative training descriptions and practical advice
- **convert_borg_6_20_scale**: Converts Borg 6-20 scale RPE to physiological metrics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Perceived Exertion Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I feel like I'm at an RPE of 14 on the Borg scale and my max HR is 190. What is my estimated heart rate?"

**🤖 AI Agent:**
> Based on a Borg 6-20 RPE of 14 and a max HR of 190, your estimated heart rate is approximately 153 BPM, which places you in the Aerobic training zone.

---

**👤 You:**
> "Convert an RPE of 7 on the CR10 scale with a max HR of 185."

**🤖 AI Agent:**
> For a CR10 RPE of 7 and a max HR of 185, your estimated heart rate is approximately 148 BPM (70% of max), placing you in the Threshold training zone.

---

**👤 You:**
> "What kind of training should I do at an RPE of 18 on the Borg scale?"

**🤖 AI Agent:**
> An RPE of 18 represents a very high intensity, typically corresponding to the Anaerobic/Maximal zone. This effort is characterized by intense muscular effort and is usually sustainable only for short durations.


## ❓ FAQ

**Q: What is the Borg 6-20 scale?**
The Borg 6-20 scale is a traditional method for measuring perceived physical exertion, where 6 represents no effort and 20 represents maximal intensity.

**Q: How accurate are the heart rate estimates?**
The tool provides estimates based on the relative position of your RPE within the scale range applied to your maximum heart rate. It is a mathematical approximation for training guidance.

**Q: Can I use this without a heart rate monitor?**
Yes, the primary purpose of these tools is to help you estimate intensity and training zones using only your subjective perception of effort.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/perceived-exertion-converter](https://vinkius.com/mcp/perceived-exertion-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Perceived Exertion Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `perceived-exertion-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Perceived Exertion Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "perceived-exertion-converter": {
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
