# Nanoparticle Synthesis Yield Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/nanoparticle-synthesis-yield-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Calculate yield, atom economy, and particle counts for nanoparticle synthesis.

## Description
This MCP server provides specialized chemical analysis tools for nanoparticle synthesis. It allows AI agents to perform precise mass balance calculations, determine limiting reactants using `get_stoichiometry_analysis`, and evaluate material recovery with `get_yield_metrics`. It also supports calculating particle populations via `get_particle_count` and analyzing reaction efficiency through `get_mass_balance_report`.


## Available Tools (4)
- **get_mass_balance_report**: Analyzes mass distribution during the reaction
- **get_particle_count**: Calculates the number of individual particles produced
- **get_stoichiometry_analysis**: Identifies the limiting reactant and theoretical mass limit
- **get_yield_metrics**: Calculates yield and efficiency of nanoparticle synthesis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nanoparticle Synthesis Yield Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the yield and atom economy for my synthesis using 5g of precursor A (molar mass 100) and 4g of product mass with 1g of ligand mass?"

**🤖 AI Agent:**
> The synthesis achieved a percentage yield of 85% and an atom economy of 92%.

---

**👤 You:**
> "How many particles were produced if I have 2mg of core mass and the radius is 10nm?"

**🤖 AI Agent:**
> The synthesis produced approximately 1.25e15 individual nanoparticles.

---

**👤 You:**
> "Identify the limiting reactant for precursors with masses [10, 5] and molar masses [50, 50] with a stoichiometric ratio of [1, 1]."

**🤖 AI Agent:**
> The limiting reactant is the second precursor (index 1).


## ❓ FAQ

**Q: How do I calculate the limiting reactant?**
You can use the `get_stoichiometry_analysis` tool by providing the precursor masses and their stoichiometric ratios.

**Q: Does this account for surfactants and ligands?**
Yes, tools like `get_yield_metrics` and `get_mass_balance_report` allow you to input ligand mass to ensure accurate mass balance.

**Q: Can I estimate the number of particles produced?**
Yes, use the `get_particle_count` tool with the core mass and the particle radius to find the total count.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/nanoparticle-synthesis-yield-analyzer](https://vinkius.com/ai-agent-connect/nanoparticle-synthesis-yield-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nanoparticle Synthesis Yield Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nanoparticle-synthesis-yield-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nanoparticle Synthesis Yield Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nanoparticle-synthesis-yield-analyzer": {
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
