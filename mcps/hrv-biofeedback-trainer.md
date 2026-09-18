# HRV Biofeedback Trainer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hrv-biofeedback-trainer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Generates personalized HRV biofeedback training sessions to improve autonomic regulation.

## Description
This MCP server provides tools to design personalized HRV biofeedback training sessions. By using `get_session_plan`, users can generate a complete roadmap including breathing rates and session structures. The server also includes `validate_physiological_targets` to ensure inputs are consistent, `get_breathing_guidance` for specific inhalation and exhalation timings, and `calculate_progression_metrics` to manage training load over time. It is designed to help users reach their target physiological state through resonance breathing techniques.


## Available Tools (4)
- **calculate_progression_metrics**: Determines how much the training load should increase to reach the goal HRV
- **get_breathing_guidance**: Provides specific breathing instructions based on the calculated target breathing rate
- **get_session_plan**: Generates a complete training session roadmap based on user physiological targets
- **validate_physiological_targets**: Ensures that the provided HRV and coherence metrics are physiologically plausible and logically consistent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HRV Biofeedback Trainer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a 10-minute training session plan for a user with a current HRV of 45 and a goal HRV of 60, targeting a coherence level of 0.8."

**🤖 AI Agent:**
> Your 10-minute session plan is ready. The optimal breathing rate is 5.5 breaths per minute. The session includes a 2-minute warm-up, 6 minutes of active practice, and a 2-minute cool-down.

---

**👤 You:**
> "What are the breathing instructions for a target rate of 6 breaths per minute?"

**🤖 AI Agent:**
> For a rate of 6 breaths per minute, you should inhale for 5 seconds and exhale for 5 seconds for a total of 60 cycles.

---

**👤 You:**
> "Check if my physiological targets are valid: current HRV 50, goal HRV 40."

**🤖 AI Agent:**
> The targets are invalid because the goal HRV must be higher than the current HRV for a progressive training model.


## ❓ FAQ

**Q: What is HRV biofeedback?**
It is a technique that uses Heart Rate Variability (HRV) to help users regulate their autonomic nervous system through controlled breathing patterns.

**Q: How do I use the session planning tool?**
You can use `get_session_plan` by providing your current HRV, your goal HRV, the desired coherence target, and the total session duration.

**Q: Can I adjust my training intensity?**
Yes, you can use `calculate_progression_metrics` to determine the recommended duration increase or breathing rate adjustment for your next session.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hrv-biofeedback-trainer](https://vinkius.com/en/ai-agent-connect/hrv-biofeedback-trainer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HRV Biofeedback Trainer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hrv-biofeedback-trainer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HRV Biofeedback Trainer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hrv-biofeedback-trainer": {
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
