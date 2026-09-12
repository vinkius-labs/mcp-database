# Acrylic Acid Plant Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/acrylic-acid-plant-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Simulate chemical production of acrylic acid through oxidation kinetics and separation modeling.

## Description
This MCP server provides a complete engineering suite for designing acrylic acid production facilities. It allows AI agents to model the entire chemical lifecycle, from initial feedstock requirements to final product purification. Using `design_reactor_system`, you can determine optimal reactor volumes and catalyst types based on propylene availability and target purity. The suite includes `calculate_separation_train` to configure purification units for glacial acid or esters, `estimate_byproduct_profile` to predict waste generation, and `evaluate_economic_feasibility` to assess plant viability. It is designed to bridge chemical engineering models with AI-driven design workflows.


## Available Tools (4)
- **design_reactor_system**: Calculates the physical reactor specifications and the necessary catalyst type based on raw material inputs
- **estimate_byproduct_profile**: Predicts the quantity and types of byproducts generated during the oxidation process
- **evaluate_economic_feasibility**: Assesses if the plant design is viable based on feedstock costs and product value
- **calculate_separation_train**: Determines the configuration of purification units required to reach the target product state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Acrylic Acid Plant Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Design a reactor for 5000 units of capacity with 99% purity and 10000 units of propylene available."

**🤖 AI Agent:**
> The reactor requires a volume of 450 cubic meters using a Selective Oxidation Tier catalyst, operating at an optimal temperature of 350K.

---

**👤 You:**
> "What is the byproduct profile for a reactor operating at 380K with 2000 units of propylene?"

**🤖 AI Agent:**
> The process will generate CO2 and organic acid byproducts with a mass yield of 0.85 per unit of propylene.

---

**👤 You:**
> "Is it profitable to produce glacial acid if propylene costs 500 per unit and product value is 1200 per unit?"

**🤖 AI Agent:**
> Based on the provided reactor and separation configurations, the plant shows a positive gross margin and a break-even capacity of 1200 units.


## ❓ FAQ

**Q: What can I design with this server?**
You can design full reactor systems, determine separation train configurations for glacial acid or esters, estimate byproduct profiles, and evaluate the economic feasibility of the entire plant design.

**Q: How do I calculate the reactor size?**
Use the `design_reactor_system` tool by providing the available propylene, your target capacity, and the desired product purity.

**Q: Can I model ester production?**
Yes, by using `calculate_separation_train` and specifying 'ester' as the product type, the tool will include the necessary esterification reactor stages and distillation requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/acrylic-acid-plant-designer](https://vinkius.com/en/ai-agent-connect/acrylic-acid-plant-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Acrylic Acid Plant Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `acrylic-acid-plant-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Acrylic Acid Plant Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "acrylic-acid-plant-designer": {
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
