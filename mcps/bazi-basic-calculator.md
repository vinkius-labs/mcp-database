# BaZi Basic Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bazi-basic-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Calculate the Four Pillars of Destiny (BaZi) using birth date and time.

## Description
This MCP server provides tools to calculate the Four Pillars of Destiny (BaZi). Use `calculate_four_pillars` to derive the Heavenly Stems and Earthly Branches for a specific birth date. You can also use `identify_elemental_interaction` to understand how elements interact, or `lookup_component_properties` to find the element and polarity of any Stem or Branch.


## Available Tools
- **calculate_four_pillars**: Derive the complete Four Pillars (Stem and Branch for each) from a specific birth date and time
- **lookup_component_properties**: Find the elemental nature and polarity of a specific Heavenly Stem or Earthly Branch
- **identify_elemental_interaction**: Determine the relationship between two different elemental components


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BaZi Basic Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Four Pillars for someone born on June 15, 1990, at 14:30."

**🤖 AI Agent:**
> The calculation for June 15, 1990, at 14:30 resulted in the following pillars...

---

**👤 You:**
> "What is the relationship between Wood and Water?"

**🤖 AI Agent:**
> Water generates Wood, representing a productive interaction.

---

**👤 You:**
> "What is the polarity of the 'Dragon' branch?"

**🤖 AI Agent:**
> The Dragon (Chen) branch has the element Earth and a Yang polarity.


## ❓ FAQ

**Q: What is the Four Pillars of Destiny?**
It is a traditional system that analyzes an individual's destiny by dividing their birth moment into four pillars: Year, Month, Day, and Hour.

**Q: How do I use the `calculate_four_pillars` tool?**
Provide the year, month, day, and hour of birth in Gregorian format to get the corresponding Heavenly Stems and Earthly Branches.

**Q: Can I check elemental relationships?**
Yes, use the `identify_elemental_interaction` tool to see if one element generates or overcomes another.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bazi-basic-calculator](https://vinkius.com/mcp/bazi-basic-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BaZi Basic Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bazi-basic-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BaZi Basic Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bazi-basic-calculator": {
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
