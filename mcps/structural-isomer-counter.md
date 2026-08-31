# Structural Isomer Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/structural-isomer-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Identify and count constitutional isomers for organic molecular formulas.

## Description
This MCP server provides specialized tools for organic chemistry analysis. It allows AI agents to determine the total number of unique constitutional isomers for a given molecular formula using `get_isomer_count`. Users can retrieve detailed structural information, including IUPAC names and condensed formulas, via `list_isomer_details`. The server also categorizes isomers into chain, position, or functional groups using `get_isomer_classification`, and ensures chemical validity with `validate_formula_feasibility`.


## Available Tools (4)
- **get_isomer_classification**: Segregates isomers into groups based on their specific type of structural isomerism
- **get_isomer_count**: Determines the total number of unique constitutional isomers for a given molecular formula
- **list_isomer_details**: Provides a detailed breakdown of every isomer, including its structure and systematic name
- **validate_formula_feasibility**: Checks if a molecular formula can actually form stable organic structures based on standard valence rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Structural Isomer Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many isomers are there for C3H8O?"

**🤖 AI Agent:**
> There are 3 constitutional isomers for C3H8O: propan-1-ol, propan-2-ol, and methoxyethane.

---

**👤 You:**
> "List the details for C2H6O."

**🤖 AI Agent:**
> The isomers for C2H6O are ethanol (CH3CH2OH) and dimethyl ether (CH3OCH3).

---

**👤 You:**
> "Is C10H30 a valid molecular formula?"

**🤖 AI Agent:**
> No, C10H30 is not a valid formula because the hydrogen count exceeds the maximum capacity for 10 carbon atoms.


## ❓ FAQ

**Q: What types of isomers are supported?**
The tool identifies constitutional isomers, specifically covering chain, position, and functional group isomers.

**Q: How can I check if a formula is valid?**
You can use the `validate_formula_feasibility` tool to check if a molecular formula follows standard organic valence rules.

**Q: Does it provide IUPAC names?**
Yes, `list_isomer_details` provides the official IUPAC name for every identified isomer.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/structural-isomer-counter](https://vinkius.com/ai-agent-connect/structural-isomer-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Structural Isomer Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `structural-isomer-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Structural Isomer Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "structural-isomer-counter": {
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
