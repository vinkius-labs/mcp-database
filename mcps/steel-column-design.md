# Steel Column Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/steel-column-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Design steel columns for compression and combined loading using AISC standards.

## Description
This MCP server provides structural engineering tools to design steel columns. It calculates axial capacity, evaluates combined loading (axial and bending), recommends steel sections and bracing, and validates slenderness limits. Use `calculate_pure_compression_capacity` for axial loads, `evaluate_combined_loading` for moment checks, `recommend_section_and_bracing` for profile selection, and `validate_slenderness_limits` to ensure compliance with AISC buckling standards.


## Available Tools (4)
- **calculate_pure_compression_capacity**: Determines the maximum axial load a specific steel section can carry under pure compression
- **evaluate_combined_loading**: Checks if a column is safe when subjected to both axial compression and a bending moment
- **recommend_section_and_bracing**: Recommends an appropriate steel profile and specifies the necessary lateral bracing
- **validate_slenderness_limits**: Checks if a proposed column configuration meets the maximum allowable slenderness limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steel Column Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the maximum axial capacity for a column with 500kN load, 4m effective length, A992 steel, and a section with area 5000mm2 and radius of gyration 50mm?"

**🤖 AI Agent:**
> The maximum axial capacity for the specified A992 steel section is 425.5 kN.

---

**👤 You:**
> "Is a column safe with 200kN axial load, 15kNm bending moment, 5m length, A36 steel, and section properties (area: 4000, inertia: 20000000, modulus: 5000)?"

**🤖 AI Agent:**
> Yes, the interaction ratio is 0.72, which is below the 1.0 limit, so the column is safe.

---

**👤 You:**
> "Recommend a section for 1000kN axial load, 6m length, A992 steel, and a pinned connection."

**🤖 AI Agent:**
> The recommended section is W14x90 with a bracing interval of 4.5 meters.


## ❓ FAQ

**Q: What standards does this tool follow?**
The tools follow AISC (American Institute of Steel Construction) standards for column design and interaction equations.

**Q: Can I check for combined loading?**
Yes, you can use `evaluate_combined_loading` to check if a column is safe under both axial compression and bending moments.

**Q: How do I get a section recommendation?**
Use the `recommend_section_and_bracing` tool by providing the axial load, effective length, steel grade, and connection type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/steel-column-design](https://vinkius.com/ai-agent-connect/steel-column-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steel Column Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steel-column-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steel Column Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steel-column-design": {
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
