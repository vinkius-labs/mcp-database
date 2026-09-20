# Sleep Restriction Therapy Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sleep-restriction-therapy-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Clinical tool for planning CBT-I sleep restriction protocols.

## Description
This MCP server provides clinical tools for Sleep Restriction Therapy (SRT), a core component of Cognitive Behavioral Therapy for Insomnia (CBT-I). It allows AI agents to manage sleep titration by calculating sleep windows, evaluating efficiency, and generating weekly schedules. Use `calculate_initial_window` to establish a starting protocol, `evaluate_titration` to adjust sleep windows based on efficiency, and `generate_weekly_schedule` to provide patients with structured daily routines.


## Available Tools (4)
- **get_current_protocol_status**: Retrieves the current parameters of an existing sleep restriction plan
- **calculate_initial_window**: Generates the starting sleep restriction protocol based on a patient's current insomnia metrics
- **evaluate_titration**: Determines how to adjust the sleep window based on the previous week's sleep efficiency
- **generate_weekly_schedule**: Produces a structured schedule for a patient to follow for the upcoming week


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sleep Restriction Therapy Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a new sleep window for a patient with 75% efficiency, 420 minutes of sleep, 540 minutes in bed, and a fixed wake-up time of 07:00."

**🤖 AI Agent:**
> The new sleep window is set for 23:00 to 07:00, providing a total duration of 480 minutes.

---

**👤 You:**
> "The patient's recent sleep efficiency was 90%. Should we adjust the window?"

**🤖 AI Agent:**
> Since the efficiency is above the target, the action is to EXPAND the sleep window by increasing the time in bed.

---

**👤 You:**
> "Generate a weekly schedule for patient ID 123 with a 480-minute window and a 06:30 wake-up time."

**🤖 AI Agent:**
> The daily schedule for the upcoming week is bedtime at 22:30 and wake time at 06:30.


## ❓ FAQ

**Q: How do I start a new sleep protocol?**
You can use the `calculate_initial_window` tool by providing the patient's current sleep efficiency, total sleep time, time in bed, and fixed wake-up time.

**Q: How is the sleep window adjusted?**
The window is adjusted using `evaluate_titration`, which determines if the sleep window should be expanded, contracted, or maintained based on recent sleep efficiency.

**Q: Can I see the current status of a patient's plan?**
Yes, use `get_current_protocol_status` with the patient's unique identifier to retrieve their current sleep window and efficiency targets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sleep-restriction-therapy-planner](https://vinkius.com/en/ai-agent-connect/sleep-restriction-therapy-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sleep Restriction Therapy Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sleep-restriction-therapy-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sleep Restriction Therapy Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sleep-restriction-therapy-planner": {
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
