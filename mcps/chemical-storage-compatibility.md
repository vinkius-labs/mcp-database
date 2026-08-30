# Chemical Storage Compatibility MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/chemical-storage-compatibility)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Determines safe chemical storage arrangements and segregation requirements.

## Description
This MCP server provides essential tools for laboratory and industrial safety by analyzing chemical inventories against hazard-based compatibility rules. It helps prevent hazardous reactions by calculating segregation needs, assigning chemicals to appropriate cabinets, and determining secondary containment requirements. Use `analyze_segregation_needs` to check for incompatible pairs, `assign_storage_cabinets` to organize inventory, `calculate_containment_requirements` for spill prevention, and `verify_storage_safety` to audit proposed arrangements.


## Available Tools (4)
- **analyze_segregation_needs**: Determines if a set of chemicals can be stored together or if they require physical separation
- **assign_storage_cabinets**: Groups chemicals into the most efficient and safe cabinet assignments
- **calculate_containment_requirements**: Determines the type and volume of secondary containment needed to prevent leaks from mixing
- **verify_storage_safety**: Provides a final safety audit of a proposed storage arrangement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chemical Storage Compatibility** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if these chemicals can be stored together: Sulfuric Acid (Acid) and Sodium Hydroxide (Base)."

**🤖 AI Agent:**
> No, these chemicals are incompatible. Sulfuric Acid and Sodium Hydroxide must be stored separately to prevent a violent neutralization reaction.

---

**👤 You:**
> "What containment is needed for 5L of Ethanol (Flammable) and 2L of Nitric Acid (Oxidizer)?"

**🤖 AI Agent:**
> You need secondary containment with a capacity of at least 5L. It is recommended to use separate trays for the Ethanol and the Nitric Acid to prevent them from mixing in the event of a leak.

---

**👤 You:**
> "Suggest cabinet assignments for an inventory containing Acetone (Flammable), Hydrochloric Acid (Acid), and Distilled Water (General)."

**🤖 AI Agent:**
> The recommended assignments are: Acetone in a Flammable Cabinet, Hydrochloric Acid in an Acid Cabinet, and Distilled Water on a General Shelf.


## ❓ FAQ

**Q: How does the tool determine if chemicals can be stored together?**
The `analyze_segregation_needs` tool compares the hazard classes of all chemicals in your inventory against a compatibility matrix to identify any conflicting pairs.

**Q: Can I use this to plan my cabinet layout?**
Yes, you can use `assign_storage_cabinets` to receive a recommended list of cabinet assignments based on the hazard classes of your chemicals.

**Q: What is the purpose of the safety audit tool?**
The `verify_storage_safety` tool performs a final check on a proposed arrangement to identify any safety violations or warnings before you finalize your storage setup.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/chemical-storage-compatibility](https://vinkius.com/ai-agent-connect/chemical-storage-compatibility)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chemical Storage Compatibility** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chemical-storage-compatibility` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chemical Storage Compatibility** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chemical-storage-compatibility": {
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
