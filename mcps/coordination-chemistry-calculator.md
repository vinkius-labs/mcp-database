# Coordination Chemistry Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/coordination-chemistry-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Calculate oxidation states, d-electron counts, and CFSE for coordination complexes.

## Description
This MCP server provides specialized tools for analyzing coordination compounds. It allows AI agents to determine the fundamental identity of a complex using `calculate_basic_properties`, identify electronic configurations via `calculate_electron_configuration`, and quantify stabilization energy with `calculate_cfse`. For a complete technical profile, use `get_complex_summary` to aggregate all properties including oxidation state, coordination number, d-electron count, spin state, and CFSE.


## Available Tools (4)
- **calculate_cfse**: Quantifies the Crystal Field Stabilization Energy
- **calculate_electron_configuration**: Calculates the remaining d-electrons and identifies the spin state
- **get_complex_summary**: Provides a human-readable technical profile of the coordination compound
- **calculate_basic_properties**: Determines the fundamental identity of the complex (oxidation state and coordination number)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coordination Chemistry Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the oxidation state and coordination number of a complex with Iron(III) and three cyanide ligands with a net charge of 0?"

**🤖 AI Agent:**
> The oxidation state of Iron is +3 and the coordination number is 6.

---

**👤 You:**
> "Calculate the CFSE for an octahedral complex with 3 d-electrons in a high-spin state where Δ is 20,000 cm⁻¹."

**🤖 AI Agent:**
> The total CFSE is 6000 cm⁻¹.

---

**👤 You:**
> "Give me a summary for a complex with Cobalt, two ethylenediamine ligands, and a charge of +2 in an octahedral geometry."

**🤖 AI Agent:**
> The complex has Cobalt as the metal, an oxidation state of +2, a coordination number of 4, a d-electron count of 7, a high-spin state, and a calculated CFSE.


## ❓ FAQ

**Q: What can I calculate with this tool?**
You can calculate the oxidation state, coordination number, d-electron count, spin state, and Crystal Field Stabilization Energy (CFSE) for various coordination complexes.

**Q: How do I get a full report of a complex?**
Use the `get_complex_summary` tool to receive a complete technical profile of the coordination compound in one go.

**Q: Does it support different geometries?**
Yes, the tools account for different spatial arrangements like octahedral and tetrahedral geometries to determine splitting and spin states.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/coordination-chemistry-calculator](https://vinkius.com/ai-agent-connect/coordination-chemistry-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coordination Chemistry Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coordination-chemistry-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coordination Chemistry Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coordination-chemistry-calculator": {
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
