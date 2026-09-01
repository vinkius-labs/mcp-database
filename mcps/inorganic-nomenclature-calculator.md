# Inorganic Nomenclature Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/inorganic-nomenclature-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Converts chemical formulas into IUPAC systematic names, common names, and validated formulas.

## Description
This MCP server provides precise chemical identification tools for inorganic compounds. It allows AI agents to determine the formal IUPAC systematic name using `get_systematic_name`, retrieve widely recognized traditional names via `get_common_name`, and obtain properly formatted chemical formulas with `get_validated_formula`. It also categorizes substances into families like Salts, Oxoacids, or Coordination Compounds using `identify_compound_class`.


## Available Tools (4)
- **get_common_name**: Retrieves the widely recognized traditional name for a compound
- **get_systematic_name**: Provides the formal, rule-based IUPAC name for a given chemical entity
- **get_validated_formula**: Returns the correctly formatted chemical formula
- **identify_compound_class**: Categorizes the compound into its specific chemical family


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Inorganic Nomenclature Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the IUPAC name for Fe2O3?"

**🤖 AI Agent:**
> The systematic IUPAC name for Fe2O3 is iron(III) oxide.

---

**👤 You:**
> "Give me the common name for NaCl."

**🤖 AI Agent:**
> The common name for NaCl is sodium chloride.

---

**👤 You:**
> "What type of compound is H2SO4?"

**🤖 AI Agent:**
> H2SO4 is classified as an Oxoacid.


## ❓ FAQ

**Q: Can I use this for coordination compounds?**
Yes, the `identify_compound_class` tool can detect coordination compounds, and `get_systematic_name` provides the correct IUPAC naming for complex structures.

**Q: Does it support common names?**
Yes, you can use `get_common_name` to find traditional names like 'Soda ash' for Sodium carbonate.

**Q: How are formulas formatted?**
The `get_validated_formula` tool ensures all element symbols follow standard capitalization and proper stoichiometry.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/inorganic-nomenclature-calculator](https://vinkius.com/ai-agent-connect/inorganic-nomenclature-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Inorganic Nomenclature Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `inorganic-nomenclature-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Inorganic Nomenclature Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "inorganic-nomenclature-calculator": {
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
