# Concrete Mix Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-mix-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate precise concrete mix proportions using ACI methodology.

## Description
This MCP server provides professional-grade tools for concrete mix design based on the ACI methodology. It allows engineers and technicians to calculate the exact mass of cement, water, fine aggregate, and coarse aggregate required for 1 m³ of concrete. Use `calculate_proportions` to determine the base mix, `adjust_for_moisture` to account for aggregate moisture states, and `validate_workability` to ensure the target slump is achievable within the specified water-cement ratio. It also provides access to physical constants via `get_cement_constants`.


## Available Tools (4)
- **adjust_for_moisture**: Modifies the calculated water and aggregate weights based on the existing moisture state of the aggregates
- **calculate_proportions**: Calculates the complete mass of all constituent materials for 1 m³ of concrete
- **get_cement_constants**: Retrieves the specific properties and water requirements associated with a specific cement type
- **validate_workability**: Checks if the proposed mix can achieve the requested slump without exceeding the w/c ratio limit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Mix Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a mix for 30 MPa strength using Type I cement, 20mm aggregate, and a 0.45 water-cement ratio."

**🤖 AI Agent:**
> For a 30 MPa target strength, the required mix per 1 m³ is: 350.5 kg of cement, 157.7 kg of water, 780.2 kg of fine aggregate, and 1050.4 kg of coarse aggregate.

---

**👤 You:**
> "Is a 0.50 w/c ratio with 25mm aggregate feasible for a 100mm slump?"

**🤖 AI Agent:**
> The mix is feasible. The estimated slump is 115mm, which meets your 100mm requirement. No additional admixtures are strictly required for this consistency.

---

**👤 You:**
> "What are the properties for Type V cement?"

**🤖 AI Agent:**
> Type V cement has a specific gravity of 3.15 and a typical water demand of 165 kg/m³ for standard mixes.


## ❓ FAQ

**Q: How do I account for wet aggregates in my mix?**
You should use the `adjust_for_moisture` tool. Provide the output from the initial proportion calculation and the moisture data for your aggregates to get the corrected weights.

**Q: Can I check if my target slump is realistic?**
Yes, use the `validate_workability` tool. It checks if the combination of water-cement ratio, aggregate size, and slump requirement is physically feasible.

**Q: Does this tool handle environmental exposure limits?**
Yes, the `calculate_proportions` tool accepts an `exposureCategory` to ensure the water-cement ratio complies with durability requirements for Mild, Moderate, or Severe conditions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-mix-design](https://vinkius.com/ai-agent-connect/concrete-mix-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Mix Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-mix-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Mix Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-mix-design": {
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
