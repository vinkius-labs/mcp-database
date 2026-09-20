# Spa Client Journey Timer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/spa-client-journey-timer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scheduling](../categories/scheduling.md)

Maps the complete spa client experience from arrival to departure.

## Description
This MCP server provides precise scheduling and logistics for spa operations. It calculates optimal arrival times, phase-by-phase timings, and predicted departure moments. Use `calculate_journey_timeline` to generate a full schedule, `get_service_requirements` to find service durations, `predict_departure_time` to estimate exit times, or `validate_arrival_window` to ensure clients have enough preparation time.


## Available Tools (4)
- **calculate_journey_timeline**: Provides a comprehensive schedule of the entire client journey
- **get_service_requirements**: Retrieves the specific duration for a set of services
- **predict_departure_time**: Calculates the exact moment a client will exit the spa
- **validate_arrival_window**: Determines if a proposed arrival time is sufficient


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spa Client Journey Timer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the journey timeline for a massage and facial starting at 14:00, with 15 mins consultation, 10 mins changing, and 20 mins departure needs."

**🤖 AI Agent:**
> The recommended arrival time is 13:15. The total duration is 165 minutes. The journey includes Arrival, Consultation, Changing, Massage, Facial, and Departure phases.

---

**👤 You:**
> "What is the total time needed for a deep tissue massage and a scalp treatment?"

**🤖 AI Agent:**
> The total service time for these treatments is 110 minutes.

---

**👤 You:**
> "If a service starts at 10:00 and I need 30 minutes for prep, is arriving at 09:45 enough?"

**🤖 AI Agent:**
> No, arriving at 09:45 is not sufficient. You need at least 30 minutes of preparation, and arriving at 09:45 only provides 15 minutes before the 10:00 start.


## ❓ FAQ

**Q: How can I see the full schedule for a client?**
You can use the `calculate_journey_timeline` tool to receive a complete breakdown of all phases, including recommended arrival and total duration.

**Q: Can I check if a client will arrive too late for their service?**
Yes, use `validate_arrival_window` to determine if the proposed arrival time provides enough buffer for consultation and changing.

**Q: How do I know when a client will leave the facility?**
The `predict_departure_time` tool calculates the exact exit moment based on service start time and all required durations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/spa-client-journey-timer](https://vinkius.com/en/ai-agent-connect/spa-client-journey-timer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spa Client Journey Timer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spa-client-journey-timer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spa Client Journey Timer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spa-client-journey-timer": {
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
