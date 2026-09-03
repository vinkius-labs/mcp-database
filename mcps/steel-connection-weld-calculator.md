# Steel Connection Weld Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/steel-connection-weld-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculates critical weld parameters like size, length, and electrode requirements for steel connections.

## Description
This MCP server provides precise engineering calculations for steel welding. It allows AI agents to determine the minimum weld size to prevent cracking, calculate the total load-carrying capacity of a weld, and find the required weld length to resist specific forces. Using tools like `recommend_weld_parameters`, an agent can generate a complete specification package including minimum size, required length, and electrode classification based on AISC and EN standards.


## Available Tools (4)
- **calculate_minimum_weld_size**: Determines the minimum allowable weld size to prevent cracking based on part thicknesses
- **determine_required_length**: Calculates how long a weld must be to safely resist a specific applied load
- **calculate_weld_strength**: Calculates the total load-carrying capacity of a specific weld configuration
- **recommend_weld_parameters**: Provides a complete package of weld specifications (size, length, and electrode) for a given connection scenario


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steel Connection Weld Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Recommend weld parameters for a 50kN load on S355 steel with part thicknesses of 10mm and 12mm using a fillet weld in flat position with SMAW."

**🤖 AI Agent:**
> The recommended specifications are: minimum size 6mm, required length 145mm, electrode E7018, and effective throat 4.2mm.

---

**👤 You:**
> "What is the minimum weld size for a connection with steel grades S235 and part thicknesses of 8mm and 15mm?"

**🤖 AI Agent:**
> The minimum allowable weld size is 5mm.

---

**👤 You:**
> "How much weld length is needed to resist 100kN with a 6mm effective throat for a fillet weld using E70XX electrode?"

**🤖 AI Agent:**
> The required weld length is 285mm.


## ❓ FAQ

**Q: Which standards does this tool follow?**
The calculations adhere to AISC (American Institute of Steel Construction) and EN (European) standards.

**Q: Can I get a full specification for a weld?**
Yes, by using the `recommend_weld_parameters` tool, you receive the minimum size, required length, electrode classification, and effective throat.

**Q: What inputs are needed for strength calculation?**
To use `calculate_weld_strength`, you need the applied force, weld length, effective throat, weld type, electrode strength, and process efficiency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/steel-connection-weld-calculator](https://vinkius.com/ai-agent-connect/steel-connection-weld-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steel Connection Weld Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steel-connection-weld-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steel Connection Weld Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steel-connection-weld-calculator": {
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
