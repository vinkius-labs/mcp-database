# Incident Postmortem Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/incident-postmortem-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Most postmortems fail: vague timelines, symptom-level root causes, and action items with no owner. This tool forces SRE-grade rigor: minute-by-minute timeline reconstruction, systemic 5-Whys analysis, root cause isolation, accountable action items with owners and deadlines, and historical pattern detection.

## Description
70% of incident postmortems fail at root cause identification. Teams write 'add monitoring' as an action item and move on. The same incident recurs 3 months later.

### The 5 Postmortem Failures This Tool Prevents

1. **TIMELINE_INCOMPLETE** — No minute-by-minute reconstruction. 'Around 3 PM something happened' is not a timeline.
2. **ROOT_CAUSE_SHALLOW** — Stopped at the symptom. 'The server crashed' is what happened, not WHY it happened.
3. **CAUSES_CONFLATED** — Root cause mixed with contributing factors. The trigger is not the vulnerability.
4. **ACTIONS_UNACCOUNTABLE** — 'Add monitoring' has no owner, no deadline, no success metric.
5. **PATTERN_IGNORED** — No comparison with previous incidents. This may be the 3rd time this quarter.

The engine enforces 5 Decision Pivots with semantic trap lists that catch vague timelines, shallow analysis, conflated causes, hand-wavy actions, and dismissed patterns.


## Available Tools
- **validate_incident_postmortem**: A postmortem that stops at "the server crashed" is a narrative, not an investigation. You must: (1) reconstruct the TIMELINE minute-by-minute in UTC — every alert, page, action, decision, and escalation. If you cannot account for a 5-minute gap, that gap hides a process failure, (2) apply 5 WHYS until you reach an organizational or systemic root — "server crashed" is Why #0. Why crashed? Why THAT? Why THAT? Keep going until you reach a process, incentive, or cultural root cause, (3) SEPARATE root cause from contributing factors — root cause ENABLES, factors AMPLIFY. "Multiple causes" is a dodge. There is one enabling cause and several amplifiers, (4) write ACTION ITEMS with ODAS: [Owner] [Deadline] [Specific Action] [Success Metric]. "Add monitoring" will be forgotten. An owner, a date, an action, and a measurable success criterion will not, (5) cross-reference INCIDENT HISTORY for recurrence patterns — same service, same cause type, same window, same team. "First time" requires evidence. If rejected, your postmortem is a narrative, not an investigation.

Structured reflection tool for rigorous incident postmortem analysis — forces minute-by-minute timeline reconstruction, 5 Whys chain to systemic root cause, root cause isolation from contributing factors, owner-deadline-metric action items, and recurrence pattern analysis. Catches Timeline Incomplete (narrative summary instead of minute-by-minute reconstruction — "the site went down for about an hour" is a story. "14:32 UTC — PagerDuty alert fires. 14:33 — @bob paged. 14:35 — Joins #incident-123. 14:38 — Identifies crash loop in payment-svc. 14:42 — Rollback v2.4.1→v2.4.0 initiated. 14:45 — Service recovered" is an investigation. Every minute unaccounted for is a gap in the investigation), Shallow Whys (stopping at the surface symptom instead of reaching systemic root cause — "the server crashed" is Why #0, not a root cause. Why crashed? → OOM. Why OOM? → Memory leak. Why leak? → No integration test on payment→inventory path. Why no test? → Testing culture prioritizes unit tests. Why? → Team incentives reward feature velocity. THAT is a root cause — an organizational incentive structure), Root Cause Confused (conflating root cause with contributing factors — "multiple causes" is a dodge. There is ONE root cause that ENABLES the incident. Contributing factors AMPLIFY but do not cause. Friday deploy is a contributing factor — it did not cause the bug, it reduced staffing to catch it. Root cause: no integration test. Contributing: Friday deploy, high alert threshold, outdated runbook), Actions Vague ("add monitoring" without owner, deadline, or success metric — "improve testing" is a wish, not an action item. "[@alice] [By: 2024-03-15] [Deploy connection pool metric alert at 80% threshold] [Success: alert fires in staging within 30 seconds of threshold breach]" is actionable. Every action item without ODAS (Owner-Deadline-Action-Success) will be forgotten), and Pattern Ignored (treating every incident as unique without cross-referencing history — "first time this happened" requires evidence from the incident database. Same service in 6 months? Same root cause type? Same deploy window? Same team? If no incident database exists, that IS the first action item). Call once per incident postmortem or root cause analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Incident Postmortem Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Our API went down for 2 hours last Tuesday. The database connection pool was exhausted. We added monitoring."

**🤖 AI Agent:**
> Verdict: ACTIONS_UNACCOUNTABLE + ROOT_CAUSE_SHALLOW. 'Added monitoring' has no owner, no deadline, no success metric. 'Connection pool exhausted' is the symptom. WHY was it exhausted? Leaked connections? Missing pool size tuning? N+1 queries from a new deployment?

---

**👤 You:**
> "The deploy at 14:00 caused a 500 error spike. John rolled back at 14:45. Problem solved."

**🤖 AI Agent:**
> Verdict: TIMELINE_INCOMPLETE. 45 minutes between deploy and rollback — what happened at 14:01? 14:15? When was the alert fired? Who was paged? What was the blast radius? A timeline needs minute-by-minute entries, not just start and end.

---

**👤 You:**
> "Root cause: the engineer forgot to update the config file before deploying."

**🤖 AI Agent:**
> Verdict: ROOT_CAUSE_SHALLOW. 'Forgot to update config' is blame, not root cause. Systemic question: WHY is config managed manually? WHY does the deploy pipeline not validate config? WHY is there no pre-deploy diff check? The root cause is the absence of automated config validation.


## ❓ FAQ

**Q: What makes a timeline 'complete'?**
Minute-by-minute entries from first alert to full resolution. Each entry: [HH:MM] [Actor] [Action] [Outcome]. 'Around 3 PM' is rejected. '15:03 — PagerDuty alert fired for p95 > 2s on /api/orders' is accepted.

**Q: How deep should the 5 Whys analysis go?**
Until you reach a SYSTEMIC root — not a human error. 'Bob forgot to restart' is blame. 'The deployment pipeline has no post-deploy health check' is a system fix. The 5th Why should expose a process, architecture, or policy gap.

**Q: What makes an action item 'accountable'?**
Three requirements: (1) Named owner — not 'the team'. (2) Deadline — not 'soon'. (3) Success metric — not 'improved'. Example: 'Owner: @maria, Deadline: 2024-02-15, Metric: p95 latency < 500ms for 7 consecutive days.'


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/incident-postmortem-prover](https://vinkius.com/mcp/incident-postmortem-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Incident Postmortem Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `incident-postmortem-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Incident Postmortem Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "incident-postmortem-prover": {
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
