# Federal Contracts ICP MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/federal-contracts-icp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless US federal spending intelligence from the government's own public database — company federal footprint, fresh contract wins, new-budget triggers and top vendors per industry or agency, for ICP proof and outbound timing. No key, no account.

## Description
A company that takes US federal contract dollars is the strongest ICP proof available: it has a paying government customer, compliance muscle, and budget that shows up in public records. This MCP makes that proof queryable — and turns fresh awards into timing triggers — with no key and no account anywhere in the chain.

### What you can do

- **Prove an ICP** — ask whether a company receives federal contract money, and get its total dollars, award count, agencies served and NAICS mix back. An empty answer is itself a fact: the trigger does not apply to that target.
- **Read a footprint** — the depth tool: total dollars over a window, UEI, the most recent awards with links to the public award pages.
- **Watch fresh movement** — awards that were just modified or that just started performance: new budget at the recipient is the warmest timing signal, filterable by industry, agency and minimum amount.
- **Benchmark a vertical** — the biggest federal vendors inside a NAICS code or an agency, by dollars awarded.
- **Deep-read one award** — full card for any award id: recipient, UEI, dollars, period, agencies, the NAICS description and the public page. The description text is personalization fuel ("congratulations on the X contract").

### How it works

The server reads the federal government's own public spending database — the same one behind the national contract-expenditure site — through its open API, no credentials. Responses are cached in memory for an hour so repeated scans do not burn the public quota, and award lookups walk every award-type family until one answers, so contract, grant, loan and payment ids all resolve.

### Who is this for

Outbound and enterprise sales teams that sell into the government-adjacent market: ICP proof before the call, fresh-award timing as the outreach hook, and federal benchmarking to know who else is in the room.


## Available Tools (6)
- **company_federal_footprint**: A large multi-agency footprint means a mature, compliance-heavy organization — the ICP proof and the personalization context in one call. An empty result means the trigger does not apply: try the registered legal name, or pick a different signal for this target. This is the depth tool: run federal_icp_targets first for discovery, then this one for the specific company you are about to call.

Is a company a federal vendor at all, and how big is its footprint: total dollars, agencies served, NAICS mix, recent awards. Keyless
- **award_detail**: Use it after any list tool when a single award is worth deep reading — the description text is your personalization source, e.g. "they just won an RF analytics contract for a specific detachment". The engine looks the id up across every award-type family, so contract, grant, loan, direct payment and IDV ids all resolve. If the id is not in the federal spending database the result says so explicitly instead of erroring — it may come from another system or have a typo.

Full card for one federal award by its id: recipient, UEI, dollars, period, agencies, NAICS description and the public page. Keyless
- **federal_icp_targets**: For every matching recipient it returns total dollars awarded, how many awards, when the activity was last modified, which agencies and NAICS codes are involved, and an example award id. The window defaults to one year; narrow it for "still active". A recipient of federal money is the strongest ICP proof available: a paying government customer, compliance muscle and budget. An empty result is also a fact — the company may be registered under a different legal name (try it) or it simply does not hold federal business, in which case the federal trigger does not apply to it. Results are paged: has_more says whether to call again with a higher offset.

Companies receiving federal contract dollars, aggregated per recipient: total awarded, award count, agencies and NAICS. Paged. Keyless
- **new_budget_triggers**: Each row carries recipient, amount, agency, NAICS, start date and the public award page. This is the purest timing trigger the server offers: a company that just started a big federal contract is rebuilding — new teams, new tooling, new vendor choices, all this week. Filter by minimum amount to keep only the deals big enough to matter; by NAICS or agency to focus a vertical. An empty result means no matching award started that fresh in the slice: widen the window or drop the minimum before concluding there is no fresh budget.

