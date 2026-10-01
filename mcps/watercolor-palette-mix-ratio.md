# Watercolor Palette Mix Ratio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/watercolor-palette-mix-ratio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate exact pigment masses for custom watercolor mixes.

## Description
This MCP server provides precision calculation tools for watercolor artists. It allows you to determine the exact mass of individual pigment tubes required to create a specific volume of custom-mixed paint. Using `calculate_pigment_requirements`, you can input your target volume, color percentages, and paint density to get a detailed list of required pigments. You can also use `verify_inventory_sufficiency` to check if your current tube contents are enough for the mix, or `get_pigment_density_lookup` to find specific pigment densities. It is designed to account for loss allowance, ensuring you have enough material to cover waste on palettes and brushes.


## Available Tools (4)
- **get_pigment_density_lookup**: Retrieves the density for a specific pigment type
- **calculate_pigment_requirements**: Calculates the required mass of each pigment to achieve a target volume of mixed paint
- **summarize_mix_profile**: Provides a high-level overview of the planned mixture and the impact of the loss allowance
- **verify_inventory_sufficiency**: Checks if the artist has enough paint in their existing tubes to complete the calculated mix


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Watercolor Palette Mix Ratio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to make 50ml of a mix that is 40% Ultramarine Blue and 60% Lemon Yellow. The density is 1.2g/ml and I want a 10% loss allowance. How much of each do I need?"

**🤖 AI Agent:**
> You will need 26.4g of Ultramarine Blue and 39.6g of Lemon Yellow.

---

**👤 You:**
> "Show me a summary for a 100ml mix with 15% loss allowance and 1.1g/ml density."

**🤖 AI Agent:**
> The total target mass is 110g, the total mass with loss is 126.5g, and the expected loss mass is 16.5g.

---

**👤 You:**
> "I need 10g of Cobalt Blue. I have 5g in my tube. Do I have enough?"

**🤖 AI Agent:**
> No, you are short by 5g of Cobalt Blue.


## ❓ FAQ

**Q: How do I know if I have enough paint?**
You can use the `verify_inventory_sufficiency` tool by providing your calculated requirements and your current tube contents.

**Q: What is loss allowance?**
Loss allowance is a safety margin that accounts for the paint lost on palettes, brushes, or containers during the mixing process.

**Q: Can I find pigment densities?**
Yes, the `get_pigment_density_lookup` tool provides the density for specific pigment types.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/watercolor-palette-mix-ratio](https://vinkius.com/en/ai-agent-connect/watercolor-palette-mix-ratio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Watercolor Palette Mix Ratio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `watercolor-palette-mix-ratio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Watercolor Palette Mix Ratio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "watercolor-palette-mix-ratio": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
