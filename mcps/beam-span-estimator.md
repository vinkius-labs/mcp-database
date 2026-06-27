# Beam Span Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/beam-span-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Quickly estimate concrete beam dimensions and compare with steel profiles.

## Description
The Beam Span Estimator is a structural engineering pre-dimensioning tool designed for the initial architectural scheme phase. It allows engineers to quickly estimate the minimum required height and width of concrete beams using the L/10 to L/12 rule-of-thumb method based on clear span. The tool also identifies equivalent steel profiles that match or exceed the calculated beam depth, facilitating rapid material comparison. Use `calculate_concrete_beam_dimensions` to find dimensions, `compare_with_steel_profiles` for steel alternatives, and `validate_load_adequacy` to assess structural risk levels.


## Available Tools (3)
- **calculate_beam_dimensions**: Estimates the required height and width for a concrete beam based on its span
- **compare_steel_profiles**: Identifies standard steel profiles that match or exceed the depth of a concrete beam
- **validate_load_adequacy**: Evaluates if the estimated load is within a typical range for the calculated beam geometry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beam Span Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a clear span of 5 meters. What should the minimum height and width of my concrete beam be?"

**🤖 AI Agent:**
> For a 5m span, the minimum height is approximately 0.42m (L/12) and the maximum is 0.50m (L/10). The suggested width is 0.25m.

---

**👤 You:**
> "Find steel profiles that match a concrete beam height of 0.4 meters."

**🤖 AI Agent:**
> The following matching profiles were found: W410x60 (depth 410mm), W460x52 (depth 460mm).

---

**👤 You:**
> "Is a load of 50 kN/m safe for a beam with a height of 0.3 meters?"

**🤖 AI Agent:**
> The risk level is High. A load of 50 kN/m on a 0.3m beam indicates a significant risk of excessive deflection.


## ❓ FAQ

**Q: How are the concrete beam dimensions calculated?**
The tool uses a rule-of-thumb method where the minimum height is one-twelfth of the clear span and the maximum height is one-tenth. The suggested width is estimated at 60% of the minimum height.

**Q: Can I compare concrete beams with steel sections?**
Yes, by using the `compare_with_steel_profiles` tool, you can find standard steel profiles that meet or exceed the depth of your calculated concrete beam.

**Q: What does load adequacy validation do?**
The `validate_load_adequacy` tool evaluates if the estimated load is appropriate for the beam's geometry, flagging high risk levels if a heavy load is paired with an insufficient beam depth.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/beam-span-estimator](https://vinkius.com/mcp/beam-span-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Beam Span Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `beam-span-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Beam Span Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "beam-span-estimator": {
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
