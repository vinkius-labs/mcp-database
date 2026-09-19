# Digital Detox Duration Recommender MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/digital-detox-duration-recommender)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Personalized digital detox roadmaps and wellness strategies.

## Description
This MCP server provides a clinical-style wellness engine to help users manage digital dependency. It uses tools like `recommend_detox_plan` to generate personalized detox durations and tiers, `get_activity_suggestions` to find non-digital replacements, `evaluate_dependency_level` to assess digital health, and `calculate_reintegration_protocol` to establish post-detox boundaries. It is designed to help users recalibrate dopamine sensitivity and regain mental focus.


## Available Tools (4)
- **calculate_reintegration_protocol**: Determines rules for returning to digital life
- **evaluate_dependency_level**: Assesses current digital health status and dependency score
- **get_activity_suggestions**: Suggests non-digital activities to replace device usage
- **recommend_detox_plan**: Provides a personalized digital detox roadmap


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Digital Detox Duration Recommender** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I spend 8 hours a day on my phone, use social media heavily, and feel anxious when I don't have it. Can you recommend a detox plan?"

**🤖 AI Agent:**
> Based on your high dependency, I recommend a Deep Reset detox lasting 7 days. You should prepare by notifying your close contacts and setting up a dedicated physical space for your phone. During the detox, try activities like sketching or walking to fill your time.

---

**👤 You:**
> "I have 30 minutes and low energy. What is a good non-digital activity for me?"

**🤖 AI Agent:**
> Since you have low energy and 30 minutes, I suggest practicing a brief meditation or some light breathing exercises.

---

**👤 You:**
> "How dependent am I on my devices? I use them for 10 hours a day and feel phantom vibrations."

**🤖 AI Agent:**
> Your dependency score is high, placing you in the critical health risk level due to your high screen time and physical symptoms.


## ❓ FAQ

**Q: How does the detox duration get calculated?**
The duration is determined by combining your screen time, social media intensity, and specific addiction indicators using the `recommend_detox_plan` tool.

**Q: Can I get suggestions for things to do instead of using my phone?**
Yes, you can use `get_activity_suggestions` to find physical, creative, or relaxing activities that match your available time and energy level.

**Q: What happens after my detox is finished?**
The `calculate_reintegration_protocol` tool provides specific rules and a transition phase to help you return to digital life without immediate relapse.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/digital-detox-duration-recommender](https://vinkius.com/en/ai-agent-connect/digital-detox-duration-recommender)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Digital Detox Duration Recommender** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `digital-detox-duration-recommender` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Digital Detox Duration Recommender** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "digital-detox-duration-recommender": {
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
