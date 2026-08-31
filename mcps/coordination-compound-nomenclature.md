# Coordination Compound Nomenclature MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/coordination-compound-nomenclature)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Generate IUPAC names, formulas, and geometries for coordination complexes.

## Description
This MCP server provides specialized tools for inorganic chemistry. Use `generate_systematic_name` to obtain full IUPAC names, `derive_chemical_formula` for standard chemical formulas, `identify_geometry` to predict 3D shapes, and `analyze_isomers` to find structural or stereoisomers. It follows IUPAC Red Book guidelines for metal oxidation states, ligand naming, and bridging ligands.


## Available Tools (4)
- **analyze_isomers**: Identifies possible structural or stereoisomers for a given complex
- **derive_chemical_formula**: Converts the component parts into a standard chemical formula
- **generate_systematic_name**: Provides the full IUPAC name for a given coordination complex
- **identify_geometry**: Predicts the three-dimensional shape of the complex


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coordination Compound Nomenclature** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the IUPAC name for a complex with Cobalt(III) and six ammine ligands?"

**🤖 AI Agent:**
> hexaamminecobalt(III)

---

**👤 You:**
> "Give me the chemical formula for a complex with Platinum(II) and four chloride ligands."

**🤖 AI Agent:**
> [PtCl4]2-

---

**👤 You:**
> "What is the geometry of an octahedral complex with six water ligands and Iron(III)?"

**🤖 AI Agent:**
> Octahedral


## ❓ FAQ

**Q: Does this tool follow official IUPAC rules?**
Yes, the tools follow the IUPAC Red Book guidelines for naming and describing coordination compounds.

**Q: Can I identify the geometry of a complex?**
Yes, you can use the `identify_geometry` tool to predict the three-dimensional shape based on the metal and ligands provided.

**Q: How do I handle bridging ligands?**
When using `generate_systematic_name`, you can specify if the complex is bridged using the `is_bridged` parameter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/coordination-compound-nomenclature](https://vinkius.com/ai-agent-connect/coordination-compound-nomenclature)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coordination Compound Nomenclature** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coordination-compound-nomenclature` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coordination Compound Nomenclature** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coordination-compound-nomenclature": {
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
