# Shoulder Impingement Risk Assessment for Surfers MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shoulder-impingement-risk-assessment-for-surfers)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Assess shoulder impingement risk and get personalized prevention exercises for surfers.

## Description
This MCP server provides specialized tools for surfers to evaluate their risk of shoulder impingement. By analyzing paddling volume, posture scores, and strength imbalances between internal and external rotators, the server identifies specific physical drivers of injury risk. Users can utilize `get_risk_assessment` to determine their risk level, `get_contributing_factors` to pinpoint specific weaknesses, and `get_prevention_protocol` to receive a customized set of mobility, stability, and strength exercises. It also provides `get_volume_guidelines` to help manage paddling hours safely based on current physical status.


## Available Tools (4)
- **get_contributing_factors**: Provides a detailed breakdown of physical metrics responsible for the risk
- **get_prevention_protocol**: Generates targeted exercises to mitigate impingement risk
- **get_risk_assessment**: Calculates the overall impingement risk level and identifies primary drivers
- **get_volume_guidelines**: Provides recommended paddling limits to manage risk


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shoulder Impingement Risk Assessment for Surfers** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I paddle 10 hours a week, my posture score is 7, and my strength imbalance ratio is 1.5. What is my risk?"

**🤖 AI Agent:**
> Your risk level is High. The primary driver is your strength imbalance ratio of 1.5, which indicates overactive internal rotators.

---

**👤 You:**
> "What exercises should I do if I have a high posture score and limited overhead mobility?"

**🤖 AI Agent:**
> You should focus on thoracic spine mobility and scapular stability exercises, such as thoracic extensions and wall slides.

---

**👤 You:**
> "My risk level is Moderate and my posture score is 4. How many hours should I paddle?"

**🤖 AI Agent:**
> Based on a Moderate risk level and a posture score of 4, your recommended maximum paddling volume is 8 hours per week.


## ❓ FAQ

**Q: How do I determine my shoulder impingement risk?**
You can use the `get_risk_assessment` tool by providing your weekly paddling hours, a posture score from 1 to 10, and your internal to external rotator strength ratio.

**Q: Can I get specific exercises to prevent injury?**
Yes, the `get_prevention_protocol` tool generates a customized list of mobility, stability, and strength exercises tailored to your specific posture and strength profile.

**Q: How much should I paddle each week?**
The `get_volume_guidelines` tool provides recommended maximum paddling hours based on your current risk level and posture score.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shoulder-impingement-risk-assessment-for-surfers](https://vinkius.com/en/ai-agent-connect/shoulder-impingement-risk-assessment-for-surfers)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shoulder Impingement Risk Assessment for Surfers** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shoulder-impingement-risk-assessment-for-surfers` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shoulder Impingement Risk Assessment for Surfers** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shoulder-impingement-risk-assessment-for-surfers": {
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
