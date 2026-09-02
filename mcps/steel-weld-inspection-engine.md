# Steel Weld Inspection Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/steel-weld-inspection-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculates weld quality compliance, discontinuity limits, and inspection planning based on AWS D1.1 and ISO 5817 standards.

## Description
This MCP server provides specialized engineering tools for structural steel inspection. It allows AI agents to determine maximum allowable discontinuity sizes using `get_discontinuity_limits`, plan sensor placement with `calculate_inspection_spacing`, and establish inspection coverage via `determine_test_frequency`. It also provides a critical validation step with `validate_inspection_result` to check if detected defects meet specific AWS D1.1 or ISO 5817 quality levels. The engine accounts for material thickness, weld geometry, and fatigue loading conditions to ensure structural integrity.


## Available Tools (4)
- **calculate_inspection_spacing**: Calculate the maximum allowable inspection spacing
- **get_discontinuity_limits**: Get maximum allowable discontinuity sizes for a specific weld
- **determine_test_frequency**: Determine the required test frequency for weld inspection
- **validate_inspection_result**: Validate if a detected defect meets the acceptance criteria


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steel Weld Inspection Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the maximum allowable porosity size for a 10mm fillet weld with ISO_5817_B criteria?"

**🤖 AI Agent:**
> The maximum allowable porosity size for a 10mm fillet weld under ISO 5817 Level B is 1.5mm.

---

**👤 You:**
> "How much of a 5000mm weldment must be inspected if it is a primary structural weld?"

**🤖 AI Agent:**
> For a primary structural weldment of 5000mm, a 100% inspection length of 5000mm is required to meet compliance.

---

**👤 You:**
> "I found a 3mm undercut on a 12mm thick groove weld. Does it pass AWS_D1.1_STRUCTURAL?"

**🤖 AI Agent:**
> No, the 3mm undercut exceeds the permitted limit for this weld type and thickness under AWS D1.1 standards.


## ❓ FAQ

**Q: Which welding standards are supported?**
The engine supports AWS D1.1 (Structural Welding Code - Steel) and ISO 5817 (Quality levels for imperfections).

**Q: How does fatigue loading affect the results?**
When `isFatigueLoading` is enabled, the tool strictly reduces all allowable discontinuity dimensions to prevent crack initiation under cyclic loads.

**Q: Can I use this for ultrasonic testing (UT) planning?**
Yes, you can use `calculate_inspection_spacing` to determine the maximum allowable distance between ultrasonic probes based on material thickness.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/steel-weld-inspection-engine](https://vinkius.com/ai-agent-connect/steel-weld-inspection-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steel Weld Inspection Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steel-weld-inspection-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steel Weld Inspection Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steel-weld-inspection-engine": {
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
