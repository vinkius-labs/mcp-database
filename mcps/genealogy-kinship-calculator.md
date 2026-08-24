# Genealogy Kinship Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/genealogy-kinship-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analysis](../categories/data-analysis.md)

Calculate exact kinship terms, civil law degrees, and biological coefficients.

## Description
This MCP server provides high-precision genealogical analysis. Use `get_kinship_details` to determine exact English kinship terms like 'second cousin once removed', or `find_common_ancestors` to identify shared biological lineage. It also includes `validate_tree_integrity` to ensure family structures are logically sound and free of circularities.


## Available Tools (3)
- **find_common_ancestors**: Identifies all shared biological ancestors between two individuals
- **get_kinship_details**: Provides the complete kinship profile between two specific individuals
- **validate_tree_integrity**: Ensures the provided family tree structure is logically sound


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Genealogy Kinship Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the relationship between person_001 and person_005 in this tree?"

**🤖 AI Agent:**
> The relationship is 'first cousin once removed'.

---

**👤 You:**
> "Find the common ancestors for person_A and person_B."

**🤖 AI Agent:**
> The common ancestors are person_Z (distance 2 to A, distance 3 to B) and person_Y (distance 3 to A, distance 4 to B).

---

**👤 You:**
> "Is this family tree valid?"

**🤖 AI Agent:**
> The tree is valid and contains no circularities or impossible biological links.


## ❓ FAQ

**Q: How does the tool calculate the kinship term?**
The engine uses deterministic algorithms to analyze the path between individuals, accounting for consanguinity, affinity, and generational distance to provide exact terms.

**Q: Can I find common ancestors between two people?**
Yes, you can use the `find_common_ancestors` tool to identify all shared biological ancestors and their distance from each individual.

**Q: What is the difference between consanguinity and affinity?**
Consanguinity refers to biological blood relations, while affinity refers to relations established through marriage or legal unions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/genealogy-kinship-calculator](https://vinkius.com/ai-agent-connect/genealogy-kinship-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Genealogy Kinship Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `genealogy-kinship-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Genealogy Kinship Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "genealogy-kinship-calculator": {
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
