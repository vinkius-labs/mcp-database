# Blood Flow Restriction Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/blood-flow-restriction-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate safe and effective BFR training parameters including pressure, sets, and reps.

## Description
This MCP server provides specialized tools for Blood Flow Restriction (BFR) training. It allows AI agents to determine safe cuff pressure ranges using `calculate_pressure_parameters`, design structured workouts with `generate_training_protocol`, assess physiological risks via `evaluate_safety_profile`, and verify equipment suitability with `get_equipment_compatibility`. It is designed to help athletes and coaches optimize metabolic stress while maintaining safety protocols.


## Available Tools (4)
- **calculate_pressure_parameters**: Determines the safe and effective cuff pressure range for the user
- **evaluate_safety_profile**: Assesses the risk level of the planned session based on user inputs
- **generate_training_protocol**: Provides the specific set, rep, and rest structure for a workout
- **get_equipment_compatibility**: Checks if the selected cuff is appropriate for the user's limb size


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blood Flow Restriction Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the pressure parameters for an arm with a 30cm circumference using a 5cm wide cuff."

**🤖 AI Agent:**
> The target pressure for your arm is 45 mmHg, with a safe range between 40 and 50 mmHg.

---

**👤 You:**
> "Generate a training protocol for an advanced user performing isotonic exercises at 50 mmHg pressure."

**🤖 AI Agent:**
> Your protocol consists of 4 sets: 30, 15, 15, and 15 repetitions, with 30-second rest intervals.

---

**👤 You:**
> "Is a 4cm wide cuff suitable for a 35cm circumference leg?"

**🤖 AI Agent:**
> No, the cuff is too narrow for this limb size and may cause excessive localized pressure.


## ❓ FAQ

**Q: How do I know if the pressure is safe?**
You can use the `evaluate_safety_profile` tool to assess risk levels based on your limb circumference and any pre-existing medical conditions.

**Q: Can I use this for both arm and leg training?**
Yes, the `calculate_pressure_parameters` tool supports both arm and leg limb types with specific physiological thresholds for each.

**Q: What information do I need to provide?**
To get accurate results, you should provide your limb circumference, the width of your pressure cuff, and your training experience level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/blood-flow-restriction-calculator](https://vinkius.com/en/ai-agent-connect/blood-flow-restriction-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blood Flow Restriction Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `blood-flow-restriction-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blood Flow Restriction Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blood-flow-restriction-calculator": {
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
