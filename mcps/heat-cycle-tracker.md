# Heat Cycle Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/heat-cycle-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [biology](../categories/biology.md)

Predict reproductive cycles and fertile windows for unspayed animals based on breed data.

## Description
The Heat Cycle Tracker MCP server provides biological insights into the estrous cycles of unspayed female animals. By using tools like `get_breed_metadata`, `calculate_upcoming_heat`, and `segment_cycle_phases`, users can estimate future fertile windows, identify upcoming heat dates, and view a complete chronological breakdown of physiological phases including Proestrus, Estrus, Diestrus, and Anestrus based on breed-specific biological baselines.


## Available Tools (3)
- **get_breed_metadata**: Retrieve average cycle duration and phase distribution for a specific breed
- **segment_cycle_phases**: Provide a complete chronological breakdown of all biological phases for a single specific cycle
- **calculate_upcoming_heat**: Predict the date of the next fertile window and the estimated start of the next heat cycle


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heat Cycle Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the metadata for a Golden Retriever."

**🤖 AI Agent:**
> The average cycle duration for a Golden Retriever is 120 days, with specific proportions for Proestrus, Estrus, Diestrus, and Anestrus.

---

**👤 You:**
> "Predict the next heat date for a Siamese cat starting from 2023-01-01."

**🤖 AI Agent:**
> The estimated next heat date is calculated based on the Siamese breed's biological baseline, providing a predicted fertile window.

---

**👤 You:**
> "Show me the cycle phases for a Beagle starting on 2023-05-10."

**🤖 AI Agent:**
> The timeline includes Proestrus, Estrus, Diestrus, and Anestrus phases with specific start and end dates derived from the Beagle's cycle length.


## ❓ FAQ

**Q: What information does `get_breed_metadata` provide?**
It returns the average cycle duration and the percentage of time spent in each phase (Proestrus, Estrus, Diestrus, and Anestrus) for a specific breed.

**Q: How is the fertile window calculated in `calculate_upcoming_heat`?**
The tool uses the date of the last heat and the breed's specific Estrus phase proportion to estimate the start and end dates of the next fertile period.

**Q: Can I see a full timeline of the cycle phases?**
Yes, using the `segment_cycle_phases` tool, you can get a chronological breakdown of all biological stages for a specific cycle start date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heat-cycle-tracker](https://vinkius.com/mcp/heat-cycle-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Heat Cycle Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `heat-cycle-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Heat Cycle Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heat-cycle-tracker": {
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
