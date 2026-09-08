# Mine Power Distribution Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mine-power-distribution-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design electrical distribution networks for mining environments, including transformer sizing and cable selection.

## Description
This MCP server provides specialized engineering tools for designing electrical distribution networks in mining operations. It allows AI agents to calculate critical parameters such as transformer capacity using `calculate_transformer_capacity`, select appropriate conductors with `size_distribution_cables`, and configure safety devices via `determine_protection_settings`. The toolset also includes `analyze_system_efficiency` to evaluate how power factor and demand factor impact total apparent power requirements, ensuring designs meet industrial electrical standards.


## Available Tools (4)
- **analyze_system_efficiency**: Evaluates the impact of the power factor and demand factor on the overall system sizing
- **calculate_transformer_capacity**: Determines the required rating for a transformer based on the total connected load and operational factors
- **determine_protection_settings**: Calculates the threshold settings for protective devices to prevent equipment damage
- **size_distribution_cables**: Selects appropriate cable specifications to ensure voltage stability across the distribution distance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mine Power Distribution Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What transformer capacity do I need for a 500kVA load with a 0.8 demand factor and 0.9 power factor?"

**🤖 AI Agent:**
> The recommended transformer capacity is 555.56 kVA with a suggested safety margin of 55.56 kVA.

---

**👤 You:**
> "Calculate the cable size for a 200A load at 480V over a distance of 150 meters with a 3% allowable voltage drop."

**🤖 AI Agent:**
> The required conductor size is 70.0 mm² with an estimated voltage drop of 2.85%.

---

**👤 You:**
> "What should the trip threshold be for a device with a 150A full load current, a 20% overload margin, and a 1000A fault current?"

**🤖 AI Agent:**
> The pickup current is 150.0 A and the trip threshold is 180.0 A.


## ❓ FAQ

**Q: How do I calculate the required transformer size?**
You can use the `calculate_transformer_capacity` tool by providing the total connected load, the demand factor, and the power factor.

**Q: Can this tool help with cable selection?**
Yes, the `size_distribution_cables` tool calculates the required cross-sectional area and estimates voltage drop based on load, voltage, and distance.

**Q: Does it account for safety standards?**
Yes, the toolset uses industry-standard electrical design principles to determine protection settings and sizing requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mine-power-distribution-designer](https://vinkius.com/ai-agent-connect/mine-power-distribution-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mine Power Distribution Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mine-power-distribution-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mine Power Distribution Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mine-power-distribution-designer": {
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
