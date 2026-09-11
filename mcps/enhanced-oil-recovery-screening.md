# Enhanced Oil Recovery Screening MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/enhanced-oil-recovery-screening)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [energy](../categories/energy.md)

Evaluates technical feasibility and recovery uplift for EOR methods.

## Description
This MCP server provides specialized tools to evaluate Enhanced Oil Recovery (EOR) strategies. By analyzing reservoir parameters like oil gravity, viscosity, and temperature, users can use `screen_eor_methods` to rank suitable techniques such as thermal, chemical, or gas injection. The tool `get_method_feasibility_details` provides technical justifications for specific method recommendations, while `compare_eor_scenarios` allows for sensitivity analysis by comparing different reservoir profiles.


## Available Tools (4)
- **get_eor_screening_criteria**: Retrieves the hardcoded technical windows and constants used for the screening process
- **get_method_feasibility_details**: Provides a detailed breakdown of why a specific EOR method was or was not recommended
- **screen_eor_methods**: Evaluates the suitability of all EOR methods for a given set of reservoir parameters
- **compare_eor_scenarios**: Compares two different reservoir profiles to see how changing a single variable shifts the optimal EOR strategy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enhanced Oil Recovery Screening** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Screen EOR methods for an oil with 30 API gravity, 50 cP viscosity, 80C temperature, 1500m depth, and 0.6 oil saturation."

**🤖 AI Agent:**
> The most suitable method is gas injection with a suitability score of 0.85, followed by chemical flooding at 0.65.

---

**👤 You:**
> "Why is thermal injection not recommended for this reservoir?"

**🤖 AI Agent:**
> Thermal injection is not recommended because the oil gravity is too low and the reservoir depth exceeds the heat loss limits for steam injection.

---

**👤 You:**
> "What are the technical constraints for the chemical category?"

**🤖 AI Agent:**
> The chemical category constraints include temperature limits to prevent surfactant degradation and specific salinity tolerances.


## ❓ FAQ

**Q: What parameters are required for screening?**
To use `screen_eor_methods`, you must provide oil gravity, viscosity, reservoir temperature, depth, and remaining oil saturation.

**Q: Can I compare two different reservoir scenarios?**
Yes, the `compare_eor_scenarios` tool is designed to compare two reservoir profiles and identify shifts in the optimal EOR strategy.

**Q: How are suitability scores determined?**
Suitability scores are calculated by comparing your reservoir inputs against the technical constraints stored in the EOR Screening Database.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/enhanced-oil-recovery-screening](https://vinkius.com/en/ai-agent-connect/enhanced-oil-recovery-screening)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enhanced Oil Recovery Screening** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enhanced-oil-recovery-screening` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enhanced Oil Recovery Screening** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enhanced-oil-recovery-screening": {
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
