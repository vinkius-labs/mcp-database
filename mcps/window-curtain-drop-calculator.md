# Window Curtain Drop Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/window-curtain-drop-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Calculate precise curtain fabric lengths based on window height and style.

## Description
This MCP server provides specialized tools to determine the exact vertical fabric length required for window curtains. It handles complex calculations including heading styles like `rodPocket` or `eyelet`, bottom hem types such as `puddle` or `floating`, and floor clearance adjustments. Use `calculate_stylized_drop` to automatically account for hardware allowances or `estimate_fabric_requirement` to factor in the distance from the floor to the rod.


## Available Tools (4)
- **calculate_basic_drop**: Calculates the simplest curtain length based on a raw window height and a single extra length value
- **calculate_stylized_drop**: Calculates the curtain length by automatically determining extra length based on the selected heading style
- **estimate_fabric_requirement**: Determines the total drop considering a desired floor clearance
- **validate_drop_safety**: Checks if a calculated drop is physically viable for a specific installation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Window Curtain Drop Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the drop for a window that is 200cm high with a rod pocket heading and a puddle hem."

**🤖 AI Agent:**
> The total drop for your window is 225cm, which includes the necessary allowance for the rod pocket and the puddle effect.

---

**👤 You:**
> "I have a rod at 250cm height. Will a 260cm curtain work?"

**🤖 AI Agent:**
> No, a 260cm curtain will drag on the floor because the total drop exceeds the rod height of 250cm.

---

**👤 You:**
> "What is the fabric needed for a 150cm window with a 10cm floor clearance?"

**🤖 AI Agent:**
> The final fabric length required is 160cm, accounting for the window height and your desired clearance.


## ❓ FAQ

**Q: How do I calculate the drop for a specific curtain style?**
You can use the `calculate_stylized_drop` tool. Simply provide the window height and select your preferred heading style and bottom hem type.

**Q: Can I account for the gap between the curtain and the floor?**
Yes, the `estimate_fabric_requirement` tool allows you to specify a desired clearance to ensure the curtain hangs at the perfect height.

**Q: Is it possible to check if my curtain will drag on the floor?**
Yes, use `validate_drop_safety` to check if your calculated drop is physically viable for your specific rod height.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/window-curtain-drop-calculator](https://vinkius.com/en/ai-agent-connect/window-curtain-drop-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Window Curtain Drop Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `window-curtain-drop-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Window Curtain Drop Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "window-curtain-drop-calculator": {
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
