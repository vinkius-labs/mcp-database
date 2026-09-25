# Outbound Briefing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/outbound-briefing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lead-generation](../categories/lead-generation.md)

Keyless pre-call and pre-email card for any target: who they are, whether they are hiring, whose mail they run, what new surface they just shipped, how much fresh federal money they hold — and what to do next. No key, no account.

## Description
Outbound dies on generic openings. This MCP assembles the concrete, verifiable material for the first line of any call or email, entirely from public reads — no key and no account anywhere in the chain.

### What you can do

- **One pre-call card** — the company's own words about itself, whose mail it runs and how strict the SPF/DMARC posture is, which stack its DNS points at, whether a job board is linked and how many roles are open, what subdomains appeared in the last 30 days, and the federal contract dollars its legal name just received.
- **Timing the attack** — a motion signal that says whether anything changed at the target inside your window (new surface, live hiring), so the outreach opens with a concrete event instead of an assumption.
- **Qualify the inbox** — MX, SPF and DMARC read from public DNS: the infrastructure side of cold-email deliverability, and the "email taken seriously" read.
- **Read the federal angle** — recent federal contract awards by recipient name: fresh government money is a proven ICP — a paying customer, compliance muscle, and a budget that just landed.
- **Score and order the list** — an ICP score across the readable signals (hot / warm / cold, with the per-signal points and the recommended move), and a compact per-domain brief that ranks a list by motion.

### How it works

The server reads the target's own homepage (job-board links included), the keyless public job-board endpoints for detected boards, the public certificate log, public DNS, and the public federal spending API. Readings are cached for an hour, and every source that does not answer is reported as unreadable with a retry note — never as an empty result — so an unavailable read is never mistaken for a negative signal.

### Who is this for

Outbound reps, SDRs, founders and sales engineers who need a grounded first line for every target: a card built only from what the target itself publishes, ready to read in seconds.


## Available Tools (7)
- **email_reachability**: This is the infrastructure side of cold-email deliverability, not a guarantee: SPF plus a strict DMARC policy marks "email taken seriously", and the absence of either is the qualifying signal that their inbox is easier to reach — while a strict posture also means bounce monitoring is more likely. If the lookups fail, the result says the source is unavailable, not that the posture is weak.

Whose mail the domain sends through and how strict its SPF/DMARC posture is, from public DNS. Keyless
- **tech_shift_signals**: Use the newest names as the opening hook ("you just shipped X") and the stack as qualification language ("you run Y"). Dates are first observations in the public certificate log, not exact deploy dates; an unavailable log is reported as such, not as "nothing changed".

What changed on the target's tech side: new subdomains in a window, what they run on, what mail they use. Keyless
- **prospect_briefing**: Each piece is from a public read; any source that did not answer is listed under unreadable sources, so a missing piece is "not read this time", never "does not exist". Lead the conversation with one concrete event from the card, not a generic introduction.

The full pre-call card for one domain: who they are, their mail posture, stack, hiring, fresh surface, and federal angle. Keyless
- **sales_motion_signal**: The motion flag is the timing read — when it is true, open with the concrete event as the hook; when it is false, the target goes on the radar for a re-check instead of an immediate blitz. Unreadable sources are listed, so a "no motion" answer with unreadables is not proof of stillness.

Whether anything at the target changed recently enough to attack now: new surface plus hiring. Keyless
- **federal_budget_signals**: Fresh federal money is a proven ICP trigger — a paying government customer, compliance muscle, and budget that just landed while the organization is choosing new tooling. An empty answer means the angle is not federal money (or the legal name differs); a rejected query is reported as the source pushing back, never as "no awards". Rate-limited source: read it when it matters, not in loops.

Recent federal contract dollars paid to a company, by recipient name. Keyless public spending data
- **icp_score**: Every component carries its own reading, and any source that did not answer is listed as unreadable and contributes zero — so the score is what is visible, not a verdict on the whole target; re-read after the flagged sources come back.

Score the target across the readable signals and say how to move: hot, warm or cold. Keyless
- **multi_domain_brief**: Order the attack list by the motion flag — rows with motion go first. The call reads only the first page; the note says how many domains were skipped so the remainder can be requested with the next page. Unreadable sources are listed per row: a row with unreadables is a partial read, not a clean one.

