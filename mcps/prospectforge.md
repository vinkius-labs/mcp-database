# ProspectForge MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/prospectforge)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lead-generation](../categories/lead-generation.md)

Prospecting intelligence, not a database: describe your ideal customer, get ranked prospects with verified legal entity, confirmed contacts and observable growth signals — every claim carrying its source and its confidence. Keyless by default.

## Description
A record says "João Silva, joao@empresa.com". ProspectForge says "João Silva, Head of Sales — role confirmed on the company leadership page; the company is hiring 4 commercial roles and rewrote its pricing page 3 times in 6 months." The difference is the whole point: prospecting intelligence instead of a stale list.

### What you can do

- **Forge prospects from a profile** — "SaaS companies in Portugal with 10-100 employees and Heads of Sales". One call runs discovery, verification, signal extraction and ranking, and returns every prospect with a per-field evidence ledger.
- **Find companies like a reference** — "companies like Stripe in Europe with sales leaders I can contact": the tool profiles the reference company and runs the pipeline on its footprint, and tells you when it had to fall back to a looser keyword match.
- **Discover the candidate pool** — the light call: candidate companies with source and fit data, nothing verified yet, so you always see the full set.
- **Verify one company in depth** — live official site (about/team/leadership/contact/careers), legal entity against the public register, engineering org activity, web-archive history and named people in your target roles.
- **Verify one contact** — does this person still hold this role, today, on the company's own site? Is a matching email actually published there?
- **Read observable signals** — open commercial roles, the engineering org's repositories and languages, and product/pricing page change in the web archive.
- **Recover a vanished page** — old pricing, discontinued product, previous contact sheet — from historical web indexes.

### How it works

The pipeline is deliberately staged: **discover → verify → signal → score → rank**. Discovery builds the candidate pool from public web data. Verification cross-checks each candidate against independent public records. Signals read what the company is visibly doing right now. Ranking then orders the result by how much of it was actually confirmed.

Every field the pipeline asserts ends up with a state — **confirmed / unverified / conflicted / absent** — and its source URL. Ranking is confidence, not promise: fit (40) + observable signals (35) + verification depth (25), so a company that fits the profile but could not be verified ranks below a slightly-less-perfect company you actually confirmed.

### The hard rules

- **No email is ever invented.** An email is reported only when a public page publishes it. If none is found, the answer says so and points at enrichment.
- **A missing fact is a fact.** Unknown headcount, no legal-entity record, no published email — each is reported as absent, never filled in.
- **Sources are soft.** One source failing degrades that source's evidence to "unavailable in this run"; it never fails the prospect.
- **Prospecting on B2B contact data is your responsibility** — handle it under GDPR legitimate interest with a real purpose.

### Who is this for

Outbound teams, SDRs, agency operators and founders who would rather have 6 real prospects with evidence than 60 rows of guesses — and who need to know exactly which fields they can trust before writing a single personalized line.


## Available Tools (10)
- **recover_page**: Use it to verify market/product history ("what did they sell two years ago") and to recover evidence that the current site no longer shows. A "not captured" answer is a real negative: the page was either never crawled or was robots-excluded.

Recover a company public page that no longer exists on the live site, from Common Crawl historical indexes. Keyless
- **find_people**: Results are HEURISTIC — the confidence is labelled, and every person it returns should be re-checked with verify_contact before outreach. Pass roles like "head of sales" or "chief financial officer". An empty list means no matching role mention was found on the readable pages: a different, honest answer from "the site has no team page".

Find named people in target roles on the company own team/leadership pages. Keyless, heuristic and labelled as such
- **find_prospects**: Nothing here is verified yet — treat the result as candidates to check with forge_prospects or verify_company, and say so when you report it. Employees/country/industry fields come straight from their discovery source and are labelled as such.

