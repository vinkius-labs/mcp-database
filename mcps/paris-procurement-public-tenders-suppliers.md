# Paris Procurement: Public Tenders & Suppliers MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paris-procurement-public-tenders-suppliers)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government](../categories/government.md)

Keyless Paris public-procurement data: the 19,000+ city tenders 2013–2023 — market type, supplier, amount range, notification year — with per-year series, high-value filters and a dataset overview.

## Description
The City of Paris public-tender register (liste des marchés de la collectivité parisienne) — keyless, straight from the Paris open-data platform (opendata.paris.fr).

### What you can do
- **list_tenders / count_tenders / tender_lookup** — the ~19,000 tender rows: tender number (num_marche, the lookup key), object, market type ("SERVICES" / "TRAVAUX" / "FOURNITURE"), supplier (name, SIRET, postal code), amount range (montant_min / montant_max in euros), notification year, budgeting perimeter and purchase category
- **supplier_tenders / supplier_profile** — one supplier's whole tender history, or its totals split by the three market types
- **big_tenders** — the highest-value contracts at a minimum amount (a bare integer >= on montant_max; 1e6 returns 501 rows in 2023 services)
- **tenders_by_year** — per-year totals across the range, with the range sum and the last-minus-first delta
- **tenders_by_category / procurement_overview** — one purchase category's total (with its label) and the dataset's preset facets: top suppliers, top categories and the type split

### Who is this for
Public-procurement analysts, journalists tracking who wins city contracts, and researchers measuring public spending. The notification-year column is date-typed: the tools convert your 4-digit year into a quoted ISO year window automatically, and amount filters are bare integers on the montant_max column.


## Available Tools (8)
- **procurement_overview**: No parameters; one facets call plus one total call.

Overview of the public-tenders dataset: top suppliers, categories, types
- **supplier_tenders**: g. "ENEXCO PARIS") exactly matches the given value. supplier_nom is required; optionally restrict to one notification year (4 digits) and/or one market type (nature: "SERVICES" / "TRAVAUX" / "FOURNITURE"). Each row carries the negotiated amount range (montant_min / montant_max in euros) and the tender object.

List the tenders won by a supplier
- **big_tenders**: min_amount is required; optionally restrict to one notification year (4 digits) and/or one market type (nature). Useful to surface the city’s largest contracts, e.g. min_amount 1000000 for the seven-figure tenders.

List the highest-value tenders by a minimum amount
- **count_tenders**: A fast total count — use it to compare volumes between years, market types or suppliers’ budgets.

Count public tenders by type, year, perimeter or minimum amount
- **list_tenders**: Each row has: the tender number (num_marche, e.g. "20232023S09306"), the notification year (annee_de_notification, the display year "2013".."2023"), the object of the tender (objet_du_marche), the market type (nature_du_marche: "SERVICES", "TRAVAUX" or "FOURNITURE"), the supplier (fournisseur_nom, with SIRET and postal code/city), the negotiated amount range in euros (montant_min / montant_max) and the budgeting perimeter (perimetre_financier, e.g. "M57 Ville" or "M49 Assainissement") plus the purchase category (categorie_d_achat_cle code and categorie_d_achat_texte label). The year filter maps onto a DATE-typed column, so it is a quoted ISO window over annee_de_notification. Page with limit/offset (100 rows max).

List public tenders (marchés publics) awarded by the City of Paris
- **tender_lookup**: g. "20232023S09306") exactly matches the given value. num_marche is required; 0 or 1 row comes back with the object, supplier, amount range, notification year, budgeting perimeter and purchase category.

Look up a public tender by its number
- **tenders_by_category**: g. "7719"). categorie_cle is required; optionally restrict to one notification year (4 digits). The category label (categorie_d_achat_texte) is shown in the response metadata.

Count tenders for one purchase category
- **tenders_by_year**: year_to, 4 digits, default 2019..2023, both ends clamped to the dataset span ~2013..2023), computed as one fast DATE-window count per year plus the range total and the last-minus-first delta. Optionally restricted to one market type (nature).

Count tenders per notification year


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paris Procurement: Public Tenders & Suppliers** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many services tenders did Paris notify in 2023?"

**🤖 AI Agent:**
> Call count_tenders with nature "SERVICES" and year "2023" — the date column is windowed automatically; one fast total comes back.

---

**👤 You:**
> "Show me the ten biggest construction contracts of 2023."

**🤖 AI Agent:**
> Run list_tenders with nature "TRAVAUX", year "2023", min_amount "1000000" and limit 10 — each row carries the object, the supplier and the amount range.

---

**👤 You:**
> "Which supplier wins the most city tenders?"

**🤖 AI Agent:**
> procurement_overview returns the top-suppliers facet by tender count — the first entry is the most frequent awardee; supplier_tenders then lists that supplier's rows.


## ❓ FAQ

**Q: Do I need an API key?**
No. opendata.paris.fr serves all city datasets anonymously over its Opendatasoft REST API. This MCP defines no credentials and needs nothing configured.

**Q: How do I filter tenders by year?**
Pass a 4-digit year (e.g. "2023"). The annee_de_notification column is date-typed, so the tool builds a quoted ISO year window (>="2023-01-01T00:00:00" AND <="2023-12-31T23:59:59") instead of a text equality, which the platform would reject with a 400.

**Q: What is the difference between montant_min and montant_max?**
A tender's negotiated amount is a range: montant_min and montant_max in euros. big_tenders and the min_amount filter test montant_max — so min_amount 1e6 returns the tenders whose upper bound reaches a million euros.

**Q: Which budgeting perimeters are included?**
perimetre_financier marks the budgeting perimeter, e.g. "M57 Ville" (City of Paris), "M49 Assainissement" or "M57 Département" — the register covers both city and department markets. Use the perimetre filter for an exact match.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paris-procurement-public-tenders-suppliers](https://vinkius.com/en/ai-agent-connect/paris-procurement-public-tenders-suppliers)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paris Procurement: Public Tenders & Suppliers** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paris-procurement-public-tenders-suppliers` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paris Procurement: Public Tenders & Suppliers** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paris-procurement-public-tenders-suppliers": {
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
