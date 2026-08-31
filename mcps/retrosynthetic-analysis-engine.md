# Retrosynthetic Analysis Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/retrosynthetic-analysis-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Deconstruct complex molecules into simpler precursors using strategic disconnection analysis.

## Description
This MCP server provides a complete suite of tools for chemical retrosynthesis. It allows AI agents to perform strategic bond disconnections, identify theoretical synthons, map synthons to real-world synthetic equivalents, and construct full hierarchical route trees. By using `analyze_disconnections`, agents can find optimal breaking points, while `generate_route_tree` provides a complete map from the target molecule down to available starting materials.


## Available Tools (4)
- **analyze_disconnections**: Identifies the most logical points to break the target molecule to simplify its structure
- **generate_route_tree**: Constructs a complete hierarchical map of the synthetic pathways from the target down to available precursors
- **identify_synthons**: Converts the identified strategic bond breaks into theoretical chemical fragments
- **map_synthetic_equivalents**: Suggests real-world chemical reagents that can perform the function of the theoretical synthons


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Retrosynthetic Analysis Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the best strategic bonds to break for the molecule C1=CC=CC=C1."

**🤖 AI Agent:**
> The strategic bonds for benzene (C1=CC=CC=C1) have been identified with a complexity reduction score of 0.5.

---

**👤 You:**
> "What are the synthetic equivalents for these synthons: [{"formula": "CH3+", "charge": 1, "type": "carbocation"}]?"

**🤖 AI Agent:**
> The suggested reagent for the methyl cation synthon is Methyl Iodide (CH3I).

---

**👤 You:**
> "Generate a route tree for the target molecule CC(=O)C."

**🤖 AI Agent:**
> The synthetic route tree for acetone (CC(=O)C) has been generated, showing pathways to simple precursors.


## ❓ FAQ

**Q: What kind of molecular structures can I analyze?**
You can analyze molecules provided in SMILES or IUPAC format using the `analyze_disconnections` tool.

**Q: How does the tool suggest reagents?**
The `map_synthetic_equivalents` tool maps theoretical synthons to stable, commercially available chemical reagents.

**Q: Can I see the full synthesis pathway?**
Yes, the `generate_route_tree` tool constructs a hierarchical map of pathways from the target to starting materials.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/retrosynthetic-analysis-engine](https://vinkius.com/ai-agent-connect/retrosynthetic-analysis-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Retrosynthetic Analysis Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `retrosynthetic-analysis-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Retrosynthetic Analysis Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "retrosynthetic-analysis-engine": {
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
