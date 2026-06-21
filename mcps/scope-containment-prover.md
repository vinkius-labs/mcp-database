# Scope Containment Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scope-containment-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [reasoning](../categories/reasoning.md)

AIs over-engineer everything. This engine is a 6-pivot cognitive trap that forces the LLM to apply YAGNI, reject premature optimization, and define the absolute minimum viable product.

## Description
Left unchecked, an LLM will build a microservices architecture for a to-do app. The Scope Containment Prover is a cognitive trap designed to enforce ruthless simplicity and YAGNI (You Aren't Gonna Need It).

### The Semantic Trap

Before writing code, the agent must pass a strict 6-pivot validation:

1. **coreProblemIsolated** — Define the ONE thing this feature must do.
2. **yagniEnforced** — Explicitly reject a 'nice-to-have' addition.
3. **prematureOptimizationRejected** — Explicitly ignore a future scaling concern.
4. **dependenciesMinimized** — Prove we don't need another npm package.
5. **maintenanceCostMapped** — Acknowledge that code is a liability.
6. **mvpDefined** — Define the absolute minimum to ship.


## Available Tools
- **validate_scope_containment**: You must prove discipline across 6 axes: (1) CORE PROBLEM — isolate the ONE thing this must do. Not a wish list — one sentence, one user action, one outcome. Everything else is a separate feature, (2) YAGNI — name the features you are REJECTING. If you cannot name what you are NOT building, you have not constrained the scope, (3) PREMATURE OPTIMIZATION — state the CURRENT scale. Build for that, not for 1000x. Monitor. Optimize when data shows you must, (4) DEPENDENCIES — justify every library. If solvable in < 20 lines: do not add it. Each dependency is a long-term maintenance commitment, (5) MAINTENANCE COST — who maintains this code after you ship it? Test updates, documentation, monitoring, on-call burden. Calculate total cost of ownership, (6) MVP — define the absolute minimum to ship and validate. If your MVP takes more than 2 weeks to build, it is not minimum. If rejected, scope is bloated — cut until it passes.

Structured reflection tool that forces scope discipline before any feature is built — eliminates bloat, YAGNI violations, premature optimization, dependency sprawl, and maintenance debt by forcing the LLM to justify every decision BEFORE code exists. Based on YAGNI (Beck, XP 1999), "Simple Made Easy" (Hickey, 2011), and the observation that 65% of features in enterprise software are rarely or never used (Standish Group CHAOS Report 2020). Catches Problem Blur (solving a vague problem that grows to absorb everything — "Build a file upload feature." What starts as "upload a file" becomes: Week 1: "We should support drag-and-drop." Week 2: "What about multiple files?" Week 3: "Can we preview images before upload?" Week 4: "Users want to edit images inline." Week 5: "We need a media library to manage uploaded files." Week 6: "The media library needs folders and search." What was 2 days of work is now 8 weeks — and the ORIGINAL problem (user uploads a single CSV for data import) is buried under a media management system. The ONE thing: "User selects a CSV file → system validates format → imports rows." That is 2 days. Everything else is a DIFFERENT feature for a DIFFERENT sprint), YAGNI Violation (building for hypothetical future requirements — "We should make the upload handler support any file type — we might need PDFs later." We MIGHT. But right now, the requirement is CSV. Adding PDF support: + 2 days for PDF parsing. + 1 day for PDF validation. + 3 days for PDF preview rendering. + ongoing maintenance for a feature nobody requested. Total cost: 6 days of work for 0 users. "But what if we need it in 3 months?" Then build it in 3 months — when you know the ACTUAL requirements, the actual file sizes, the actual edge cases. Building it now means: guessing the requirements (wrong 60% of the time), maintaining code nobody uses (every unused feature is a maintenance tax), and delaying the feature users ACTUALLY need (the CSV import that was due yesterday)), Premature Optimization (optimizing for scale that does not exist — "We should build the upload pipeline to handle 10 million files." Current users: 47. Expected files per month: ~200. Building for 10M files requires: distributed storage (S3 multipart + CDN), message queue for async processing (SQS/RabbitMQ), worker pool for parallel processing, database sharding for file metadata, caching layer for frequently accessed files. Time: 4 weeks. Complexity: 3 new infrastructure dependencies. Building for 200 files requires: single server, local disk, synchronous processing. Time: 2 days. Complexity: zero new dependencies. "But what if we go viral?" At 200 files/month growing 100% month-over-month, it takes 16 months to reach 10M files. You have 16 months to optimize. Build for 200. Monitor. Optimize when you have data — not guesses), Dependency Bloat (adding libraries for problems solvable in 10 lines of code — "We need moment.js for date formatting." The requirement: display "Jan 15, 2024." moment.js: 300KB minified. 35 transitive dependencies. Abandoned in 2020 (maintenance-only). Native JavaScript: new Date(timestamp).toLocaleDateString("en-US", {month: "short", day: "numeric", year: "numeric"}). Zero dependencies. Zero bundle impact. Zero maintenance debt. Each dependency is a commitment: security patches, breaking changes on major versions, bundle size impact, and a bet that the maintainer will not abandon the project. Left-pad (2016) broke thousands of builds when 1 maintainer unpublished 11 lines of code. Rule: can you solve this in < 20 lines of code? Then do not add a dependency. Exception: complex domains where the library encapsulates genuine expertise (cryptography, date math with timezones, PDF generation)), and Maintenance Amnesia (shipping code without accounting for its long-term cost — "The feature is done! Ship it!" But who maintains it? A feature is not "done" when the code is written — it is done when: tests exist (who updates them when requirements change?), documentation exists (who keeps it current?), monitoring exists (who responds to alerts?), and the on-call rotation knows it exists (who debugs it at 3 AM?). Every feature has a Total Cost of Ownership: Build cost: 5 days. Annual maintenance: 2 days of bug fixes, 1 day of dependency updates, 0.5 days of documentation updates, 0.5 days of monitoring review = 4 days/year. Over 3 years: 5 + 12 = 17 days. The build cost is 29% of the total cost. A team maintaining 50 features: 200 days/year = 1 full-time engineer just on maintenance. Every new feature you ship REDUCES the team's capacity for new work). Call once per new feature, library addition, or scope decision


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scope Containment Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Problem: Auth. YAGNI: none. Opt: none."

**🤖 AI Agent:**
> Verdict: YAGNI_VIOLATION. You must explicitly state what you are choosing NOT to build.

---

**👤 You:**
> "Problem: Button. YAGNI: no animation. Opt: Using Redis for state just in case."

**🤖 AI Agent:**
> Verdict: PREMATURE_OPTIMIZATION. Using Redis 'just in case' is exactly the bloat this trap prevents.

---

**👤 You:**
> "Problem: Send email. YAGNI: Rejecting bulk batching. Opt: Ignoring 1M/day scale. Deps: Using native fetch. Maint: Tiny function. MVP: One API call."

**🤖 AI Agent:**
> Verdict: SCOPE_CONTAINMENT_PROVEN. Perfect MVP isolation.


## ❓ FAQ

**Q: What does YAGNI mean?**
'You Aren't Gonna Need It'. It's the principle of not building features until you actually need them.

**Q: Why force rejection of premature optimization?**
Because optimizing for 1M users when you have 10 adds massive complexity that slows down development.

**Q: Why map maintenance cost?**
Code is a liability, not an asset. Every line written must be read, tested, and updated forever.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scope-containment-prover](https://vinkius.com/mcp/scope-containment-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scope Containment Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `scope-containment-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scope Containment Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scope-containment-prover": {
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
