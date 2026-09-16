# Diesel Blend Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/diesel-blend-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Predict diesel blend properties including Cetane Index, sulfur content, and cold flow metrics.

## Description
This MCP server provides a specialized calculation engine for diesel fuel blending. It allows AI agents to determine the mass composition of blends, predict chemical properties like Cetane Index and sulfur content using `predict_chemical_properties`, and calculate critical cold flow metrics such as Cloud Point, Pour Point, and CFPP via `predict_cold_flow_properties`. It also includes tools to `validate_regulatory_compliance` for USA and Europe sulfur standards, ensuring blends meet regional requirements.


## Available Tools (4)
- **predict_chemical_properties**: Calculates the resulting Cetane Index and Sulfur content of the total blend
- **predict_cold_flow_properties**: Calculates the Cloud Point, Pour Point, and CFPP for the resulting blend
- **validate_regulatory_compliance**: Checks if the calculated blend meets specific regional standards for sulfur
- **calculate_blend_composition**: Determines the total mass and the weight percentage of each component in a proposed blend


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Diesel Blend Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the composition for a blend of 500kg of component A and 500kg of component B."

**🤖 AI Agent:**
> The total mass is 1000kg, with each component having a mass fraction of 0.5.

---

**👤 You:**
> "What is the sulfur content for a blend with a 0.8 mass fraction of a component having 15 ppm sulfur?"

**🤖 AI Agent:**
> The resulting sulfur content for that component contribution is 12 ppm.

---

**👤 You:**
> "Is a blend with 10 ppm sulfur compliant with USA regulations?"

**🤖 AI Agent:**
> Yes, a sulfur content of 10 ppm is compliant with the USA regulatory limit.


## ❓ FAQ

**Q: How does the tool handle additives?**
Additives are treated as distinct streams that can influence chemical properties like Cetane Index or improve cold flow properties like Cloud Point and CFPP.

**Q: Can I check if my blend meets EU regulations?**
Yes, you can use the `validate_regulatory_compliance` tool and specify 'Europe' as the target region to check sulfur limits.

**Q: What properties are calculated for cold flow?**
The engine calculates the Cloud Point, Pour Point, and Cold Filter Plugging Point (CFPP).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/diesel-blend-calculator](https://vinkius.com/en/ai-agent-connect/diesel-blend-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Diesel Blend Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `diesel-blend-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Diesel Blend Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "diesel-blend-calculator": {
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
