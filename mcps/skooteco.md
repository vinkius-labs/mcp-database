# SkootEco MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/skooteco)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Connect your AI agents to SkootEco to track carbon emissions, purchase offsets, plant trees, and generate ESG compliance reports.

## Description
Take control of your corporate sustainability targets by connecting SkootEco to your AI agents. With 18 specialized environmental tools, your AI can programmatically log emissions across all GHG scopes, purchase certified carbon offsets, track reforestation projects, and dynamically generate compliance reports.

### What you can do
- Track direct and indirect emissions (GHG Scope 1, 2, 3)
- Automatically calculate supply chain carbon footprint
- Purchase certified carbon offset credits programmatically
- Fund reforestation projects and track your tree count
- Publish your public sustainability impact profile
- Generate CSRD and TCFD-aligned ESG reports

### How it works
1. Subscribe to this server
2. Enter your SkootEco API Key (found in your provider dashboard)
3. Let your AI seamlessly manage your carbon compliance directly via Vinkius

### Who is it for?
Crucial for ESG managers, sustainability officers, and environmentally conscious businesses looking to accurately track, offset, and report on their carbon emissions.


## Available Tools
- **add_emission**: Log an emission
- **check_skooteco_status**: Verify connectivity
- **get_account**: Get account info
- **get_esg_report**: Get ESG report
- **get_emissions_by_category**: Get emissions by category
- **get_emissions_by_scope**: Get emissions by scope
- **get_emissions**: Get total emissions
- **get_impact_profile**: Get impact profile
- **get_metrics**: Get impact metrics
- **get_offset**: Get offset details
- **get_project**: Get project details
- **get_report**: Get summary report
- **get_tree_count**: Get tree count
- **list_categories**: List emission categories
- **list_offsets**: List carbon offsets
- **list_projects**: List climate projects
- **plant_tree**: Plant a tree
- **purchase_offset**: Purchase carbon offset


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SkootEco** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show my Scope 3 supply chain emissions in SkootEco."

**🤖 AI Agent:**
> I've retrieved your emissions data. Your Scope 3 supply chain emissions for this quarter are currently at 45.2 metric tons of CO2e. This represents a 12% decrease compared to the previous quarter. Would you like a detailed breakdown by vendor?

---

**👤 You:**
> "Plant 100 trees through SkootEco to offset our Q1 travel emissions."

**🤖 AI Agent:**
> Success! I've initiated the planting of 100 trees through your SkootEco account. This brings your company's total planted trees to 2,450. You can expect a digital certificate of this impact in your inbox shortly.

---

**👤 You:**
> "Generate our ESG compliance report from SkootEco for the board meeting."

**🤖 AI Agent:**
> I've generated your latest ESG compliance report. The document is aligned with CSRD and TCFD frameworks and highlights your recent 15% reduction in overall carbon footprint. Should I email this PDF directly to the board members?


## ❓ FAQ

**Q: How can my AI retrieve a breakdown of our emissions by scope?**
Simply use the `get_emissions_by_scope` tool. Your agent will instantly fetch data categorized by GHG Scope 1 (direct emissions), Scope 2 (energy), or Scope 3 (supply chain), perfectly aligned with the GHG Protocol.

**Q: Is it possible to automatically fund reforestation projects?**
Yes. By executing the `plant_trees` action, your AI agent can programmatically fund tree planting projects to offset emissions, and return the updated total tree count in real time.

**Q: Can I automatically generate ESG compliance reports for stakeholders?**
Absolutely. Ask the agent to use the `generate_esg_report` tool. It will compile your sustainability data into compliance reports aligned with CSRD and TCFD frameworks, ready for your next board meeting.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/skooteco](https://vinkius.com/mcp/skooteco)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SkootEco** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `skooteco` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SkootEco** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "skooteco": {
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
