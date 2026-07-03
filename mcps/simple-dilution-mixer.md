# Simple Dilution Mixer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/simple-dilution-mixer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Calculate exact volumes of solute and solvent needed for precise liquid dilution.

## Description
The Simple Dilution Mixer MCP server provides precision tools for laboratory and industrial applications. Use `calculate_dilution_volumes` to determine the exact amount of concentrate and base liquid required for a target volume and percentage. The `validate_concentration_tier` tool helps categorize concentrations into low, medium, or high tiers for safe handling, while `generate_dilution_recipe` produces clear, actionable instructions for technicians to follow during the mixing process.


## Available Tools (3)
- **calculate_dilution_volumes**: Determines the specific volumes of concentrate and base liquid required to reach a dilution goal
- **generate_dilution_recipe**: Converts calculated volumes into a set of clear, actionable instructions for a technician
- **validate_concentration_tier**: Categorizes a target concentration into a safety and handling tier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Simple Dilution Mixer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to make 500ml of a 10% solution. How much concentrate and water do I need?"

**🤖 AI Agent:**
> You will need 50ml of concentrate and 450ml of water.

---

**👤 You:**
> "What is the safety tier for a 75% concentration?"

**🤖 AI Agent:**
> A 75% concentration falls into the high intensity tier and is not within the standard range.

---

**👤 You:**
> "Generate a recipe for mixing 25ml of solute with 975ml of solvent."

**🤖 AI Agent:**
> Combine 25ml of the concentrate with 975ml of the base liquid to achieve the desired mixture.


## ❓ FAQ

**Q: How do I calculate the amount of concentrate needed?**
Use the `calculate_dilution_volumes` tool by providing your desired total final volume in ml and your target percentage. The tool will return the exact volume of solute and solvent required.

**Q: What does the concentration tier indicate?**
The `validate_concentration_tier` tool categorizes your target percentage into low, medium, or high tiers. This helps in determining the necessary safety precautions and handling equipment for the mixture.

**Q: Can I generate instructions for my staff?**
Yes, after calculating your volumes, use `generate_dilution_recipe` to create a human-readable instruction text that can be handed directly to technicians.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/simple-dilution-mixer](https://vinkius.com/mcp/simple-dilution-mixer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Simple Dilution Mixer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `simple-dilution-mixer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Simple Dilution Mixer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "simple-dilution-mixer": {
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
