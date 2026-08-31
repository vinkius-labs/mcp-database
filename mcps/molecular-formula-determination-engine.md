# Molecular Formula Determination Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/molecular-formula-determination-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

A precision engine for calculating empirical formulas, molecular formulas, and degree of unsaturation.

## Description
This MCP server provides high-precision stoichiometric calculations for chemical analysis. It allows AI agents to determine the simplest whole-number ratios of elements using `find_empirical_formula`, derive actual molecular formulas from empirical data with `calculate_molecular_formula`, and calculate the degree of unsaturation using `calculate_unsaturation`. It also supports converting mass percentages directly into formulas via `derive_from_composition`. These tools are essential for researchers and students working with mass spectrometry data and elemental composition analysis.


## Available Tools (4)
- **calculate_molecular_formula**: Derives the actual molecular formula from the empirical formula and known mass data
- **calculate_unsaturation**: g., "C6H12O6").

Determines the degree of unsaturation for a given molecular formula
- **derive_from_composition**: Converts mass percentages into a molecular formula
- **find_empirical_formula**: Determines the simplest whole-number ratio of elements from their masses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Molecular Formula Determination Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the molecular formula if the empirical formula is CH2 and the molar mass is 42 g/mol?"

**🤖 AI Agent:**
> The molecular formula is C3H6.

---

**👤 You:**
> "Find the empirical formula for a compound with 40% Carbon, 6.7% Hydrogen, and 53.3% Oxygen."

**🤖 AI Agent:**
> The empirical formula is CH2O.

---

**👤 You:**
> "What is the degree of unsaturation for C6H12O6?"

**🤖 AI Agent:**
> The degree of unsaturation for C6H12O6 is 1.


## ❓ FAQ

**Q: How do I calculate the molecular formula?**
You can use the `calculate_molecular_formula` tool by providing the empirical formula and the target molar mass.

**Q: Can I use mass spectrometry data?**
Yes, the `calculate_molecular_formula` tool accepts an optional `msMassData` parameter to refine the molar mass using the molecular ion peak.

**Q: What is the degree of unsaturation?**
The degree of unsaturation represents the total number of rings and pi bonds in a molecule, which can be found using `calculate_unsaturation`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/molecular-formula-determination-engine](https://vinkius.com/ai-agent-connect/molecular-formula-determination-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Molecular Formula Determination Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `molecular-formula-determination-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Molecular Formula Determination Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "molecular-formula-determination-engine": {
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