Discovery-only: candidate companies matching a profile, with source and fit data but no verification. Keyless
- **verify_company**: Returns an evidence ledger: each field with a confirmed / unverified / absent state and its sources. Use it before trusting any contact or claim about a company, and after find_prospects to check a specific candidate. A company with no live site and no LEI record comes back as unverified with those two facts — that is an answer, not an error.

Verify one company in depth: official website, legal entity, engineering org, web-archive history, leadership people. Keyless
- **verify_contact**: THE HARD RULE: if no matching email is published, the answer says no email was found and points at enrichment — it never constructs one from a pattern. This is the difference between prospecting intelligence and a stale database: a role that no longer appears on the site is reported as gone, not quietly kept.

Confirm a named person current role and published email against the company own website. Never invents an email. Keyless
- **verify_legal_entity**: Useful right before a contract or a compliance step: the answer distinguishes "legal entity confirmed in this jurisdiction" from "no LEI record at all", which are very different facts. Multiple records: prefers an exact-name match, then a record in the country you asked about, and reports how many alternatives exist.

Confirm the legal entity behind a brand in GLEIF: LEI, legal name, jurisdiction, status, address. Keyless
- **verify_website**: This is the ground-truth layer for contacts: a published email or team listing is a fact you can cite. JS-only sites may return an empty people section — the answer then says the pages were not readable, which is honest rather than guessing. Note that prospecting on B2B contact data carries a legitimate-interest responsibility under GDPR: use it for outreach with a real purpose.

Read a company official site verification pages: about/team/leadership/contact/careers, published emails and socials. Keyless
- **company_signals**: These are OBSERVABLE signals, not predictions — a company with open sales roles is visibly hiring commercial headcount; a pricing page archived 3 times in 180 days is visibly changing its commercial surface. Empty results mean the public signal is unavailable, never that the company is idle.

Observable growth signals for one company: open commercial roles, engineering org activity, product/pricing page change. Keyless
- **forge_prospects**: Every fact returned carries a state — confirmed / unverified / conflicted / absent — and its source. Use the natural form: "SaaS companies in Portugal with 10-100 employees and Heads of Sales". Inputs: country (name or ISO-2), keywords (comma list, e.g. "saas,payments"), employees ("10-100" or "50+" or "37"), roles (comma list, e.g. "head of sales,vp sales"), limit (prospects returned, default 10), verify_limit (how many get the deep pass, default 6). Important honesty rules baked into the results: an email is only reported when a public page publishes it — it is never pattern-guessed; a company whose headcount is unknown stays in the set rather than being silently dropped; and candidates beyond verify_limit come back flagged unverified so the agent knows what was not checked. If no candidates are found, widen the employee band or the keywords — discovery is strongest for companies with a real public web footprint.

The flagship pipeline: describe an ideal customer — country, industry keywords, employee band, target roles — and get back ranked, evidence-graded prospects. Keyless
- **similar_prospects**: When the peer has no usable industry data — common for well-known US tech brands — the tool says so and runs discovery on region and size band alone; those results are looser than a true industry match and the result tells you which mode ran. Use for "find 100 Portuguese companies likely to need a CRM" style asks where a reference brand anchors the profile. Inputs: peer (name or domain), region (country), employees band, limit.

Find companies similar to a reference company inside a region and size band — "companies like Stripe in Europe". Keyless


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ProspectForge** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find SaaS companies in Portugal with 10-100 employees and Heads of Sales."

**🤖 AI Agent:**
> 🔥 **3 prospects forged** (7 candidates discovered, 3 verified)

**Acme Pay — ✅ verified · confidence 78/100**

Website acmepay.com · Portugal · 37 employees · Industry fintech, payments

Why this lead:
- Hiring 4 open commercial roles (2 sales, 2 marketing); freshest posting 3 days ago.
- Engineering org with 27 public repos, TypeScript/Go, last push 2 days ago.
- Pricing page archived 3x in the last 180 days.
- Legal entity confirmed in the public register: ACME PAY LDA (PT).
- Inês Costa — Head of Sales, confirmed on /leadership.

