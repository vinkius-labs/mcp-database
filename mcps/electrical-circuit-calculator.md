# Electrical Circuit Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/electrical-circuit-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Verify residential electrical compliance, voltage drop, and breaker adequacy using NEC standards.

## Description
This MCP server provides deterministic tools for residential electrical calculations based on the National Electrical Code (NEC). It allows AI agents to verify if a circuit breaker is sufficient for a specific load, calculate voltage drop across conductors, and identify the minimum required wire gauge to maintain safety and efficiency. Use `calculate_current_and_compliance` to check breaker capacity for continuous or non-continuous loads, `calculate_voltage_drop` to measure energy loss, and `find_minimum_wire_gauge` to ensure voltage drop stays below the 3% threshold.


## Available Tools (3)
- **calculate_current_and_compliance**: Calculates the actual current draw and determines if a specific breaker is sufficient
- **calculate_voltage_drop**: Determines the percentage of voltage lost over the length of the wire
- **find_minimum_wire_gauge**: Identifies the smallest AWG wire required to keep voltage drop within safe limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Electrical Circuit Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is a 20A breaker enough for a 1500W continuous load at 120V?"

**🤖 AI Agent:**
> No, a 20A breaker is not adequate for a 1500W continuous load at 120V. The current draw is 12.5A, but the continuous load limit for a 20A breaker is 16A. Wait, let me re-calculate: 1500W / 120V = 12.5A. 80% of 20A is 16A. Since 12.5A is less than 16A, the breaker is adequate.

---

**👤 You:**
> "What is the voltage drop for a 1200W load at 120V using 12 AWG copper wire over 50 feet?"

**🤖 AI Agent:**
> The voltage drop is 1.25% with an end voltage of 118.5V.

---

**👤 You:**
> "Find the minimum wire gauge for a 240V, 3000W load over 100 feet using copper."

**🤖 AI Agent:**
> The minimum required wire gauge is 10 AWG, which results in an expected voltage drop of 2.45%.


## ❓ FAQ

**Q: How does the tool handle continuous loads?**
Following NEC rules, the tool limits continuous load capacity to 80% of the breaker's rated amperage to prevent overheating.

**Q: What is the maximum allowable voltage drop?**
The tool aims to keep voltage drop at or below 3% to ensure equipment safety and efficiency.

**Q: Can I calculate requirements for aluminum wiring?**
Yes, the tools account for the higher resistivity of aluminum compared to copper when calculating voltage drop and wire gauge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/electrical-circuit-calculator](https://vinkius.com/ai-agent-connect/electrical-circuit-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Electrical Circuit Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `electrical-circuit-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Electrical Circuit Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "electrical-circuit-calculator": {
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
