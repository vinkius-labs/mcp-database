# Surf Back Pain Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-back-pain-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Identify causes of back pain in surfers by analyzing posture, flexibility, and surfing style.

## Description
This MCP server provides specialized diagnostic tools for surfers experiencing spinal discomfort. By utilizing `analyze_pain_origin` to distinguish between lumbar and thoracic issues, and `assess_risk_profile` to evaluate injury likelihood, it helps identify the physiological drivers of pain. The system uses `identify_likely_causes` to synthesize posture and flexibility data, and `get_corrective_recommendations` to provide specific mobility and postural advice tailored to the surfer's needs.


## Available Tools (4)
- **assess_risk_profile**: Evaluates the likelihood of injury based on flexibility and surfing style
- **analyze_pain_origin**: Determines if the user's reported pain is primarily located in the lumbar or thoracic region
- **get_corrective_recommendations**: Provides actionable mobility or postural advice
- **identify_likely_causes**: Pinpoints the most probable physiological cause of the pain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Back Pain Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have lower back pain and I usually paddle with a hyperextended posture. What is the likely cause?"

**🤖 AI Agent:**
> The primary cause is likely repetitive lumbar extension.

---

**👤 You:**
> "I am a shortboarder with low flexibility. What is my risk level?"

**🤖 AI Agent:**
> Your risk level is High.

---

**👤 You:**
> "My pain is in the lumbar region caused by repetitive extension. What should I do?"

**🤖 AI Agent:**
> You should focus on hip mobility or core stability.


## ❓ FAQ

**Q: How does the tool differentiate between lumbar and thoracic pain?**
The `analyze_pain_origin` tool evaluates the reported pain location and paddling posture to determine if the issue is primarily in the lumbar or thoracic region.

**Q: Can I get specific exercises for my back pain?**
Yes, after identifying the cause, you can use `get_corrective_recommendations` to receive actionable mobility or postural advice.

**Q: Does surfing style affect the risk assessment?**
Yes, the `assess_risk_profile` tool considers whether you practice shortboarding, longboarding, or bigwave surfing to calculate your specific risk level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-back-pain-analyzer](https://vinkius.com/en/ai-agent-connect/surf-back-pain-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Back Pain Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-back-pain-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Back Pain Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-back-pain-analyzer": {
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
