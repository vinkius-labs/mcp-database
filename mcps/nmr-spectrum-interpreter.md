# NMR Spectrum Interpreter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/nmr-spectrum-interpreter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Analyze NMR spectra to determine molecular structures.

## Description
This MCP server provides specialized tools for interpreting Nuclear Magnetic Resonance (NMR) spectroscopy data. It allows AI agents to analyze chemical shifts, integration values, and spin-spin coupling patterns to identify proton environments and propose molecular structures. Use `analyze_proton_environments` to categorize signals, `calculate_neighboring_protons` to interpret splitting, `identify_molecular_symmetry` to check for structural symmetry, and `suggest_molecular_structure` to find candidate molecular frameworks.


## Available Tools (4)
- **analyze_proton_environments**: Identify the specific chemical environments of protons based on provided spectral data
- **calculate_neighboring_protons**: Determine the number of neighboring protons for a specific signal based on its observed splitting
- **identify_molecular_symmetry**: Evaluate if a proposed set of proton environments is consistent with molecular symmetry
- **suggest_molecular_structure**: Propose potential molecular frameworks that satisfy all provided NMR constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NMR Spectrum Interpreter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these NMR signals: shifts [1.2, 3.5], integrations [3, 2], multiplicities ['triplet', 'quartet']."

**🤖 AI Agent:**
> The signals correspond to an ethyl group, with a methyl triplet at 1.2 ppm and a methylene quartet at 3.5 ppm.

---

**👤 You:**
> "How many neighbors does a doublet signal have?"

**🤖 AI Agent:**
> A doublet signal indicates that there is 1 neighboring proton.

---

**👤 You:**
> "Suggest a structure for a molecule with a singlet at 9.8 ppm (1H) and an aromatic multiplet at 7.2 ppm (5H)."

**🤖 AI Agent:**
> The data suggests benzaldehyde (C7H6O), featuring an aldehydic proton and a monosubstituted benzene ring.


## ❓ FAQ

**Q: How can I use this to identify a molecule?**
You can provide your spectral data to the `suggest_molecular_structure` tool to receive potential molecular candidates based on your shifts and coupling constants.

**Q: What data is required for analysis?**
To use `analyze_proton_environments`, you need to provide arrays for chemical shifts (ppm), integrations, and multiplicities.

**Q: Can it detect molecular symmetry?**
Yes, the `identify_molecular_symmetry` tool evaluates if your proton environments are consistent with a symmetric molecular structure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/nmr-spectrum-interpreter](https://vinkius.com/ai-agent-connect/nmr-spectrum-interpreter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NMR Spectrum Interpreter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nmr-spectrum-interpreter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NMR Spectrum Interpreter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nmr-spectrum-interpreter": {
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