Compact enrichment of a list of domains: presence, mail posture, job board, fresh surface and a motion flag, one row each. Keyless


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Outbound Briefing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me the full pre-call briefing for acme.io before I talk to them about our API platform."

**🤖 AI Agent:**
> 🗂️ **Pre-call card — acme.io (Acme Corp)**

**Who they are:** "Developer tools for small teams" — the homepage reads itself.
**Mail:** Microsoft 365 · SPF present · DMARC quarantine
**Runs on:** AWS CloudFront + Google / Firebase
**Hiring:** Greenhouse board, 14 open roles — 3 of them API platform engineers
**Fresh surface (30d):** `ai.acme.io`, `partners.acme.io`
**Federal angle:** $4.5M of contract dollars in the window (DoD, NASA)

**Move:** open with the partners subdomain + the API hiring: "Saw you just stood up partners.acme.io and you're hiring for API platform — we help with exactly that integration."

---

**👤 You:**
> "I have this list of prospects — stripe.com, notion.so, linear.app, figma.com, cal.com. Which do I attack first this week?"

**🤖 AI Agent:**
> 📋 **List brief — 5 of 5 domains**

| domain | presence | job board | new 90d | flag |
|---|---|---|---|---|
| linear.app | live | Ashby (9 open) | 4 | **motion** |
| cal.com | live | — | 2 | **motion** |
| stripe.com | live | — | 0 | |
| notion.so | live | Lever (2 open) | 0 | |
| figma.com | unreadable this time | | | |

**Order:** linear.app first — hiring through Ashby with 9 open roles plus 4 fresh subdomains in 90 days is a double live signal. cal.com second on the two new surfaces. figma.com: re-check after its unreadable sources come back; an unavailable read is not a negative.

---

**👤 You:**
> "Score hubspot.com as an ICP for a dev-tools product and tell me how to move."

**🤖 AI Agent:**
> 🎯 **ICP score — hubspot.com · 72/100 · HOT**

web_presence 15/15 · hiring 20/20 (Greenhouse, 31 open roles) · fresh_motion 20/20 (7 new subdomains in 90 days) · email_maturity 13/15 (SPF + DMARC reject) · federal_budget 0/30 (no federal dollars found for that name in the window)

**Move:** hot — multiple live signals. Open with the freshest event: the new subdomains read like an integrations push; pair it with the hiring read ("I see you just opened platform roles on Greenhouse"). One concrete event does the opening the generic email can't.


## ❓ FAQ

**Q: Do I need an API key or an account?**
No. Every read is public: the target's own website, the keyless public endpoints of the detected job boards, the public certificate log, public DNS, and the public federal spending API. There is no credential anywhere in the chain — nothing to issue, rotate or store.

**Q: How is the ICP score computed, and what does a low score mean?**
Five readable signals, each with its own points: web presence (15), hiring (20), fresh subdomain motion in 90 days (20), mail-infrastructure maturity (15) and federal contract dollars (30). 70+ is hot (attack now), 40–69 warm (time the next move to the freshest event), below 40 cold (nurture and re-check). Any source that did not answer is listed as unreadable and contributes zero — so the score is what is visible, not a verdict on the whole target; re-read after the flagged sources come back.

**Q: Is the job-board read a complete census of their hiring?**
No — it is the board linked from the homepage, and the open-role count is read only where the provider publishes a keyless endpoint (Greenhouse and Lever give exact counts; other providers report the board's presence but not the number). A board linked only from a careers page, or a provider that is not scanned, does not show up: "no board detected" is a read limit, not proof of no hiring. The result says exactly what it read.

**Q: What exactly does the federal read measure?**
Federal contract dollars paid to the company's registered name in the US, inside your window: the total for the top matching recipient, how many recipients matched, and the three most recently modified awards with public links. It answers one GTM question — "did this target just receive fresh government budget that forces new tooling decisions?" — and it is US-only, by the nature of the source; for a target outside the US federal scope, that angle simply does not apply and the score says so.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/outbound-briefing](https://vinkius.com/en/ai-agent-connect/outbound-briefing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Outbound Briefing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `outbound-briefing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Outbound Briefing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "outbound-briefing": {
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
