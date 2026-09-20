# Advanced Sleep Phase Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/advanced-sleep-phase-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Assess Advanced Sleep Phase Syndrome (ASPS) and receive personalized light therapy and treatment guidance.

## Description
This MCP server provides a clinical-grade assessment engine for Advanced Sleep Phase Syndrome (ASPS). Users can use `analyze_asps_profile` to determine if their sleep patterns match ASPS criteria. Once a profile is established, the server provides actionable guidance through `calculate_light_therapy_schedule` to optimize circadian timing, and `evaluate_treatment_suitability` to suggest management strategies based on severity and age. It also includes `query_asps_knowledge_base` for deep dives into circadian biology and symptom management.


## Available Tools (4)
- **calculate_light_therapy_schedule**: Provides guidance on when to use light exposure to counteract the phase advance
- **analyze_asps_profile**: Conducts the primary assessment to determine if the user meets the criteria for ASPS
- **evaluate_treatment_suitability**: Recommends specific management strategies based on the severity of the syndrome
- **query_asps_knowledge_base**: Answers specific questions about ASPS symptoms and general characteristics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Advanced Sleep Phase Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I go to sleep at 7 PM and wake up at 3 AM every day. I feel very sleepy in the early evening. Do I have ASPS?"

**🤖 AI Agent:**
> Based on your sleep onset at 19:00 and awakening at 03:00, combined with early evening sleepiness, you meet the criteria for Advanced Sleep Phase Syndrome with a High severity level.

---

**👤 You:**
> "I have been diagnosed with moderate ASPS. When should I use light therapy?"

**🤖 AI Agent:**
> For a moderate phase advance with a current sleep onset of 20:00, the optimal light exposure window is between 18:00 and 19:00 for 45 minutes at high intensity.

---

**👤 You:**
> "What are the primary management strategies for severe ASPS?"

**🤖 AI Agent:**
> For severe cases, the primary recommendation is intensive phototherapy, supported by melatonin administration and specific lifestyle adjustments to delay the circadian phase.


## ❓ FAQ

**Q: How do I know if I have ASPS?**
You can use the `analyze_asps_profile` tool by providing your sleep onset and awakening times to see if you meet the clinical criteria.

**Q: Can this tool recommend light therapy?**
Yes, after assessing your profile, you can use `calculate_light_therapy_schedule` to get specific timing for light exposure.

**Q: What is the difference between mild and severe ASPS?**
Severity is determined by the magnitude of the phase advance. You can use `evaluate_treatment_suitability` to see how severity affects management recommendations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/advanced-sleep-phase-assessment](https://vinkius.com/en/ai-agent-connect/advanced-sleep-phase-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Advanced Sleep Phase Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `advanced-sleep-phase-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Advanced Sleep Phase Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "advanced-sleep-phase-assessment": {
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
