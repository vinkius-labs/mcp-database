# Eye Strain Index MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/eye-strain-index)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Assess ocular health and screen-related fatigue risk.

## Description
This MCP server provides tools to monitor and mitigate digital eye strain. Use `get_strain_assessment` to calculate your current fatigue score and risk level based on screen time, distance, and lighting. You can also use `get_compliance_score` to track adherence to the 20-20-20 rule, `get_break_recommendation` for personalized rest schedules, and `get_ergonomic_advice` for environmental adjustments to reduce ocular load.


## Available Tools (4)
- **get_break_recommendation**: Provides a personalized rest schedule to mitigate calculated strain
- **get_compliance_score**: Evaluates how well the user is following the 20-20-20 rule
- **get_ergonomic_advice**: Provides environmental adjustments to reduce ocular load
- **get_strain_assessment**: Calculates the immediate eye strain risk based on current user behavior and environment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eye Strain Index** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I've been working for 4 hours, I've taken 2 breaks, I'm 50cm from the screen, the light is 300 lux, and blue light is 0.5. How is my eye strain?"

**🤖 AI Agent:**
> Your Eye Strain Index is 65, which falls into the High risk category. You should take a break immediately.

---

**👤 You:**
> "I've been on screen for 60 minutes and I've followed the 20-20-20 rule 3 times. What is my compliance?"

**🤖 AI Agent:**
> Your compliance score is 100%, which means you are fully compliant with the 20-20-20 rule.

---

**👤 You:**
> "My eye strain index is 40 and I've been working for 3 hours. What should my break schedule look like?"

**🤖 AI Agent:**
> You should take a break every 30 minutes for a duration of 120 seconds. Your next break is scheduled shortly.


## ❓ FAQ

**Q: How do I calculate my eye strain risk?**
You can use the `get_strain_assessment` tool by providing your screen hours, break frequency, distance from the screen, and ambient lighting levels.

**Q: What is the 20-20-20 rule?**
The 20-20-20 rule suggests that every 20 minutes, you should look at something 20 feet away for 20 seconds to reduce eye strain.

**Q: Can this tool help with my workspace setup?**
Yes, the `get_ergonomic_advice` tool provides specific guidance on screen distance, ambient lighting, and blue light exposure to optimize your environment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/eye-strain-index](https://vinkius.com/en/ai-agent-connect/eye-strain-index)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Eye Strain Index** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `eye-strain-index` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Eye Strain Index** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eye-strain-index": {
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
