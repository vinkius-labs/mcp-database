# Steel Bolt Pretension Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/steel-bolt-pretension-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate precise bolt pretension, tightening methods, and inspection protocols using AISC and EN 1090 standards.

## Description
This MCP server provides structural engineers and installers with the precise calculations needed for bolt pretensioning. It bridges the gap between design requirements and field execution by providing specific instructions for `calculate_minimum_pretension`, `determine_tightening_method`, `get_hardware_requirements`, and `validate_inspection_protocol`. Whether you are designing slip-critical connections or verifying torque-controlled installations, this tool ensures compliance with AISC and EN 1090 standards.


## Available Tools (4)
- **get_hardware_requirements**: Identifies the necessary washers and surface treatments required for the bolt assembly
- **validate_inspection_protocol**: Defines how the installer should verify that the pretension has been correctly applied
- **calculate_minimum_pretension**: Determines the required axial tension force needed for the connection
- **determine_tightening_method**: Provides the specific tightening instruction (rotation or torque) to achieve the target tension


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steel Bolt Pretension Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the minimum pretension for a 20mm bolt, grade 10.9, in a slip-critical connection requiring 50kN slip resistance?"

**🤖 AI Agent:**
> The minimum pretension required is 125.5 kN.

---

**👤 You:**
> "What is the torque value for a 22mm, grade 8.8 bolt that is lightly oiled?"

**🤖 AI Agent:**
> The required torque value is 345 Nm.

---

**👤 You:**
> "How should I inspect a turn-of-nut tightening for a grade 10.9 bolt?"

**🤖 AI Agent:**
> The inspection should be a visual angular measurement to ensure the specified rotation was achieved.


## ❓ FAQ

**Q: Which standards does this tool support?**
The tool supports calculations based on AISC and EN 1090 standards.

**Q: Can I use this for slip-critical connections?**
Yes, you can use `calculate_minimum_pretension` to determine the required tension for slip-critical connections.

**Q: How do I know if I need hardened washers?**
You can use `get_hardware_requirements` to identify if hardened washers are necessary for your specific bolt diameter and connection type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/steel-bolt-pretension-calculator](https://vinkius.com/ai-agent-connect/steel-bolt-pretension-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steel Bolt Pretension Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steel-bolt-pretension-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steel Bolt Pretension Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steel-bolt-pretension-calculator": {
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
