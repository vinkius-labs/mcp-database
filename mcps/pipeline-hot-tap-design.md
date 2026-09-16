# Pipeline Hot Tap Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pipeline-hot-tap-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering tool for safe hot tap connections to pressurized pipelines.

## Description
This MCP server provides specialized engineering calculations for performing hot taps on live, pressurized pipelines. It allows AI agents to determine safe connection parameters by calculating fitting selection, coupon geometry, pressure containment, and welding thermal profiles. Use `calculate_fitting_selection` to choose hardware, `calculate_coupon_geometry` to manage the metal plug, `verify_pressure_containment` to ensure safety margins, and `design_welding_profile` to obtain critical thermal parameters for welding on pressurized assets.


## Available Tools (4)
- **calculate_coupon_geometry**: Defines the dimensions and physical properties of the metal segment removed during the tapping process
- **calculate_fitting_selection**: Determines the appropriate connection hardware based on the existing pipeline and the desired branch size
- **design_welding_profile**: Generates the thermal parameters required to safely weld the connection onto a pressurized pipe
- **verify_pressure_containment**: Validates if the proposed design can safely withstand the operating pressure of the pipeline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pipeline Hot Tap Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What fitting should I use for a 24-inch pipe with a 6-inch branch and 0.5-inch wall thickness using API 5L X60 material?"

**🤖 AI Agent:**
> The recommended fitting is a Split Tee with a diameter of 24 inches, which is compatible with the specified material and branch size.

---

**👤 You:**
> "Is a design safe for 500 PSI if the pipe wall is 0.4 inches and the fitting wall is 0.5 inches with a safety factor of 1.5?"

**🤖 AI Agent:**
> Yes, the design is safe. The maximum allowable pressure is 750 PSI, providing a sufficient margin of safety.

---

**👤 You:**
> "What are the welding parameters for X70 material at 300 PSI and 25 degrees Celsius?"

**🤖 AI Agent:**
> The required preheat temperature is 150 degrees Celsius, with a maximum interpass temperature of 250 degrees Celsius.


## ❓ FAQ

**Q: How do I select the right hardware for my connection?**
You can use the `calculate_fitting_selection` tool. Provide the pipe diameter, wall thickness, branch diameter, and material grade to receive the recommended fitting type and compatibility status.

**Q: Can this tool verify if my design is safe for the current pressure?**
Yes. By using `verify_pressure_containment`, you can input the operating pressure and wall thicknesses to determine if the design meets the required safety factor.

**Q: What information is needed for the welding profile?**
To use `design_welding_profile`, you must provide the pipe material grade, the current operating pressure, and the ambient temperature.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pipeline-hot-tap-design](https://vinkius.com/en/ai-agent-connect/pipeline-hot-tap-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pipeline Hot Tap Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pipeline-hot-tap-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pipeline Hot Tap Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pipeline-hot-tap-design": {
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
