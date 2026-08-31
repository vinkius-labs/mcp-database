# Organic Compound Nomenclature MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/organic-compound-nomenclature)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Precise IUPAC naming and chemical property analysis for organic molecules.

## Description
This MCP server provides a professional-grade engine for organic chemistry analysis. It allows AI agents to translate molecular structures or common names into precise IUPAC systematic names using the `get_systematic_name` tool. Users can identify compounds via `identify_compound`, retrieve fundamental chemical properties like molecular formulas and mass with `get_molecular_details`, and discover constitutional isomers using `find_structural_isomers`. It is designed to handle functional groups, stereochemistry, and complex substituents accurately.


## Available Tools (4)
- **find_structural_isomers**: Identifies and lists the unique structural isomers for a given molecular formula
- **get_molecular_details**: Provides the fundamental chemical properties of the molecule
- **get_systematic_name**: Generates the precise IUPAC name for a given compound
- **identify_compound**: Converts a provided molecular structure or a common name into a standardized internal representation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Organic Compound Nomenclature** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the IUPAC name for the SMILES string CCO?"

**🤖 AI Agent:**
> The IUPAC name for the compound with SMILES CCO is ethanol.

---

**👤 You:**
> "Find the molecular formula for benzene."

**🤖 AI Agent:**
> The molecular formula for benzene is C6H6.

---

**👤 You:**
> "Identify the compound from the common name 'Acetone'."

**🤖 AI Agent:**
> The compound Acetone is identified as propan-2-one with the SMILES string CC(=O)C.


## ❓ FAQ

**Q: What kind of molecular inputs does the server accept?**
The server accepts SMILES strings, molecular structure representations, or well-known common names through the `identify_compound` tool.

**Q: Can I get the IUPAC name including stereochemistry?**
Yes, by using the `get_systematic_name` tool and setting the includeStereochemistry parameter to true, you can receive names with R/S or E/Z descriptors.

**Q: Does it support finding isomers?**
Yes, the `find_structural_isomers` tool identifies unique structural isomers for a given molecular formula.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/organic-compound-nomenclature](https://vinkius.com/ai-agent-connect/organic-compound-nomenclature)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Organic Compound Nomenclature** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `organic-compound-nomenclature` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Organic Compound Nomenclature** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "organic-compound-nomenclature": {
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
