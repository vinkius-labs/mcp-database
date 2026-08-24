# Fabric Yardage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/fabric-yardage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fashion](../categories/fashion.md)

Calculate exact fabric, lining, and interfacing requirements for garment construction.

## Description
This MCP server provides precise tools for garment makers to determine material needs. Use `calculate_fabric_requirements` to find the exact meters of main fabric, lining, and interfacing required based on body measurements and garment type. You can also use `estimate_material_costs` to budget for your project and `validate_measurements` to ensure your body measurements are consistent for construction.


## Available Tools (3)
- **calculate_fabric_requirements**: Determines the total yardage/meterage needed for the main fabric, lining, and interfacing
- **estimate_material_costs**: Provides a rough estimate of the cost for the required materials
- **validate_measurements**: Ensures the provided body measurements are physically realistic and consistent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fabric Yardage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much fabric do I need for a silk dress? My bust is 90cm, waist is 70cm, hips are 95cm, and the length is 110cm. The fabric is 150cm wide and it is a solid color."

**🤖 AI Agent:**
> You will need 2.5 meters of main fabric. Since it is a solid color dress, no lining or interfacing is required by the standard calculation.

---

**👤 You:**
> "I'm making a plaid jacket. My measurements are bust 100cm, waist 85cm, hips 110cm, length 75cm. The fabric is 115cm wide. I am also tall."

**🤖 AI Agent:**
> For your plaid jacket, you will need 3.45 meters of main fabric (including the 25% pattern matching buffer and 15% tall adjustment), 2.5 meters of lining, and specific interfacing for the collar and cuffs.

---

**👤 You:**
> "Check if my measurements are realistic: bust 80cm, waist 95cm, hips 100cm, length 120cm."

**🤖 AI Agent:**
> The measurements are valid for garment construction.


## ❓ FAQ

**Q: How does the calculator handle pattern matching?**
When you select a stripe or plaid pattern, the `calculate_fabric_requirements` tool automatically adds a 25% buffer to the main fabric to ensure patterns align at the seams.

**Q: Can I estimate the total cost of my fabric?**
Yes, after calculating your yardage, use the `estimate_material_costs` tool to provide the price per meter for your materials and get a total cost estimate.

**Q: Does it account for different body types?**
Yes, you can specify if you are plus-size or tall to adjust the base fabric consumption accordingly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/fabric-yardage-calculator](https://vinkius.com/ai-agent-connect/fabric-yardage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fabric Yardage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fabric-yardage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fabric Yardage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fabric-yardage-calculator": {
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
