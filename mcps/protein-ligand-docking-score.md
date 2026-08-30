# Protein-Ligand Docking Score MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/protein-ligand-docking-score)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Evaluates protein-ligand binding affinity and interaction characteristics from docking poses.

## Description
This MCP server provides specialized tools for analyzing the thermodynamic stability and chemical interactions of protein-ligand complexes. Use `get_binding_energy` to calculate total affinity, including solvation and entropy effects. Use `analyze_interactions` to identify specific chemical bonds like Hydrogen Bonds or Salt Bridges. You can also use `identify_binding_site` to map contact residues or `compare_poses` to rank multiple docking configurations for the most stable binding mode.


## Available Tools (4)
- **analyze_interactions**: Identifies and categorizes the types of chemical bonds formed between the ligand and the protein
- **compare_poses**: Compares multiple docking configurations to find the most stable binding mode
- **get_binding_energy**: Calculates the total estimated binding affinity for a specific docking pose
- **identify_binding_site**: Maps the specific protein residues that are in immediate proximity to the ligand


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Protein-Ligand Docking Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the binding energy for pose 'pose_001' including solvation?"

**🤖 AI Agent:**
> The total binding energy for pose 'pose_001' is -8.4 kcal/mol, which includes a solvation contribution of -1.2 kcal/mol.

---

**👤 You:**
> "Which residues are in contact with the ligand in pose 'pose_abc'?"

**🤖 AI Agent:**
> The ligand is in contact with residues HIS-42, TRP-105, and ASP-12 in pose 'pose_abc'.

---

**👤 You:**
> "Compare the stability of poses 'p1', 'p2', and 'p3'."

**🤖 AI Agent:**
> The best pose is 'p2' with a binding energy of -9.2 kcal/mol. The energy difference between 'p2' and the next best pose is 0.5 kcal/mol.


## ❓ FAQ

**Q: How do I calculate the total binding affinity?**
You can use the `get_binding_energy` tool by providing a valid `poseId`. You can also optionally include solvation and entropy effects in the calculation.

**Q: Can I see which amino acids are interacting with my ligand?**
Yes, the `identify_binding_site` tool maps the specific protein residues in immediate proximity to the ligand based on a distance threshold.

**Q: How can I find the most stable docking configuration?**
Use the `compare_poses` tool with a list of `poseIds` to rank multiple configurations and identify the best binding mode.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/protein-ligand-docking-score](https://vinkius.com/ai-agent-connect/protein-ligand-docking-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Protein-Ligand Docking Score** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `protein-ligand-docking-score` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Protein-Ligand Docking Score** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "protein-ligand-docking-score": {
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
