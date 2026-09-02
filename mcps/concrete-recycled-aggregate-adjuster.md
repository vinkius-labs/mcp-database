# Concrete Recycled Aggregate Adjuster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-recycled-aggregate-adjuster)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Adjust concrete mix designs for recycled aggregate replacement.

## Description
This MCP server provides specialized tools to adjust concrete mix designs when replacing natural aggregate with recycled material. It accounts for physical differences like increased water absorption and potential strength loss. Use `calculate_mix_adjustments` for a full recalculation of water, cement, and air entrainment, or `estimate_strength_loss` to predict compressive strength reduction. It also includes `get_water_compensation` for workability adjustments and `validate_material_suitability` to check if specific aggregate quality meets your target strength requirements.


## Available Tools (4)
- **validate_material_suitability**: Evaluates if a specific recycled aggregate quality is appropriate for a specific target strength
- **calculate_mix_adjustments**: Provides a comprehensive recalculation of the mix design components
- **estimate_strength_loss**: Predicts the potential reduction in compressive strength caused by the use of recycled aggregates
- **get_water_compensation**: Calculates only the water adjustment needed to maintain workability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Recycled Aggregate Adjuster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the mix adjustments for a 30 MPa concrete with 30% recycled aggregate replacement, 5% water absorption, and high quality aggregate."

**🤖 AI Agent:**
> To maintain 30 MPa with 30% replacement, you need an additional 4.5 L/m³ of water, a 4.2% increase in cement, and an air entrainment adjustment of -0.5%.

---

**👤 You:**
> "What is the estimated strength loss for 40 MPa concrete if I replace 20% of the aggregate with medium quality recycled material?"

**🤖 AI Agent:**
> The estimated strength will be 36.8 MPa, resulting in a total loss of 3.2 MPa.

---

**👤 You:**
> "Is low quality recycled aggregate suitable for a 45 MPa target strength?"

**🤖 AI Agent:**
> No, aggregate is unsuitable for high-strength applications at this quality level.


## ❓ FAQ

**Q: How does recycled aggregate affect concrete strength?**
Recycled aggregates often have higher porosity, which can lead to strength reduction. You can use `estimate_strength_loss` to predict this impact based on the replacement percentage and material quality.

**Q: How do I compensate for water absorption in recycled aggregates?**
You can use `get_water_compensation` to calculate the exact additional liters of water required per cubic meter to maintain workability.

**Q: Can I use low-quality recycled aggregate for high-strength concrete?**
Not always. Use `validate_material_suitability` to check if your specific aggregate quality is appropriate for your target strength.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-recycled-aggregate-adjuster](https://vinkius.com/ai-agent-connect/concrete-recycled-aggregate-adjuster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Recycled Aggregate Adjuster** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-recycled-aggregate-adjuster` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Recycled Aggregate Adjuster** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-recycled-aggregate-adjuster": {
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
