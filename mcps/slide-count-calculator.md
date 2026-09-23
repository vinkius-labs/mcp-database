# Slide Count Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/slide-count-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate presentation slide counts and schedules based on duration and pacing.

## Description
Plan your presentations with precision using the Slide Count Calculator. This tool helps presenters and organizers determine exactly how many slides will fit into a given time slot based on their preferred pacing. You can use `get_estimated_slide_count` to find the total number of slides, `get_pacing_options` to discover recommended speeds like Rapid or Deep Dive, `get_presentation_schedule` to generate a timestamped timeline for every slide, and `validate_presentation_constraints` to ensure your planned slide count is realistic for your allotted time.


## Available Tools (4)
- **get_estimated_slide_count**: Determines the number of slides needed for a specific presentation time and pace
- **get_pacing_options**: Provides a set of standard pacing recommendations based on different presentation styles
- **get_presentation_schedule**: Generates a timeline of when each slide should occur during the presentation
- **validate_presentation_constraints**: Checks if a specific set of presentation parameters is realistic or violates time limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Slide Count Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many slides can I fit in a 30-minute presentation if I spend 2 minutes per slide?"

**🤖 AI Agent:**
> You can fit 15 slides in a 30-minute presentation with a 2-minute pacing rate.

---

**👤 You:**
> "I have 45 minutes. What are the standard pacing options?"

**🤖 AI Agent:**
> The standard pacing options are Rapid, Standard, and Deep Dive.

---

**👤 You:**
> "Will 20 slides fit in a 15-minute presentation if I spend 1 minute per slide?"

**🤖 AI Agent:**
> No, 20 slides at 1 minute per slide would require 20 minutes, which exceeds your 15-minute limit.


## ❓ FAQ

**Q: How do I know how many slides I need?**
You can use the `get_estimated_slide_count` tool by providing your total presentation time and your desired minutes per slide.

**Q: Can I include buffer time in my calculation?**
Yes, all calculation tools allow you to specify `bufferMinutes` to reserve time for transitions or technical issues.

**Q: What are the different pacing styles available?**
You can use `get_pacing_options` to see standard recommendations such as Rapid, Standard, and Deep Dive.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/slide-count-calculator](https://vinkius.com/en/ai-agent-connect/slide-count-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Slide Count Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `slide-count-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Slide Count Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "slide-count-calculator": {
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
