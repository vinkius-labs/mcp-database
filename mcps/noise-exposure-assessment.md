# Noise Exposure Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/noise-exposure-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [safety](../categories/safety.md)

Calculate workplace noise dose, TWA, and hearing protection requirements.

## Description
This MCP server provides professional tools for evaluating workplace acoustic risks. It allows for calculating the noise dose from individual events using `calculate_single_task_exposure`, aggregating multiple noise sources with `calculate_cumulative_exposure`, and retrieving regional regulatory thresholds via `get_regulatory_limits`. It also determines necessary hearing protection levels through `assess_protection_needs` based on calculated Time-Weighted Averages (TWA).


## Available Tools (4)
- **assess_protection_needs**: Determines if hearing protection is required and suggests the necessary reduction level
- **calculate_cumulative_exposure**: Aggregates multiple noise events into a total daily exposure profile
- **calculate_single_task_exposure**: Calculates the noise dose contributed by a single, continuous noise event
- **get_regulatory_limits**: Provides the standard thresholds for noise exposure based on regional regulations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Noise Exposure Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the noise dose for a 90 dB sound lasting 30 minutes?"

**🤖 AI Agent:**
> The noise dose for a 90 dB sound lasting 30 minutes is 12.5%.

---

**👤 You:**
> "Calculate the cumulative exposure for two tasks: 85 dB for 60 minutes and 95 dB for 15 minutes."

**🤖 AI Agent:**
> The total dose is 43.75% and the 8-hour TWA is 88.5 dB.

---

**👤 You:**
> "If the 8-hour TWA is 88 dB and the USA action level is 85 dB, is protection needed?"

**🤖 AI Agent:**
> Yes, hearing protection is required. A recommended attenuation of 3 dB is needed to bring the exposure below the action level.


## ❓ FAQ

**Q: How do I calculate the total daily noise exposure?**
You can use `calculate_cumulative_exposure` by providing an array of all noise tasks, including their sound levels and durations.

**Q: Does this tool support European regulations?**
Yes, you can use `get_regulatory_limits` with the region set to 'Europe' to retrieve the correct action levels and exchange rates.

**Q: How can I tell if a worker needs earplugs?**
After calculating the 8-hour TWA, use `assess_protection_needs` with the appropriate regional action level to determine if protection is required.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/noise-exposure-assessment](https://vinkius.com/ai-agent-connect/noise-exposure-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Noise Exposure Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `noise-exposure-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Noise Exposure Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "noise-exposure-assessment": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
