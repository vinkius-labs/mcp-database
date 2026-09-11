# SNS Portugal Health Transparency MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sns-portugal-health-transparency)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Official Portuguese national health service (SNS) open data: SNS24 calls, consultations, surgeries, transplants, blood donors, clinical trials, medicines and the SNS budget — queryable with filters and pagination, zero-auth.

## Description
The **official transparency portal of Portugal's Serviço Nacional de Saúde** as a single MCP server — 144 datasets of authoritative Portuguese public-health data.

### What you can do
- **Browse the catalog** — SNS24 call volumes, primary-care nursing contacts, scheduled consultations, surgeries, transplants and donors, clinical trials, medicines stock and prescriptions, the SNS budget account, FRIESA efficiency index and more
- **Query with precision** — ODSQL filters (`where data>='2025-01'`), facet refinement, field selection, sorting and true offset pagination
- **Latest values instantly** — a dedicated tool that sorts by each dataset's date column and returns the most recent records
- **Lightweight counts** — get record counts without fetching rows

### Why it matters
This is the SNS's own published data — the same numbers behind Portuguese health policy debates: SNS24 call volumes, elective surgery recovery, transplant activity, blood donation, teleconsultation growth and the health service's public account. Filterable to any period and any institution.

### Who is this for?
Healthcare analysts, journalists, policy researchers, students, and AI agents that need authoritative Portuguese national health statistics straight from the source.


## Available Tools (6)
- **list_datasets**: Covers SNS24 calls, consultations, surgeries, transplants, blood donors, clinical trials, medicines, the SNS budget account and more. Use page/page_size to navigate — never fetch all pages at once.

List all open data datasets of the Portuguese SNS (national health service) transparency portal
- **search_datasets**: g. "medicamentos", "transplantes", "cirurgias", "sns24"). Case-insensitive; all words must match.

Search SNS datasets by keyword (id, title or field names)
- **get_dataset**: Use a dataset_id from list_datasets or search_datasets.

Get full schema and metadata of an SNS dataset (fields, labels, records count)
- **query_records**: where example: data>='2025-01'; order_by: field name, prefix - for desc (e.g. -data); refine: facet=value (e.g. uf=Hospital de São João); select: comma-separated fields. Returns total_count plus the requested page — combine limit/offset to paginate.

Query records of an SNS dataset with filters (where, refine, order_by) and pagination
- **get_latest_records**: g. latest SNS24 calls, latest transplants).

Get the most recent records of an SNS dataset (sorted by its date column, descending)
- **count_records**: Useful before paginating with query_records.

Count records in an SNS dataset (with optional filter), without fetching rows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SNS Portugal Health Transparency** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many emergency calls were transferred to SNS24 recently?"

**🤖 AI Agent:**
> 🏥 **SNS24 emergency call transfers**

Latest months (dataset sns24):
- 2026-06: 6,766 calls
- 2026-05: 6,812 calls
- 2026-04: 6,950 calls

Series runs monthly since 2012 (174 records). Want the full year-over-year trend or only 2026?

---

**👤 You:**
> "Find datasets about transplants and show the latest numbers"

**🤖 AI Agent:**
> 🫀 **Transplant datasets on the SNS portal**

Found 2: `orgaos-colhidos-e-transplantados` (organs harvested & transplanted) and `dadores-vivos-e-falecidos` (living & deceased donors).

Latest records show kidney remains the most transplanted organ, with living-donor activity trending up year over year. Want the breakdown by organ type?

---

**👤 You:**
> "What is in the SNS account dataset — revenue vs budget?"

**🤖 AI Agent:**
> 💶 **Dataset: conta-do-servico-nacional-de-saude**

Monthly time series comparing:
- Budget: current revenue, fiscal taxes, direct/indirect taxes, social contributions
- Execution: actual revenue recorded by the SNS

I can pull any month and compute the execution-vs-budget gap. Want the latest month?


## ❓ FAQ

**Q: Do I need an API key or registration?**
No. The SNS transparency portal's Opendatasoft API is fully public — every tool in this MCP works without authentication.

**Q: Why is there no text-search server-side, and how does search_datasets work?**
The portal's `q` parameter is ignored by this Opendatasoft instance, so search_datasets scans the full 144-dataset catalog client-side (2 requests, cached behavior) and matches your terms against ids, titles, descriptions and column names.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sns-portugal-health-transparency](https://vinkius.com/en/ai-agent-connect/sns-portugal-health-transparency)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SNS Portugal Health Transparency** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sns-portugal-health-transparency` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SNS Portugal Health Transparency** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sns-portugal-health-transparency": {
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
