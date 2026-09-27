# NYC Consumer Protection (DCWP) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-consumer-protection-dcwp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless NYC consumer-protection data: DCWP consumer complaints, business inspections, administrative charges and issued business licenses — no API key.

## Description
New York City Department of Consumer and Worker Protection (DCWP) records, keyless.

### What you can do
- **Consumer complaints** — complaints against city-regulated businesses (about 76,000 records since 2022): intake date and channel, business category, complaint code, business name and result, always scoped to an intake-date window (90 days back by default)
- **Top complaint codes** — the most frequent complaint codes in a window
- **Top complaint categories** — the most complained-about business categories in a window
- **Complaint count** — a fast count of complaints in a window, to gauge size before listing
- **Inspections** — DCWP business inspections (about 290,000 records) by type ("Patrol", "Tobacco - Sale to Minor", ...), status, business category and address, scoped to an occurrence-date window (90 days by default)
- **Top inspection types** — inspection types ranked by count in a window
- **Charges** — DCWP administrative charges (about 137,000 records) with the violation date, charge text, cure eligibility, outcome ("Default Decision", "Pleaded", "Hearing Decision" or none yet) and guilty count, scoped to a violation-date window (365 days by default)
- **License categories** — the ~72,000 issued business licenses ranked by category, optionally restricted to one status ("Active", "Expired", ...)

### Who is this for
Consumer research, local business intelligence and compliance work. The tables publish with a lag of a few weeks (complaints, inspections) to a few months (charges), and every text filter is an exact match on the stored value — use the top_* ranking tools to discover the category, code and status values.


## Available Tools (8)
- **count_consumer_complaints**: days defaults to 90 (max 365). Use it to gauge how large a complaint search will be before calling search_consumer_complaints.

Count DCWP consumer complaints in a window
- **search_consumer_complaints**: g. "Landlord or Real Estate Agent", "Supermarket"), the complaint code, the business name and the result. The dataset is large, so an intake-date window is always applied: after defaults to 90 days ago when omitted. Newer complaints publish with a lag — the latest records trail a few weeks behind today.

Search DCWP consumer complaints
- **search_dcwp_charges**: The dataset is large, so a violation-date window is always applied: after defaults to 365 days ago when omitted. Charges publish with a lag — the latest records trail a few months behind today.

Search DCWP administrative charges
- **search_dcwp_inspections**: g. "Patrol", "Tobacco - Sale to Minor"), inspection status, the certificate of inspection and the license number, plus the business name, business category and street address. The dataset is very large, so an occurrence-date window is always applied: after defaults to 90 days ago when omitted.

Search DCWP business inspections
- **top_complaint_categories**: days defaults to 90 (max 365). Each row is one business category (e.g. "Landlord or Real Estate Agent") with its complaint count in the window.

Top DCWP business categories by complaint count
- **top_complaint_codes**: days defaults to 90 (max 365). Each row is one complaint code with its count in the window; a null code is reported for complaints without one. Use it to see what consumers are reporting the most recently.

Most common DCWP complaint codes in a window
- **top_dcwp_inspection_types**: days defaults to 90 (max 365). Each row is one inspection type with its count in the window — e.g. "Patrol" dominates, followed by the tobacco-specific inspections.

Most frequent DCWP inspection types in a window
- **top_license_categories**: Each row is one business category (e.g. "Home Improvement Contractor", "Tobacco Retail Dealer") with its license count. Optionally restrict to one license status (e.g. "Active" or "Expired"). The aggregation runs citywide and returns fast.

Top DCWP license categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Consumer Protection (DCWP)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What landlord complaints have DCWP received in the past 90 days?"

**🤖 AI Agent:**
> search_consumer_complaints with business_category: "Landlord or Real Estate Agent" returns the complaints in the default 90-day intake window, newest first, with each complaint code and result; top_complaint_categories shows which categories dominate the window.

---

**👤 You:**
> "Which tobacco inspections did DCWP run most recently?"

**🤖 AI Agent:**
> search_dcwp_inspections with inspection_type: "Tobacco - Sale to Minor" returns the inspections in the default 90-day occurrence window with the business, its category, the inspection number and status; top_dcwp_inspection_types ranks all types in the window.

---

**👤 You:**
> "Which business categories hold the most active DCWP licenses?"

**🤖 AI Agent:**
> top_license_categories with license_status: "Active" returns the categories ranked by their active license count citywide.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: Do the text filters ignore case or match partial values?**
No. The NYC data platform only supports exact-match filters, so a filter value must equal the stored value. In this MCP, business categories are stored as listed (e.g. "Landlord or Real Estate Agent", "Tobacco Retail Dealer"), complaint codes as e.g. "Unlicensed" or "Sidewalk Blocked", outcomes as "Default Decision", "Pleaded" or "Hearing Decision", and license statuses as "Active" or "Expired". Use the top_* ranking tools, or a search tool with no filters, to see the exact stored values before filtering.

**Q: Why do the complaint and inspection tools use a date window?**
The complaints table holds about 76,000 records, the inspections table about 290,000 and the charges table about 137,000. Every search and ranking is therefore scoped to a window: 90 days back by default (max 365) for complaints and inspections, 365 days back by default for charges. The count tool gives the window size before you list.

**Q: How current is the data?**
The tables publish with a lag: the most recent consumer-complaint and inspection records trail today's date by a few weeks, and the charge records by a few months. Queries are keyed on the record's own date, so a default 90-day window returns what is currently published for that period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-consumer-protection-dcwp](https://vinkius.com/en/ai-agent-connect/nyc-consumer-protection-dcwp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Consumer Protection (DCWP)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-consumer-protection-dcwp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Consumer Protection (DCWP)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-consumer-protection-dcwp": {
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
