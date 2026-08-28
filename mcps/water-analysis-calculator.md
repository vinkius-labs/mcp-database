# Water Analysis Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/water-analysis-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculates water quality indices, hardness levels, and regulatory compliance.

## Description
This MCP server provides specialized tools for water quality assessment. It allows AI agents to determine the Water Quality Index (WQI) using `calculate_wqi`, categorize mineral content with `classify_hardness`, and evaluate regulatory adherence via `assess_compliance`. It also offers a high-level chemical overview through `get_parameter_summary`.


## Available Tools (4)
- **calculate_wqi**: Determines the overall Water Quality Index based on provided analytical measurements
- **classify_hardness**: Categorizes the hardness level of a water sample
- **assess_compliance**: g., drinking_water or wastewater).

Evaluates if a water sample meets the regulatory requirements for a specific use
- **get_parameter_summary**: Provides a high-level overview of the chemical state of the water sample


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Water Analysis Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the water quality index for these values: pH 7.2, Turbidity 1.5, Nitrates 5.0?"

**🤖 AI Agent:**
> The Water Quality Index is 85, which is classified as Excellent.

---

**👤 You:**
> "Is this water compliant for drinking? pH 6.5, Lead 0.02."

**🤖 AI Agent:**
> No, the water is not compliant. The lead concentration exceeds the limit.

---

**👤 You:**
> "Classify the hardness for calcium 40 and magnesium 15."

**🤖 AI Agent:**
> The total hardness is 55, which is classified as Soft.


## ❓ FAQ

**Q: What can I calculate with this server?**
You can calculate the Water Quality Index, classify water hardness, assess compliance against drinking water or wastewater standards, and get a summary of chemical parameters.

**Q: How do I check if my water meets drinking standards?**
Use the `assess_compliance` tool and specify 'drinking_water' as the use case.

**Q: What inputs are needed for hardness classification?**
You need to provide the calcium and magnesium concentrations to the `classify_hardness` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/water-analysis-calculator](https://vinkius.com/ai-agent-connect/water-analysis-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Water Analysis Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `water-analysis-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Water Analysis Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "water-analysis-calculator": {
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
