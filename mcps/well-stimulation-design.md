# Well Stimulation Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/well-stimulation-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Optimize matrix acidizing and hydraulic fracturing treatments.

## Description
This MCP server provides specialized tools for reservoir stimulation engineering. Use `acidize_matrix` to calculate acid volumes and injection rates for mitigating formation damage. Use `fracture_design` to generate detailed hydraulic fracturing plans, including proppant schedules and fracture dimensions. The server also includes `stimulation_comparison` to evaluate the best method for specific well conditions and `skin_impact_analyzer` to predict flow rate improvements based on skin reduction.


## Available Tools (4)
- **skin_impact_analyzer**: Predicts the impact on wellbore performance based on skin reduction
- **stimulation_comparison**: Evaluates whether matrix acidizing or hydraulic fracturing is more suitable
- **acidize_matrix**: Calculates parameters for a matrix acidizing treatment to mitigate formation damage
- **fracture_design**: Generates a stimulation plan for hydraulic fracturing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Well Stimulation Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare acidizing and fracturing for a reservoir with 50 mD permeability and 5 skin."

**🤖 AI Agent:**
> Matrix acidizing is recommended for this reservoir due to the relatively high permeability of 50 mD.

---

**👤 You:**
> "Calculate acidizing parameters for carbonate scale damage with initial skin of 10 and target skin of 2 at 100 mD permeability."

**🤖 AI Agent:**
> The required acid volume is 150 liters with an injection rate of 12 L/min, resulting in an expected skin reduction to 2.

---

**👤 You:**
> "Design a fracture for a 100 mD reservoir with 50m length and 20m height using ceramic proppant for a 30% productivity increase."

**🤖 AI Agent:**
> The fracture design includes a ceramic proppant schedule with an estimated fracture width of 0.15 inches and a predicted productivity gain of 32%.


## ❓ FAQ

**Q: How do I decide between acidizing and fracturing?**
You can use the `stimulation_comparison` tool. It evaluates permeability and reservoir pressure to recommend the most efficient method.

**Q: Can I calculate the required acid volume?**
Yes, the `acidize_matrix` tool calculates the necessary acid volume, injection rate, and expected skin reduction based on your formation parameters.

**Q: What information is needed for a fracture design?**
To use `fracture_design`, you need to provide formation permeability, desired fracture length and height, proppant type, and target productivity increase.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/well-stimulation-design](https://vinkius.com/en/ai-agent-connect/well-stimulation-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Well Stimulation Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `well-stimulation-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Well Stimulation Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "well-stimulation-design": {
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
