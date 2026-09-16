# Backcountry Rescue Logistics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/backcountry-rescue-logistics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Estimates emergency response times, evacuation methods, and aerial feasibility for wilderness rescues.

## Description
This MCP server provides critical logistics modeling for wilderness emergency response. It allows AI agents to calculate total rescue time, determine if a helicopter can be used via `assess_aerial_feasibility`, and identify the most appropriate evacuation strategy. By analyzing terrain difficulty, injury severity, and communication reliability, the server helps responders plan resource allocation and prioritize life-saving interventions.


## Available Tools (4)
- **assess_aerial_feasibility**: Determines if a helicopter can be utilized for the rescue
- **calculate_rescue_estimate**: Provides the core estimation of total response time and the primary evacuation strategy
- **determine_evacuation_priority**: Categorizes the urgency of the rescue to prioritize resource allocation
- **evaluate_communication_latency**: Calculates the delay between the incident occurring and rescuers receiving the signal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Backcountry Rescue Logistics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We are 5km from the roadhead in steep terrain. One person has a critical injury and we have a satellite messenger. How long will rescue take?"

**🤖 AI Agent:**
> The estimated rescue time is 4.5 hours, and the suggested evacuation method is Air.

---

**👤 You:**
> "Is it possible to use a helicopter for a rescue if the weather is foggy and the terrain is a flat meadow?"

**🤖 AI Agent:**
> No, aerial extraction is not feasible due to the primary constraint of Weather.

---

**👤 You:**
> "What is the priority for a group of 4 with a stable injury in clear weather?"

**🤖 AI Agent:**
> The priority level is Stable, and no specialized resources are required beyond standard ground response.


## ❓ FAQ

**Q: How does the server estimate rescue time?**
The server uses `calculate_rescue_estimate` to process distance, terrain difficulty, and communication latency to provide a total time estimate.

**Q: Can I check if a helicopter is an option?**
Yes, use the `assess_aerial_feasibility` tool to evaluate if weather and terrain allow for aerial extraction.

**Q: Does communication method affect the results?**
Yes, `evaluate_communication_latency` calculates delays based on whether you are using satellite, cellular, or analog signals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/backcountry-rescue-logistics](https://vinkius.com/en/ai-agent-connect/backcountry-rescue-logistics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Backcountry Rescue Logistics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `backcountry-rescue-logistics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Backcountry Rescue Logistics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "backcountry-rescue-logistics": {
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
