# InnoVint MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/innovint)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage wine production, lots, vessels, lab analyses, and cellar actions for your InnoVint winery through natural conversation.

## Description
Connect your **InnoVint** winery to any AI agent and transform how your cellar team works — from harvest intake to bottling.

### What you can do

- **Lots** — Search and track wine lots by varietal, vintage, lot code, or vessel assignment
- **Vessels** — Monitor tanks, barrels, concrete eggs, and amphorae — capacity, fill level, and contents
- **Lab Analyses** — View pH, TA, SO2, Brix, RS, VA, and alcohol readings for any lot over time
- **Cellar Actions** — Track rackings, pump-overs, punchdowns, additions, fining, and filtration history
- **Wines & Vintages** — Browse wine products and navigate production by vintage year
- **Additives** — Reference registered chemicals, enzymes, and fining agents with dosage guidelines
- **Multi-Winery** — Manage multiple wineries from a single AI connection

### Who is this for?

- **Enologists** — Instant lab data and fermentation tracking while walking the vineyard
- **Winemakers** — Blend decisions, barrel aging, and lot management by voice
- **Cellar Masters** — Tank availability, vessel contents, and space planning
- **Vineyard Owners** — Production overview, vintage comparison, and quality metrics


## Available Tools
- **search_lots**: Returns lot details including volume, vessel assignment, varietal composition, and current status. Essential for tracking individual batches through the winemaking process — from harvest intake to bottling.

Search wine lots
- **list_wineries**: Multi-winery operations can manage several facilities from one account.

List wineries
- **get_lot**: The primary data point for any winemaking question.

Get full lot details
- **list_vessels**: Shows capacity, current contents, fill level, and location. Critical for cellar management and space planning.

List tanks and barrels
- **get_vessel**: Essential for barrel program management.

Get vessel details
- **list_wines**: Each with varietal rules, appellation, and production notes.

List wine products
- **list_vintages**: Navigate wine production by year.

List vintages
- **list_analyses**: Filter by lot to see a specific wine's chemistry over time.

List lab analyses
- **list_actions**: Filter by lot to see complete cellar history.

List cellar actions
- **list_additives**: With regulatory limits and typical dosage.

List additives


## 💬 Prompt Examples

Here are some examples of how you can interact with the **InnoVint** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How is the 2025 Pinot Noir fermentation going?"

**🤖 AI Agent:**
> 🍷 **Pinot Noir 2025 — Lot PN-25-01**

🧪 Latest lab analysis (Oct 14):
- **pH**: 3.48 (within range)
- **Brix**: 0.2° (fermentation nearly complete)
- **Free SO₂**: 28 ppm
- **TA**: 6.1 g/L

🛢️ **Vessel**: Tank T-07 (2,500L) — 92% full

📋 Recent actions:
- Oct 12: Punchdown (2x daily)
- Oct 10: SO₂ addition (25 ppm)
- Oct 8: Inoculated with RC-212 yeast

✅ Fermentation is on track. Expect dryness in 2-3 days.

---

**👤 You:**
> "Record a new lab reading for the 2025 Chardonnay: pH is 3.32 and TA is 6.5 g/L."

**🤖 AI Agent:**
> I have successfully recorded the lab analysis for the 2025 Chardonnay lot. The pH is now updated to 3.32 and TA to 6.5 g/L.

---

**👤 You:**
> "Which vessels are currently empty and available for the upcoming harvest?"

**🤖 AI Agent:**
> There are currently 6 empty vessels available: 4 stainless steel tanks (T-02, T-05, T-12, T-14) and 2 concrete eggs. Total available capacity is 18,500L.


## ❓ FAQ

**Q: How do I get InnoVint API access?**
Contact InnoVint support at support@innovint.us to request a Personal Access Token. You'll need an active InnoVint account.

**Q: Can I record lab analysis results using this integration?**
Yes, you can input new lab readings such as pH, TA, Brix, and free SO2 directly for a specific lot or vessel using natural language, and the AI will post them to the InnoVint API.

**Q: Does this support managing multiple wineries under the same account?**
Yes, if your InnoVint integrator account has access to multiple wineries, you can scope your API requests to a specific Winery ID to manage lots and vessels across different properties.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/innovint](https://vinkius.com/mcp/innovint)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **InnoVint** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `innovint` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **InnoVint** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "innovint": {
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
