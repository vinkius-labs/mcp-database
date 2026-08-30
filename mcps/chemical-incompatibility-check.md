# Chemical Incompatibility Check MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/chemical-incompatibility-check)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Predict hazardous chemical reactions and determine storage segregation requirements.

## Description
This MCP server provides critical safety intelligence for chemical management. It allows AI agents to identify hazardous interactions between substances using `check_pair_compatibility` and `analyze_storage_group`. Users can also retrieve specific storage instructions via `get_segregation_recommendations` and understand chemical properties through `identify_reactive_groups`. It is designed to prevent dangerous reactions in laboratories and warehouses by enforcing proper segregation based on reactive groups.


## Available Tools (4)
- **analyze_storage_group**: Evaluates a collection of chemicals to identify any internal incompatibilities
- **check_pair_compatibility**: Determines if two specific chemicals can be safely stored or handled together
- **get_segregation_recommendations**: Provides specific storage instructions based on a chemical's reactive group
- **identify_reactive_groups**: Explains the chemical properties and reactive characteristics of a specific substance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chemical Incompatibility Check** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are Sodium Chloride and Hydrochloric Acid safe to store together?"

**🤖 AI Agent:**
> Yes, Sodium Chloride and Hydrochloric Acid are compatible for storage.

---

**👤 You:**
> "Check if this list of chemicals is safe for a single cabinet: Acetone, Nitric Acid, Ethanol."

**🤖 AI Agent:**
> The storage plan is unsafe. Nitric Acid is incompatible with Acetone and Ethanol, posing a high risk of exothermic reaction.

---

**👤 You:**
> "What are the storage requirements for Sulfuric Acid in a warehouse?"

**🤖 AI Agent:**
> Sulfuric Acid should be stored in a Corrosive Cabinet. It requires secondary containment and must be kept away from strong bases and organic materials.


## ❓ FAQ

**Q: How do I check if two chemicals are safe to store together?**
You can use the `check_pair_compatibility` tool to determine if a specific pair of chemicals is compatible and what the hazard level is.

**Q: Can I check an entire storage cabinet at once?**
Yes, the `analyze_storage_group` tool evaluates a list of chemicals to identify any internal incompatibilities within a proposed storage area.

**Q: What kind of storage advice does it provide?**
By using `get_segregation_recommendations`, you receive specific storage classes and directives, such as whether secondary containment is required.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/chemical-incompatibility-check](https://vinkius.com/ai-agent-connect/chemical-incompatibility-check)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chemical Incompatibility Check** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chemical-incompatibility-check` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chemical Incompatibility Check** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chemical-incompatibility-check": {
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
