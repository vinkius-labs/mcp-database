# Rebar Lap Length Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/rebar-lap-length-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate required rebar lap splice lengths and verify structural compliance.

## Description
This MCP server provides specialized tools for structural engineers to determine required rebar lap splice lengths. It accounts for material properties like concrete and steel strength, bar position (top bar vs. standard), and epoxy coatings. Use `calculate_lap_length` to find the required overlap, `validate_stagger_requirement` to ensure proper spacing between splices, and `check_cover_compliance` to verify concrete cover requirements. It also provides a `get_splice_summary` for quick reporting.


## Available Tools (4)
- **calculate_lap_length**: Calculates the primary required lap splice length for a single rebar configuration
- **check_cover_compliance**: Verifies if the provided concrete cover is sufficient for the bar diameter
- **get_splice_summary**: Provides a human-readable summary of a calculated reinforcement configuration
- **validate_stagger_requirement**: Determines the minimum distance required between two consecutive splices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rebar Lap Length Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the lap length for a 20mm rebar with 30MPa concrete and 400MPa steel using Class B splice."

**🤖 AI Agent:**
> The required lap length for this configuration is 1250 mm.

---

**👤 You:**
> "Is a 40mm concrete cover enough for a 25mm epoxy-coated rebar?"

**🤖 AI Agent:**
> Yes, the concrete cover is sufficient for the effective diameter of the epoxy-coated bar.

---

**👤 You:**
> "What is the minimum stagger distance for a 1000mm lap length if staggering is required?"

**🤖 AI Agent:**
> The minimum stagger distance required is 300 mm.


## ❓ FAQ

**Q: How does bar position affect the calculation?**
Top bars require longer splices because concrete settlement can create a weak zone under the bar. The `calculate_lap_length` tool automatically adjusts for this.

**Q: Does epoxy coating change the required length?**
Yes, epoxy coating reduces bond strength between steel and concrete, so the `calculate_lap_length` tool increases the required overlap to maintain structural integrity.

**Q: How can I check if my concrete cover is sufficient?**
You can use the `check_cover_compliance` tool, which compares the bar diameter (including epoxy thickness) against your provided concrete cover.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/rebar-lap-length-calculator](https://vinkius.com/ai-agent-connect/rebar-lap-length-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rebar Lap Length Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rebar-lap-length-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rebar Lap Length Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rebar-lap-length-calculator": {
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
