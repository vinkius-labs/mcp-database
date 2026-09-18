# Vagal Tone Improvement Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/vagal-tone-improvement-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Personalized vagus nerve stimulation protocols based on HRV and lifestyle.

## Description
This MCP server provides specialized tools to design personalized vagus nerve stimulation regimens. By analyzing Heart Rate Variability (HRV), symptoms, and lifestyle factors, it generates multi-modal training plans. Users can use `generate_protocol` to create a full schedule, `calculate_cold_exposure_window` to find optimal thermal stress timing, `get_vocal_stimulation_routine` for vocal exercises like humming, and `evaluate_progression` to track training tiers.


## Available Tools (4)
- **calculate_cold_exposure_window**: Determines the optimal timing and duration for cold stimulus
- **evaluate_progression**: Determines if the user is ready to move to a more advanced tier of the protocol
- **generate_protocol**: Creates a comprehensive, multi-modal training plan based on user data
- **get_vocal_stimulation_routine**: Recommends specific vocal exercises (singing, humming, chanting)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vagal Tone Improvement Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a protocol for me. My HRV is 55ms, I feel anxious, and my stress is medium with 7 hours of sleep."

**🤖 AI Agent:**
> Your personalized protocol includes 10 minutes of resonant breathing daily, light humming for 5 minutes in the morning, and a brief cold water face plunge scheduled for 8:00 AM.

---

**👤 You:**
> "What is the best time for cold exposure if I want to build resilience and my stress is low?"

**🤖 AI Agent:**
> For your resilience goal with low stress, the optimal time is in the evening with a 3-minute cold exposure at an intermediate intensity.

---

**👤 You:**
> "I have 5 minutes for vocal exercises to help with anxiety. What should I do?"

**🤖 AI Agent:**
> I recommend 5 minutes of rhythmic humming to stimulate the vagus nerve and promote relaxation.


## ❓ FAQ

**Q: How do I start my protocol?**
You can start by using the `generate_protocol` tool with your current HRV baseline and lifestyle factors to receive a complete training plan.

**Q: Can I adjust my training based on stress levels?**
Yes, the `calculate_cold_exposure_window` tool specifically accounts for your current stress level to ensure the intensity is safe and effective.

**Q: How do I know when to advance to a higher tier?**
Use the `evaluate_progression` tool. It analyzes your recent HRV trends and symptom severity to determine if you are ready for a higher tier.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/vagal-tone-improvement-plan](https://vinkius.com/en/ai-agent-connect/vagal-tone-improvement-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vagal Tone Improvement Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vagal-tone-improvement-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vagal Tone Improvement Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vagal-tone-improvement-plan": {
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