Federal awards whose performance just started — fresh budget at the recipient, filterable by NAICS, agency and minimum amount. Keyless
- **recent_contract_wins**: Every row carries the award id, recipient, dollar amount, agency, NAICS code, performance start date and a link to the public award page. Use it as the "who just won" trigger: a freshly modified award is money the recipient just took and is rebuilding around — vendors land well then. With no filter it is a general market-activity watch; with a NAICS it is an industry trigger feed; with an agency it is a government-relationship watch. A recent win at a recipient is the timing signal that personalizes any outreach: "congratulations on the X contract".

The most recently modified federal contract awards, optionally filtered by recipient, NAICS or agency. Paged. Keyless
- **top_federal_vendors**: Each row is the vendor, its total, its award count, last activity and the agencies it serves. Use it as ICP benchmarking — "who is the biggest player in this vertical at government" — and as competitor discovery: a vendor ranked high with a strong federal mix is both a proof point for your own outreach and a competitive signal. The ranking reflects the most recently modified matching awards, so read it as the visible picture, not the full census: a longer window gives a bigger one.

Rank the biggest federal vendors by dollars awarded, in a NAICS slice, at an agency, or across the board. Keyless


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Federal Contracts ICP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is Palantir a proven federal ICP? How big is its footprint?"

**🤖 AI Agent:**
> 🏛️ **Federal footprint: Palantir — 3 years**

Federal vendor: 47 recently modified contract awards, totaling **$1.9B**.
Agencies served: Department of Defense, Department of the Army, Department of the Air Force, NASA · NAICS mix: 541511, 541519

ICP proof: a paying government customer, multi-agency, at enterprise scale. Want the ten most recent awards with links?

---

**👤 You:**
> "What fresh federal budget landed in custom computer programming this month? Only deals over $10M."

**🤖 AI Agent:**
> 💸 **New budget triggers — NAICS 541511, min $10M, last 30 days**

3 qualifying awards:
- Amazon Web Services, Inc. — $15.2M, Department of Defense, started 2026-08-30 (RF analytics contract)
- …

Fresh money at the recipient = new scope, new teams, new tooling decisions. These three are the warmest outreach windows in this vertical right now. Want the full award card of the first one?

---

**👤 You:**
> "Read award FA930125P0031 in full — I'm writing the outreach to its recipient."

**🤖 AI Agent:**
> 📄 **Award FA930125P0031**

Recipient: Amazon Web Services, Inc. (UEI NQEWN6C1LSU5)
Amount: $4.5M · NAICS 541511 — Custom Computer Programming Services
Period: 2025-06-16 → 2027-06-15 · Awarding: Department of Defense
Description: "CSO — RADIO FREQUENCY (RF) DATA ANALYTICS FOR AFTC DET 1/MDTF"

Outreach hook: a two-year RF-analytics contract just in performance means a data pipeline and tooling decisions are happening now. Lead with the analytics workload, not the product list.


## ❓ FAQ

**Q: Do I need an API key or an account?**
No. The federal government publishes its own contract spending data through an open API with no credentials — the same data behind the national contract-expenditure site. There is nothing to issue, rotate or store.

**Q: What counts as a "new budget" trigger?**
An award whose performance period just started and that was modified inside your freshness window (default 30 days). The recipient took new money: new scope, new teams, new tooling decisions. Filter by minimum amount to keep only deals big enough to matter, and by NAICS or agency to focus a vertical.

**Q: Why do rankings and totals sometimes look partial?**
The open API exposes a ranked, paged view rather than a server-side census per company, so every aggregation works over the most recently modified matching awards in the slice you asked for. The result says how many awards it scanned, and a longer window or deeper paging gives a fuller picture. That is documented in each result, never silently assumed.

**Q: How is the public source protected from repeated scans?**
Each distinct query is cached in memory for one hour, so re-asking the same question minutes apart costs nothing upstream. If the source rate-limits, the error tells you to vary the query or try again later instead of hammering in a loop.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/federal-contracts-icp](https://vinkius.com/en/ai-agent-connect/federal-contracts-icp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Federal Contracts ICP** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `federal-contracts-icp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Federal Contracts ICP** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "federal-contracts-icp": {
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
