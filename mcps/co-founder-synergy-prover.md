# Co-Founder Synergy Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/co-founder-synergy-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [strategy](../categories/strategy.md)

Two founders shook hands on 'we trust each other' — with no vesting cliff. It approved a 50/50 equity split out of politeness. It said 'we always agree' as conflict resolution. That is not synergy — that is a lawsuit. This tool forces five YC-level partnership axes: vesting protection, skill separation, deadlock resolution, equity justification, and execution velocity.

## Description
## The Problem

Every LLM commits five partnership reasoning failures:
1. **Cliff Blindness** — accepts handshakes without 4-year vesting and 1-year cliff.
2. **Skill Overlap** — approves two 'CEOs' with no builder.
3. **Deadlock Design** — accepts 50/50 without tie-breaker.
4. **Equity Politeness** — defaults to 50/50 out of fairness.
5. **Velocity Absence** — lets founders plan forever.

### The 5 Partnership Axes

| Axis | Pivot | Rule |
|---|---|---|
| **Vesting** | Cliff Mandated | 4-year, 1-year cliff, forfeiture terms. |
| **Skills** | Separated | Builder vs Seller — mutually exclusive. |
| **Conflict** | Deadlock Broken | Named CEO with tie-breaker authority. |
| **Equity** | Justified | Time, risk, capital, IP — not politeness. |
| **Execution** | Velocity Proven | Shipping dates, user counts, deploys. |

### Verdict Matrix

```
Axis 1 fails → CLIFF_ABSENT
Axis 2 fails → SKILL_OVERLAP
Axis 3 fails → DEADLOCK_RISK
Axis 4 fails → EQUITY_NAIVE
Axis 5 fails → VELOCITY_ABSENT
All pass     → SYNERGY_PROVEN
```


## Available Tools (1)
- **validate_co_founder_synergy**: Think like a YC partner evaluating a founding team — the #1 cause of startup death is co-founder conflict, and it is always structural. You must: (1) secure the CAP TABLE — 4-year vesting, 1-year cliff, monthly vesting after cliff, forfeiture terms, acceleration clauses. "We trust each other" is not a cap table strategy. Trust is necessary AND insufficient — legal structure protects both parties WHEN trust is tested, not IF, (2) separate SKILLS with MUTUALLY EXCLUSIVE ACCOUNTABILITY — who builds, who sells. Not "we complement each other" — specific daily activities. CTO writes code daily. CEO runs customer calls daily. If both "manage," nobody is accountable for output, (3) break DEADLOCKS — name the CEO with strategic tie-breaker authority. Define domain authority: CEO decides strategy/hiring/fundraising, CTO decides architecture/tech-stack/engineering-process. Escalation protocol: if disagreement persists after 48h, CEO decides. "We always agree" is a fantasy — disagreement is inevitable and healthy IF there is a resolution mechanism, (4) justify EQUITY — calculate based on measurable contributions: time invested (full-time from when?), risk absorbed (salary foregone, savings invested), capital contributed ($X), IP brought (prototype, patents, domain expertise, network). "50/50 to be fair" is politeness, not a rationale — it creates resentment when one founder contributes more, (5) prove VELOCITY — show shipping evidence. MVP launched by week X. First Y paying users by week Z. Weekly deploys. Customer interviews per week. Pivots based on data. "Stealth mode" is death — you learn nothing without shipping. "Perfecting the plan" is procrastination. If rejected, the partnership has a fatal structural flaw.

Structured reflection tool for YC-partner-level co-founder dynamics evaluation. Forces the agent to validate partnership structure with legal protections, mutually exclusive accountability, conflict resolution mechanisms, contribution-based equity, and shipping velocity. Catches Cliff Blindness (no vesting cliff — trusting handshakes instead of 4-year/1-year-cliff equity protection with forfeiture terms), Skill Overlap (two CEOs, no builder — "we both manage" means nobody is accountable), Deadlock Design (50/50 equity without tie-breaker authority — "we always agree" is a fantasy that kills startups), Equity Politeness (splitting 50/50 "to be fair" instead of calculating based on time, risk, capital, and IP contribution), and Velocity Absence ("stealth mode," perfecting the plan — no shipped product, no users, no data). Call once per founder team evaluation or partnership structure decision


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Co-Founder Synergy Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We trust each other, 50/50, we both manage, we always agree, still in stealth mode."

**🤖 AI Agent:**
> CLIFF_ABSENT — Five fatal gaps: no vesting, skill overlap, deadlock, equity politeness, zero velocity.

---

**👤 You:**
> "4y vesting, 1y cliff. CTO builds, CEO sells. CEO decides after 48h. 60/40 by contribution. MVP week 4, 10 users week 8, weekly deploys."

**🤖 AI Agent:**
> SYNERGY_PROVEN — Partnership validated. All axes pass. Execute.

---

**👤 You:**
> "Technical co-founder wants to rebuild the entire backend (6 months). Business co-founder wants to launch in 3 markets simultaneously (needs current backend). Both have valid points. Equity is 50/50."

**🤖 AI Agent:**
> Classic build-vs-ship tension. Neither is wrong — the conflict reveals missing decision framework. Define: what is the technical debt cost of NOT rebuilding? What is the market cost of NOT launching? Make the tradeoff quantitative, not emotional. Set a 90-day compromise: launch 1 market on current backend while scoping modular rebuild.


## ❓ FAQ

**Q: Why does it reject 'we trust each other'?**
Trust is not a cap table strategy. Without vesting, a co-founder can leave in month 2 with half the company. Mandate 4-year vesting, 1-year cliff.

**Q: Why is 50/50 considered naive?**
50/50 is politeness, not math. When one founder works full-time and the other part-time, equity must reflect actual contribution — time, risk, capital, IP.

**Q: What is 'Velocity Absent'?**
Strong alignment but zero shipping. Stuck in stealth mode. Launch now, iterate tomorrow. Show MVP date, first 10 users, deployment frequency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/co-founder-synergy-prover](https://vinkius.com/mcp/co-founder-synergy-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Co-Founder Synergy Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `co-founder-synergy-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Co-Founder Synergy Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "co-founder-synergy-prover": {
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
