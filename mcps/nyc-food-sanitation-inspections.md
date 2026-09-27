# NYC Food & Sanitation Inspections MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-food-sanitation-inspections)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless NYC food-safety data: restaurant health inspections and A/B/C grades by CA#, rodent inspection results, school cafeteria inspection findings, and food scrap drop-off sites — no API key.

## Description
The Department of Health & Mental Hygiene and DSNY food-safety datasets, keyless.

### What you can do
- **Search restaurant inspections** — by CA# (health certificate), business name, borough, grade (A/B/C) or date window
- **Get one restaurant's grade** — the most recent inspection of a CA#: score, grade, type and date
- **Rodent inspections** — DSNY property inspections and abatements, with result and any letter issued
- **School cafeteria findings** — inspection codes and violation descriptions per school
- **Food scrap drop-off sites** — the city's compost drop-off locations with open months and hours

### Who is this for
Food-safety research, restaurant due diligence, public-health analysis and local-jurisdiction comparisons.


## Available Tools (5)
- **get_restaurant_grade**: If the establishment has never been graded, the grade field is empty.

The current grade and latest inspection of one restaurant by CA#
- **list_food_scrap_dropoffs**: Filter by borough (title case) or council district.

List NYC food scrap drop-off sites (composting locations)
- **search_cafeteria_inspections**: Filter by school name, borough or inspection date window.

Search school cafeteria health inspections (violations and codes)
- **search_restaurant_inspections**: Boro values are title case (Manhattan, Brooklyn, ...); dba is the business (legal) name. Dates are ISO "YYYY-MM-DD".

Search NYC restaurant health inspections and grades
- **search_rodent_inspections**: ) and any letter issued. Filter by borough, zip, street/house number or inspection date window.

Search DSNY rodent infestation inspections and abatements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Food & Sanitation Inspections** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What grade does this restaurant (CA# 50155931) have?"

**🤖 AI Agent:**
> get_restaurant_grade("50155931") returns the most recent inspection: name, address, current grade, score, inspection type and date.

---

**👤 You:**
> "Which Queens neighborhoods have the most rodent problems?"

**🤖 AI Agent:**
> search_rodent_inspections with borough "Queens" and result "Rodent Activity" over a date window shows the affected properties; the open-data MCP's grouped stats can rank by community board.

---

**👤 You:**
> "Where can I drop off food scraps in Manhattan?"

**🤖 AI Agent:**
> list_food_scrap_dropoffs with borough "Manhattan" returns the compost drop-off sites with open months, operating days and hours.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: What does the CA# mean?**
The CA# (health certificate number) is the unique id of a restaurant establishment. Each inspection row belongs to one CA#, so you can follow a restaurant's full inspection history and its current grade.

**Q: What do the grades mean?**
Grade A means the restaurant meets most requirements; B is a fair score with violations to correct; C signals serious violations; Z is assigned when an inspection cannot be scored yet (e.g. a new establishment).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-food-sanitation-inspections](https://vinkius.com/en/ai-agent-connect/nyc-food-sanitation-inspections)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Food & Sanitation Inspections** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-food-sanitation-inspections` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Food & Sanitation Inspections** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-food-sanitation-inspections": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
