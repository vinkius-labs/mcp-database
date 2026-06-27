# Footing Size Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/footing-size-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate minimum square footing dimensions and thickness based on column load and soil bearing capacity.

## Description
The Footing Size Calculator is a structural engineering tool designed to determine the required width and thickness for square concrete footings. By providing the axial column load in kips and the allowable soil bearing capacity in ksf, users can instantly find the minimum footing dimensions needed to prevent structural failure or excessive settlement. The server includes specialized tools such as `retrieve_soil_capacity` for quick geotechnical lookups, `calculate_footing_dimensions` for precise geometry calculation, and `validate_engineering_params` to ensure all inputs remain within safe engineering bounds.


## Available Tools (3)
- **calculate_footing_dimensions**: Determines the minimum width and thickness required for a square footing
- **validate_engineering_params**: Verifies that input engineering parameters are within realistic and safe operational bounds
- **retrieve_soil_capacity**: Clay, Sand, Gravel) and returns its capacity in ksf.

Provides the standardized allowable bearing capacity for a known soil type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Footing Size Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the bearing capacity for Sand?"

**🤖 AI Agent:**
> The allowable bearing capacity for Sand is 2.0 ksf.

---

**👤 You:**
> "Calculate the footing size for a load of 500 kips and a soil capacity of 3.0 ksf."

**🤖 AI Agent:**
> For a load of 500 kips and 3.0 ksf capacity, the minimum required footing width is 12.91 ft and the thickness is 1.29 ft.

---

**👤 You:**
> "Is a column load of 15000 kips valid?"

**🤖 AI Agent:**
> No, the load of 15000 kips exceeds the safety threshold of 10,000 kips and may be an error.


## ❓ FAQ

**Q: What inputs are required for the calculation?**
You need to provide the column load in kips and the allowable soil bearing capacity in ksf.

**Q: How can I find the bearing capacity for different soil types?**
You can use the `retrieve_soil_capacity` tool to look up standardized values for Clay, Sand, and Gravel.

**Q: What happens if my input parameters are too high?**
The `validate_engineering_params` tool will flag any load exceeding 10,000 kips or capacity exceeding 20 ksf as potentially erroneous.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/footing-size-calculator](https://vinkius.com/mcp/footing-size-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Footing Size Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `footing-size-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Footing Size Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "footing-size-calculator": {
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