Caveat: Inês Costa has no email published on the site — enrichment needed for a verified address.

Evidence ledger: company ✅ website ✅ employees 🟡 hiring ✅ technology ✅ legal_entity ✅ role ✅ email ⬜

Want me to verify Inês Costa's email separately, or deepen the next 4 candidates?

---

**👤 You:**
> "Find companies like Stripe in Europe with sales leaders I can contact."

**🤖 AI Agent:**
> 🧲 **Similar to Stripe — keyword fallback**

The reference company carries no usable industry profile, so discovery used its name as a keyword rather than a true industry match — results are looser. 5 prospects forged, 3 verified.

Top match: **PayX (payx.eu)** — ✅ verified, confidence 71/100. Payments infrastructure, Portugal, 54 employees. Hiring 3 commercial roles (freshest 6 days ago); a VP Sales appears on /leadership; legal entity confirmed in jurisdiction PT. No email published for the VP — enrichment would be the next step.

Want me to drop to discovery-only for a wider set, or verify the VP Sales at PayX in depth?

---

**👤 You:**
> "Verify stripe.com as a company — is the legal entity real and what is it actually building?"

**🤖 AI Agent:**
> 🔎 **Stripe — ✅ verified**

Legal entity confirmed in the public register: STRIPE (LEI 894500EDC64T52PGFL08, jurisdiction BE — the Belgian operating entity; the group has 58 records under this name). Live official site with /about, /contact and /careers readable.

Technology: public engineering org `stripe` with 200+ public repositories — stripe-android, stripe-ios and stripe-python are the most recently pushed; TypeScript, Go, Ruby and Java dominate.

Hiring: open commercial roles including Account Executive positions, with the freshest posting 3 days ago — visibly staffing the commercial org.

Evidence ledger: company ✅ website ✅ legal_entity ✅ technology ✅ hiring ✅ employees ⬜. Note the registered jurisdiction is Belgium, not the US parent — a fact worth citing before a contract step.


## ❓ FAQ

**Q: Do I need an API key or an account?**
No. ProspectForge needs no API key, no account and no credit card. It works entirely from public web data, out of the box.

**Q: Will it give me an email for every contact?**
Only when a public source publishes it. ProspectForge never constructs an email from a name-pattern guess: if nothing publishes one, the field is reported as absent and the answer points at enrichment. That is deliberate — an invented email costs you sender reputation and trust, while a known absence tells you exactly which step to buy.

**Q: How can results be trusted? What does the verification state mean?**
Every field the pipeline asserts lands in an evidence ledger with one of four states: confirmed (at least one independent public source shows it), unverified (a source reported it but no source corroborates it), conflicted (sources disagree — flagged, never averaged away) or absent (no source had it). A whole prospect is verified only when its website is live AND its legal entity is confirmed in the public register; partially_verified means one of the two. Ranking follows confidence: fit (40) + observable signals (35) + verification depth (25).

**Q: What happens when discovery finds few companies for my profile?**
Discovery is strongest for companies with a real public web footprint — a live site, published people pages and visible hiring activity. Many small, purely non-technical businesses leave few public traces, and the result tells you exactly which part of the profile came up thin, so you can widen the employee band, loosen the keywords or try a neighbouring market.

**Q: Is using contact data from company websites allowed?**
Reading publicly published B2B contact data for outreach is generally permitted under GDPR's legitimate-interest basis when there is a real commercial purpose and the individual could reasonably expect it, and you must honor opt-outs. This server reads only public pages and labels every contact with its source and confidence. It is your responsibility to apply that legal basis in your jurisdiction — the tool gives evidence, not legal advice.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/prospectforge](https://vinkius.com/en/ai-agent-connect/prospectforge)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ProspectForge** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `prospectforge` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ProspectForge** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "prospectforge": {
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
