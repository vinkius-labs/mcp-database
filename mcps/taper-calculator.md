# Taper Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/taper-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Generate optimal tapering schedules to maximize athletic performance.

## Description
Taper Calculator provides data-driven tapering strategies to help athletes reach peak performance. By analyzing training load, sport type, and event importance, the server generates precise tapering schedules. Use `get_taper_plan` to determine the ideal duration and volume reduction, `get_volume_breakdown` for a granular daily schedule, `get_intensity_profile` to maintain sharpness, and `analyze_performance_readiness` to assess the risk and likelihood of peaking for your competition.


## Available Tools (4)
- **analyze_performance_readiness**: Predicts the expected performance outcome and identifies potential risks based on the planned taper
- **get_intensity_profile**: Defines how the athlete should maintain or adjust intensity to ensure they are sharp for the event
- **get_taper_plan**: Generates a comprehensive tapering schedule including duration, volume, and intensity guidelines
- **get_volume_breakdown**: Provides a detailed, granular schedule of volume percentages for a specific taper duration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Taper Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am an endurance athlete with a training load of 80. My race is on 2025-06-15 and it is a high importance event. Can you create a taper plan?"

**🤖 AI Agent:**
> Your optimal taper will last 14 days. You should follow a volume reduction starting at 80% and tapering down to 40% in the final days, while maintaining high intensity to stay sharp for your race on June 15th.

---

**👤 You:**
> "What should my intensity look like for a power-based sport with high event importance?"

**🤖 AI Agent:**
> For power sports, you should target an intensity zone of 85-95% of maximum effort to maintain neuromuscular recruitment.

---

**👤 You:**
> "Will a 7-day taper be enough for my current training load of 90 in an endurance sport?"

**🤖 AI Agent:**
> A 7-day taper for a training load of 90 in an endurance sport carries a high risk of insufficient fatigue dissipation. It is recommended to extend the taper duration to ensure peak readiness.


## ❓ FAQ

**Q: How do I know if my taper is effective?**
You can use `analyze_performance_readiness` to get a readiness score and identify potential risks in your planned taper.

**Q: Does the tool support different types of sports?**
Yes, the tool provides specific guidance for endurance, power, and hybrid sport types.

**Q: Can I get a day-by-day volume schedule?**
Yes, use the `get_volume_breakdown` tool to receive a detailed daily or phase-based volume percentage schedule.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/taper-calculator](https://vinkius.com/en/ai-agent-connect/taper-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Taper Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `taper-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Taper Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "taper-calculator": {
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
