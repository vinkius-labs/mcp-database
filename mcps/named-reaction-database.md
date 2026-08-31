# Named Reaction Database MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/named-reaction-database)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

A specialized lookup service for organic named reactions, mechanisms, and substrate compatibility.

## Description
This MCP server provides organic chemists with a precise interface to query a comprehensive database of named reactions. It allows for deep exploration of chemical transformations, including detailed reaction mechanisms, typical reaction conditions, and substrate scope. Users can use `find_reaction_by_name` to retrieve core definitions, `search_reaction_by_transformation` to discover reactions based on functional group changes, `get_reaction_variations` to find modern improvements like new catalysts, and `analyze_substrate_compatibility` to evaluate if a specific molecule is suitable for a given reaction.


## Available Tools (4)
- **find_reaction_by_name**: Retrieves the core definition and fundamental details of a specific named reaction
- **analyze_substrate_compatibility**: Determines if a specific molecule is likely to be a successful substrate for a given reaction
- **get_reaction_variations**: Identifies specific modifications or modern improvements to a standard named reaction
- **search_reaction_by_transformation**: Finds reactions that achieve a specific structural change between reactants and products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Named Reaction Database** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the mechanism for the Diels-Alder reaction?"

**🤖 AI Agent:**
> The Diels-Alder reaction is a [4+2] cycloaddition between a conjugated diene and a substituted alkene (dienophile). The mechanism involves a concerted, pericyclic process where three pi bonds are broken and two new sigma bonds and one new pi bond are formed in a single step.

---

**👤 You:**
> "Find reactions that transform an alcohol into an aldehyde."

**🤖 AI Agent:**
> Common reactions for this transformation include the Swern oxidation, PCC (Pyridinium chlorochromate) oxidation, and Dess-Martin periodinane oxidation.

---

**👤 You:**
> "Is a molecule with a primary alcohol and a benzene ring compatible with the Wittig reaction?"

**🤖 AI Agent:**
> The Wittig reaction typically requires an aldehyde or ketone to react with a phosphonium ylide. A primary alcohol alone is not a direct substrate for the Wittig reaction; it would first need to be oxidized to an aldehyde.


## ❓ FAQ

**Q: How can I find reactions that convert one functional group to another?**
You can use the `search_reaction_by_transformation` tool by specifying the reactant type and the desired product type.

**Q: Can I check if a specific molecule will work with a reaction?**
Yes, use the `analyze_substrate_compatibility` tool. Provide the reaction name and a description of the molecule's functional groups.

**Q: Does this include modern variations of classic reactions?**
Yes, the `get_reaction_variations` tool allows you to find modern improvements, such as new catalysts or ligands, for established reactions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/named-reaction-database](https://vinkius.com/ai-agent-connect/named-reaction-database)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Named Reaction Database** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `named-reaction-database` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Named Reaction Database** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "named-reaction-database": {
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
