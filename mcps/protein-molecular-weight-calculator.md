# Protein Molecular Weight Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/protein-molecular-weight-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [biochemistry](../categories/biochemistry.md)

Calculate protein mass, extinction coefficient, and isoelectric point from sequences or compositions.

## Description
This MCP server provides specialized biochemical tools for protein characterization. Use `calculate_sequence_properties` to derive a full suite of physical properties including molecular weight, UV absorption, and pI from a single-letter amino acid sequence. For mass calculations based on residue counts, use `calculate_composition_mass`. You can also isolate specific properties using `get_extinction_coefficient` for UV absorption at 280nm or `estimate_isoelectric_point` to find the neutral pH of a protein sequence. The tools account for post-translational modifications to ensure accurate biochemical modeling.


## Available Tools (4)
- **calculate_composition_mass**: Calculates the total molecular weight based only on the counts of each amino acid present
- **calculate_sequence_properties**: Calculates a full suite of physical properties for a specific protein sequence
- **estimate_isoelectric_point**: Estimates the pH at which the protein is electrically neutral
- **get_extinction_coefficient**: Determines the UV absorption capability of a protein at 280nm


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Protein Molecular Weight Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the molecular weight and pI of the sequence MKWVTFISLLFLFSSAYSRGVFRR?"

**🤖 AI Agent:**
> The protein has a molecular weight of approximately 2543.2 Da and an estimated isoelectric point of 5.2.

---

**👤 You:**
> "Calculate the mass for a composition of 10 Alanine (A) and 5 Glycine (G)."

**🤖 AI Agent:**
> The total molecular weight for this composition is 185.15 Da.

---

**👤 You:**
> "What is the extinction coefficient for the sequence WYYW?"

**🤖 AI Agent:**
> The molar extinction coefficient (ε280) for the sequence WYYW is 12450.5.


## ❓ FAQ

**Q: How do I calculate the mass of a protein using a composition?**
You can use the `calculate_composition_mass` tool by providing a JSON mapping of amino acid single-letter codes to their respective counts.

**Q: Can I include post-translational modifications in the calculation?**
Yes, both `calculate_sequence_properties` and `calculate_composition_mass` accept an optional modifications parameter to account for added mass.

**Q: What is the purpose of the extinction coefficient tool?**
The `get_extinction_coefficient` tool determines the UV absorption capability of a protein at 280nm based on its aromatic amino acid content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/protein-molecular-weight-calculator](https://vinkius.com/ai-agent-connect/protein-molecular-weight-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Protein Molecular Weight Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `protein-molecular-weight-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Protein Molecular Weight Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "protein-molecular-weight-calculator": {
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
