# Shotcrete Thickness Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/shotcrete-thickness-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculates required shotcrete thickness, reinforcement, and application layers for ground support.

## Description
This MCP server provides specialized tools for designing shotcrete ground support in mining and tunneling environments. It calculates the `get_minimum_thickness` required based on rock mass quality and excavation span. It also identifies necessary reinforcement types using `calculate_reinforcement_requirements` and suggests optimal application methods via `determine_layer_configuration`. Finally, it ensures safety compliance through `validate_support_design` to confirm the design meets structural requirements for the specific span.


## Available Tools (4)
- **calculate_reinforcement_requirements**: Identifies the necessary type and amount of reinforcement needed to meet support requirements
- **determine_layer_configuration**: Suggests the optimal method for applying the shotcrete (single vs. multi-layer)
- **get_minimum_thickness**: Determines the baseline shotcrete thickness required based on rock quality and opening width
- **validate_support_design**: Performs a final check to ensure the combination of thickness and reinforcement meets the safety threshold for the given span


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shotcrete Thickness Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the minimum shotcrete thickness needed for a 5 meter span in poor rock conditions?"

**🤖 AI Agent:**
> The minimum thickness required for a 5 meter span in poor rock conditions is 150mm.

---

**👤 You:**
> "What reinforcement is needed for a 120mm thickness with standard support requirements?"

**🤖 AI Agent:**
> For a 120mm thickness with standard support, fiber reinforcement is recommended with a low density.

---

**👤 You:**
> "Suggest a layer configuration for 250mm of total thickness using mesh reinforcement."

**🤖 AI Agent:**
> For 250mm of mesh-reinforced shotcrete, you should apply 2 layers of 125mm each to ensure full encapsulation of the mesh.


## ❓ FAQ

**Q: How do I determine the required thickness for my excavation?**
You can use the `get_minimum_thickness` tool by providing the rock condition (e.g., 'Good' or 'Poor') and the span of the excavation in meters.

**Q: Does this tool handle mesh reinforcement?**
Yes, the `calculate_reinforcement_requirements` tool will indicate if mesh is required based on the thickness and support class.

**Q: How can I verify if my design is safe?**
Use the `validate_support_design` tool with your span, thickness, and reinforcement type to receive a safety validation and recommendation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/shotcrete-thickness-design](https://vinkius.com/ai-agent-connect/shotcrete-thickness-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shotcrete Thickness Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shotcrete-thickness-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shotcrete Thickness Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shotcrete-thickness-design": {
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
