# Steel Fire Protection Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/steel-fire-protection-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate required steel protection thickness and material consumption for fire safety.

## Description
This MCP server provides specialized engineering tools to ensure structural steel integrity during fire events. It allows users to determine the necessary insulation thickness using `get_section_factor` and `calculate_protection_thickness`. Additionally, it supports intumescent coating planning via `calculate_intumescent_specs` and project procurement estimation through `estimate_material_consumption`.


## Available Tools (4)
- **calculate_protection_thickness**: Determines the total thickness of insulation required to meet a specific fire rating
- **calculate_intumescent_specs**: Calculates the expansion-based thickness needed when using intumescent coatings
- **estimate_material_consumption**: Calculates the total volume of protection material needed for a project area
- **get_section_factor**: Provides the section factor for a specific steel geometry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steel Fire Protection Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the required protection thickness for an I-beam with a section factor of 150 for a 2-hour fire rating in an open environment at 550 degrees?"

**🤖 AI Agent:**
> The required protection thickness is 12.5 mm.

---

**👤 You:**
> "Calculate the material needed for 50 square meters of steel requiring 10mm of protection using intumescent coating."

**🤖 AI Agent:**
> The total volume required is 500 litres and the estimated weight is 650 kg.

---

**👤 You:**
> "I have an intumescent coating that needs to reach a target thickness of 15mm. What is the dry film thickness if the expansion ratio is 5?"

**🤖 AI Agent:**
> The required dry film thickness is 3 mm.


## ❓ FAQ

**Q: How do I determine the thickness needed for my steel beam?**
First, use `get_section_factor` to find the geometric vulnerability of your beam. Then, pass that value into `calculate_protection_thickness` along with your required fire rating and exposure type.

**Q: Can I calculate how much intumescent paint I need to buy?**
Yes. After calculating the required thickness, use `calculate_intumescent_specs` to find the dry film thickness, and then use `estimate_material_consumption` to get the total volume in litres.

**Q: What is a section factor?**
The section factor is a dimensionless value representing how quickly a specific steel shape will heat up during a fire based on its surface area relative to its mass.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/steel-fire-protection-calculator](https://vinkius.com/ai-agent-connect/steel-fire-protection-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steel Fire Protection Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steel-fire-protection-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steel Fire Protection Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steel-fire-protection-calculator": {
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
