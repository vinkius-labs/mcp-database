# Concrete Embed Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-embed-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Design embedment plates in concrete using ACI standards.

## Description
This MCP server provides specialized engineering tools for designing embedment plates in concrete structures according to ACI Appendix D and Chapter 17 standards. It calculates critical design parameters including anchor bolt size, quantity, embedment depth, and plate thickness. The server accounts for complex engineering factors such as group action and edge effects to ensure structural integrity.


## Available Tools (4)
- **calculate_anchor_selection**: Determines the required anchor bolt diameter and quantity based on the applied loads
- **calculate_embedment_depth**: Determines the necessary depth for the anchors to ensure sufficient concrete breakout and pull-out strength
- **calculate_plate_thickness**: Calculates the required thickness of the steel embedment plate
- **validate_group_action**: Verifies if the selected anchor arrangement is valid given the concrete geometry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Embed Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What anchor bolt size and quantity do I need for a 50kN tension load and 10kNm moment in 30MPa concrete?"

**🤖 AI Agent:**
> For a 50kN tension load and 10kNm moment in 30MPa concrete, you need 4 bolts with a diameter of 20mm.

---

**👤 You:**
> "Calculate the required embedment depth for 4 bolts of 20mm diameter in 30MPa concrete with a 150mm edge distance."

**🤖 AI Agent:**
> The required embedment depth is 185mm to ensure sufficient concrete breakout capacity.

---

**👤 You:**
> "What is the minimum plate thickness for a 40kN tension and 5kN shear load on a 200x200mm plate with 16mm bolts?"

**🤖 AI Agent:**
> The minimum required steel plate thickness is 12mm.


## ❓ FAQ

**Q: Which engineering standards does this tool follow?**
The design calculations follow ACI Appendix D and Chapter 17 standards for concrete design.

**Q: Can I calculate the required plate thickness?**
Yes, you can use the `calculate_plate_thickness` tool to determine the minimum steel plate thickness required for your specific loads and dimensions.

**Q: How does the tool handle edge effects?**
The `calculate_embedment_depth` tool incorporates edge distance to adjust the capacity of the concrete breakout cone, ensuring the design accounts for proximity to concrete edges.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-embed-design](https://vinkius.com/ai-agent-connect/concrete-embed-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Embed Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-embed-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Embed Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-embed-design": {
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
