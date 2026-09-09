# Tubing Stress Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/tubing-stress-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

High-fidelity structural integrity and movement analysis for oil and gas completion tubing.

## Description
This MCP server provides specialized tools for analyzing the structural integrity of downhole completion strings. It performs triaxial stress analysis to calculate von Mises stress and safety factors, ensuring tubing can withstand combined axial, radial, and hoop loads. Users can predict axial displacement by accounting for thermal expansion and the ballooning effect. Additionally, it assesses buckling risk under compressive loads and generates high-level compliance reports using `get_safety_summary` to verify safety margins.


## Available Tools (4)
- **calculate_tubing_movement**: Predicts the total axial displacement of the tubing string
- **evaluate_buckling_risk**: Assesses the likelihood of the tubing column buckling under compressive loads
- **get_safety_summary**: Provides a high-level compliance report against standard safety margins
- **analyze_triaxial_integrity**: Determines if the tubing can withstand the combined loads without yielding


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tubing Stress Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Perform a triaxial stress analysis for tubing with 5-inch OD, 4.276-inch ID, 0.362-inch wall, and 80,000 psi yield strength under 10,000 psi internal and 5,000 psi external pressure."

**🤖 AI Agent:**
> The von Mises stress is 42,500 psi, resulting in a safety factor of 1.88. The status is pass.

---

**👤 You:**
> "Calculate the tubing movement for a 10,000 ft string with a temperature change from 60F to 150F."

**🤖 AI Agent:**
> The total axial displacement is 12.45 feet, consisting of 15.2 feet of thermal expansion and -2.75 feet of ballooning effect.

---

**👤 You:**
> "What is the buckling risk for a tubing string with a 15,000 lb compressive load in a 7-inch wellbore?"

**🤖 AI Agent:**
> The buckling critical load is 22,000 lbs. The current risk level is low, and the tubing is not buckled.


## ❓ FAQ

**Q: How does the server handle thermal effects?**
The `calculate_tubing_movement` tool incorporates temperature profiles to calculate thermal expansion or contraction as part of the total axial displacement.

**Q: Can I check if my tubing is compliant with safety standards?**
Yes, you can use `get_safety_summary` to receive a compliance report that checks both the safety factor and buckling status against your required margins.

**Q: What is the primary metric for material yielding?**
The server uses von Mises stress, calculated via `analyze_triaxial_integrity`, to predict the onset of yielding in ductile materials.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/tubing-stress-analysis](https://vinkius.com/ai-agent-connect/tubing-stress-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tubing Stress Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tubing-stress-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tubing Stress Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tubing-stress-analysis": {
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
