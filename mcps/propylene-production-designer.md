# Propylene Production Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/propylene-production-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering design tool for modeling on-purpose propylene production pathways.

## Description
This MCP server provides specialized engineering tools to design propylene production facilities. It allows users to model different chemical pathways including Propane Dehydrogenation (PDH), Methanol to Olefins (MTO), and Metathesis. Use `calculate_reactor_specs` to determine physical vessel requirements, `design_catalyst_system` to specify catalyst mass and type, and `estimate_propylene_yield` to calculate output efficiency. You can also use `validate_process_feasibility` to audit if a specific feedstock and technology combination is chemically viable.


## Available Tools (4)
- **design_catalyst_system**: Specifies the necessary catalyst mass and type to support the production capacity
- **calculate_reactor_specs**: Determines the physical requirements and operational parameters of the reactor based on the chosen technology
- **estimate_propylene_yield**: Calculates the expected output efficiency of the plant
- **validate_process_feasibility**: An audit tool to check if the combination of feedstock, technology, and capacity is chemically and economically viable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Propylene Production Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reactor specifications for a PDH plant with a capacity of 50000 metric tons using propane."

**🤖 AI Agent:**
> The reactor for your PDH plant requires a volume of 1250 m³, a thermal load of 450 MW, an operating temperature of 620°C, and a pressure of 1.5 bar.

---

**👤 You:**
> "What is the expected propylene yield for an MTO process with 10000 tons of methanol?"

**🤖 AI Agent:**
> The expected propylene yield is 4200 metric tons, with a conversion rate of 42% and a byproduct profile primarily consisting of ethylene.

---

**👤 You:**
> "Is it feasible to use ethylene for a metathesis process with a capacity of 20000 tons?"

**🤖 AI Agent:**
> Yes, the process is viable with a low risk level, provided the stoichiometric availability of the olefin feedstock is maintained.


## ❓ FAQ

**Q: What technologies are supported?**
The server supports Propane Dehydrogenation (PDH), Methanol to Olefins (MTO), and Metathesis pathways.

**Q: How do I check if my design is viable?**
You can use the `validate_process_feasibility` tool to check if your chosen feedstock, technology, and capacity combination is chemically and economically viable.

**Q: Can I calculate reactor volume?**
Yes, the `calculate_reactor_specs` tool provides reactor volume, thermal load, operating temperature, and pressure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/propylene-production-designer](https://vinkius.com/en/ai-agent-connect/propylene-production-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Propylene Production Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `propylene-production-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Propylene Production Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "propylene-production-designer": {
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
