# Postpartum Recovery Timeline MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/postpartum-recovery-timeline)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Estimates postpartum recovery milestones, activity progression, and energy levels.

## Description
This MCP server provides physiological recovery estimates for new mothers. It uses specialized tools like `get_recovery_timeline` to map expected milestones, `get_activity_progression` to recommend safe movement, `get_energy_level_estimate` to predict fatigue, and `get_red_flag_warnings` to identify critical symptoms. The estimates account for delivery type (vaginal or cesarean), medical complications, and breastfeeding status to provide personalized recovery guidance.


## Available Tools (4)
- **get_red_flag_warnings**: Identifies critical symptoms that require immediate medical attention
- **get_activity_progression**: Recommends a safe, gradual increase in physical activity levels
- **get_energy_level_estimate**: Predicts energy fluctuations to help the user manage expectations regarding fatigue
- **get_recovery_timeline**: Provides a high-level overview of when major recovery milestones are expected to occur


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Postpartum Recovery Timeline** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I had a cesarean delivery and I am currently in week 2. What should my activity level be?"

**🤖 AI Agent:**
> At week 2 following a cesarean delivery, your recommended activity level is Light Walking. You should focus on gentle movement to aid circulation while avoiding any core-based or abdominal exercises.

---

**👤 You:**
> "What are the expected recovery milestones for a vaginal delivery without complications?"

**🤖 AI Agent:**
> For a vaginal delivery without complications, major milestones include the initial healing phase in weeks 1-2, the return of energy levels around week 6, and a gradual return to full physical capacity by week 12.

---

**👤 You:**
> "I am breastfeeding and feeling very tired at week 4. What is happening?"

**🤖 AI Agent:**
> At week 4, your energy levels are likely fluctuating. The combination of postpartum physiological shifts and the high energy demands of breastfeeding is a primary factor in your current fatigue.


## ❓ FAQ

**Q: How does delivery type affect the recovery estimate?**
The tool uses `get_recovery_timeline` to adjust milestones based on whether the delivery was vaginal or cesarean, as abdominal surgery requires a different healing trajectory.

**Q: Can I use this to check for medical emergencies?**
You can use `get_red_flag_warnings` to identify symptoms that require immediate medical attention, but this tool is for informational guidance and not a substitute for professional medical diagnosis.

**Q: Does breastfeeding change the energy predictions?**
Yes, `get_energy_level_estimate` accounts for the increased caloric and energy demands associated with breastfeeding.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/postpartum-recovery-timeline](https://vinkius.com/en/ai-agent-connect/postpartum-recovery-timeline)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Postpartum Recovery Timeline** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `postpartum-recovery-timeline` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Postpartum Recovery Timeline** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "postpartum-recovery-timeline": {
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
