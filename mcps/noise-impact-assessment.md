# Noise Impact Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/noise-impact-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Assess noise impact from oil and gas operations using sound propagation modeling.

## Description
This MCP server provides specialized tools for analyzing noise pollution in industrial oil and gas environments. It allows users to retrieve standardized noise profiles via `get_source_profiles`, predict noise levels at specific locations using `calculate_receptor_noise`, and determine total exposure with `aggregate_cumulative_impact`. Finally, it identifies necessary safety actions through `evaluate_mitigation_needs` by comparing results against regulatory limits for residential, industrial, or wildlife receptors.


## Available Tools (4)
- **aggregate_cumulative_impact**: Determine the total noise exposure when multiple sources contribute to the same receptor
- **calculate_receptor_noise**: Predict the specific noise level at a given location based on source and environment
- **evaluate_mitigation_needs**: Identify if the noise impact exceeds safety or regulatory limits and suggest necessary actions
- **get_source_profiles**: Retrieve standardized noise emission data for specific oil and gas equipment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Noise Impact Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the noise level of a compressor at 50 meters with soft ground?"

**🤖 AI Agent:**
> The predicted noise level at 50 meters is 62.4 dB.

---

**👤 You:**
> "Calculate the total noise if I have three sources at 65, 70, and 68 dB."

**🤖 AI Agent:**
> The cumulative noise level is 72.1 dB.

---

**👤 You:**
> "Is a noise level of 75 dB compliant for a residential area with a 70 dB limit?"

**🤖 AI Agent:**
> No, the noise level exceeds the limit by 5 dB. Suggested actions: install acoustic barriers or reduce operating hours.


## ❓ FAQ

**Q: How does the tool calculate noise at a distance?**
The `calculate_receptor_noise` tool uses geometric spreading and ground absorption factors to predict how sound levels diminish over distance.

**Q: Can I combine noise from multiple machines?**
Yes, use `aggregate_cumulative_impact` to calculate the total logarithmic decibel level from multiple individual noise sources.

**Q: How are mitigation strategies determined?**
The `evaluate_mitigation_needs` tool compares the calculated noise against regulatory limits for the specific receptor type and suggests actions like installing acoustic barriers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/noise-impact-assessment](https://vinkius.com/en/ai-agent-connect/noise-impact-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Noise Impact Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `noise-impact-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Noise Impact Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "noise-impact-assessment": {
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
