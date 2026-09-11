# Produced Water Quality Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/produced-water-quality-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [oil-and-gas](../categories/oil-and-gas.md)

Models produced water quality for discharge or reinjection.

## Description
This MCP provides tools to model the chemical composition of produced water and predict the impact of treatment processes. Use `get_source_water_profile` to retrieve baseline contaminant levels, `simulate_treatment_impact` to calculate how treatment steps reduce contaminants, `evaluate_compliance` to check if the final water meets regulatory limits for discharge or reinjection, and `get_treatment_summary` to analyze overall treatment efficiency.


## Available Tools (4)
- **get_source_water_profile**: Retrieves the initial chemical composition of the water from the source
- **evaluate_compliance**: Compares the treated water quality against specific regulatory thresholds
- **get_treatment_summary**: Provides a high-level overview of the effectiveness of a treatment train
- **simulate_treatment_impact**: Calculates how specific treatment steps will alter the water composition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Produced Water Quality Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the initial composition of water from source ID 'well-001'?"

**🤖 AI Agent:**
> The initial composition for well-001 is: oilAndGrease: 150 mg/L, tds: 45000 mg/L, heavyMetals: 0.5 mg/L, and norm: 0.1 Bq/L.

---

**👤 You:**
> "If I apply a filtration process with 80% efficiency to water with 100 mg/L of oil and grease, what is the final concentration?"

**🤖 AI Agent:**
> The final concentration of oil and grease will be 20 mg/L.

---

**👤 You:**
> "Is water with 5 mg/L of oil and grease compliant for discharge?"

**🤖 AI Agent:**
> No, the water is non-compliant for discharge because the oil and grease level exceeds the regulatory limit.


## ❓ FAQ

**Q: How do I check if my water is ready for discharge?**
You can use the `evaluate_compliance` tool by providing the final water quality profile and setting the destination type to 'discharge'.

**Q: Can I simulate multiple treatment steps at once?**
Yes, the `simulate_treatment_impact` tool allows you to provide an array of treatment steps to see the cumulative effect on water composition.

**Q: What contaminants are tracked?**
The model tracks oil and grease, total dissolved solids (TDS), heavy metals, and naturally occurring radioactive material (NORM).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/produced-water-quality-model](https://vinkius.com/en/ai-agent-connect/produced-water-quality-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Produced Water Quality Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `produced-water-quality-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Produced Water Quality Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "produced-water-quality-model": {
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
