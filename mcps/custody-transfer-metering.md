# Custody Transfer Metering MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/custody-transfer-metering)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Precision engineering tool for designing high-accuracy fluid measurement systems using API MPMS standards.

## Description
This MCP server provides specialized tools for designing and verifying high-precision fluid measurement systems used in custody transfer. It allows AI agents to perform critical engineering tasks such as `select_meter` to identify optimal technology, `calculate_correction_factors` for environmental adjustments, `verify_prover_accuracy` to ensure certification capability, and `perform_uncertainty_analysis` to quantify total system error. All calculations adhere to API MPMS standards for oil and gas measurement.


## Available Tools (4)
- **calculate_correction_factors**: Determines the multipliers needed to adjust raw readings to standard conditions
- **select_meter**: Identifies the most appropriate metering technology for a specific application
- **perform_uncertainty_analysis**: Provides a comprehensive overview of the total measurement error for a complete system
- **verify_prover_accuracy**: Assesses if a specific prover is capable of certifying a meter to the required precision


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Custody Transfer Metering** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What meter should I use for crude oil with a flow rate between 100 and 500 units and a target uncertainty of 0.001?"

**🤖 AI Agent:**
> The recommended technology is a Coriolis meter, which provides a suitability score of 0.95 for this specific application.

---

**👤 You:**
> "Calculate the corrected volume for 1000 cubic meters at 25 degrees Celsius, 10 bar pressure, and 850 kg/m3 density."

**🤖 AI Agent:**
> The corrected volume is 1005.42 cubic meters, using a correction factor of 1.00542.

---

**👤 You:**
> "Is a prover with 0.0005 uncertainty sufficient for a meter requiring 0.001 uncertainty?"

**🤖 AI Agent:**
> Yes, the prover is compliant with a safety margin of 0.0005.


## ❓ FAQ

**Q: What standards does this tool follow?**
The tool follows the API MPMS (Manual of Petroleum Measurement Standards) for all calculations and methodologies.

**Q: How can I verify if my prover is sufficient?**
You can use the `verify_prover_accuracy` tool by providing the prover volume, its uncertainty, and the target meter uncertainty.

**Q: Can I calculate total system error?**
Yes, the `perform_uncertainty_analysis` tool calculates the total system uncertainty using the root sum square method.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/custody-transfer-metering](https://vinkius.com/en/ai-agent-connect/custody-transfer-metering)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Custody Transfer Metering** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `custody-transfer-metering` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Custody Transfer Metering** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "custody-transfer-metering": {
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
