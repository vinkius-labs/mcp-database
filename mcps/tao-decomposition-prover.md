# Tao Decomposition Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tao-decomposition-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [architecture](../categories/architecture.md)

A team attempted a big-bang credential migration — paper to digital — in one cycle. A 4,200-item package touched policy, intake, forms, and field protocols. Went live Thursday 5pm. By 3am Friday, field staff could not verify credentials: the new process rejected submissions using the old paper form still distributed during migration. Tao did not attack the Green-Tao theorem as a monolith. He decomposed it into 3 sub-problems across 3 fields. This tool forces that discipline: decompose, collaborate across perspectives, cross domains, show reasoning, maintain rigor.

## Description
AI agents attack complex problems as monoliths. They solve in isolation when collaboration would unlock blind spots. They stay in one domain when the problem spans several. They present conclusions without showing their reasoning. They say 'it should work' instead of proving it.

### The Problem

LLMs commit five decomposition failures:

- **Decomposition Absent** — 'We will do a complete overhaul in one cycle.' Tao and Green did not attack the primes-in-arithmetic-progressions conjecture head-on. They decomposed it into 3 tractable pieces: Szemerédi regularity (structure), transference principle (density bridging), and sieve methods (prime distribution). Each was solvable individually. Together, they proved what decades of monolithic attempts could not.
- **Collaboration Missing** — 'I will handle it myself.' Tao pioneered Polymath projects — massively collaborative mathematics where dozens of mathematicians contribute openly. Polymath1 proved the density Hales-Jewett theorem in 6 weeks. Tao has published with 70+ co-authors. Who else has looked at your solution? Whose perspective are you missing — legal, financial, operational, compliance, field staff?
- **Domains Uncrossed** — 'This is purely an administrative problem.' Tao works in number theory AND harmonic analysis AND PDE AND combinatorics AND random matrix theory AND compressed sensing. The Green-Tao theorem required THREE different mathematical fields — no single domain contained the answer. Is your migration really just an administrative problem, or does it touch field operations, client communications, regulatory compliance, training?
- **Progress Opaque** — 'Trust me on this. The answer is clearly digital-first.' Tao maintains a blog with 300+ posts showing WORK-IN-PROGRESS thinking — partial results, failed approaches, open questions. He does not present conclusions without reasoning. What alternatives did YOU consider? What did you try that failed? What remains uncertain?
- **Rigor Abandoned** — 'It should work. Probably fine.' Tao won the Fields Medal for proofs that are PRECISELY correct — every step verifiable. 'Should work' is not a proof. What is your specific claim? What evidence supports it? How can someone independently verify? What gaps remain?

### How It Works

5 Decision Pivots following Tao's methodology:

1. **decompositionComplete** — At least 3 sub-problems with interfaces and ordering.
2. **collaborationStructured** — Perspectives, contributions, reviews, blind spots.
3. **domainsCrossed** — Adjacent domains identified, techniques borrowed, cross-validated.
4. **progressVisible** — Steps shown, alternatives rejected with reasons, failures documented.
5. **rigorMaintained** — Claims evidenced, independently verifiable, gaps acknowledged.

### The Verdict Matrix

| First Failing Pivot | Verdict | Meaning |
|---|---|---|
| decompositionComplete = false | DECOMPOSITION_ABSENT | Attacking a monolith. |
| collaborationStructured = false | COLLABORATION_MISSING | Solving in isolation. |
| domainsCrossed = false | DOMAINS_UNCROSSED | Single-domain thinking. |
| progressVisible = false | PROGRESS_OPAQUE | Conclusions without reasoning. |
| rigorMaintained = false | RIGOR_ABANDONED | "Should work" instead of proof. |
| All pivots pass | DECOMPOSITION_PROVEN | Decomposed. Collaborative. Cross-domain. Visible. Rigorous. |


## Available Tools (1)
- **validate_tao_decomposition**: You must: (1) DECOMPOSE — break the monolith into at least 3 tractable sub-problems with clear interfaces, (2) COLLABORATE — identify whose expertise is needed and what blind spots you have, (3) CROSS DOMAINS — borrow techniques from adjacent fields and validate from multiple perspectives, (4) SHOW PROGRESS — document intermediate reasoning, rejected alternatives, and failures, (5) MAINTAIN RIGOR — every claim supported with evidence and independently verifiable. If rejected, fix the specific decomposition gap the engine identifies.

Structured reflection tool that forces the LLM to decompose complex problems through the lens of Terence Tao — the Fields Medal laureate (2006) who proved the Green-Tao theorem by decomposing it into 3 sub-problems spanning number theory, harmonic analysis, and combinatorics, then collaborated with 70+ co-authors across his career and led the Polymath Project (distributed mathematical collaboration where 40+ mathematicians solve problems no individual could). Tao does not attack problems head-on — he decomposes, collaborates, crosses domains, shows his work publicly (300+ blog posts with in-progress reasoning), and demands verifiable rigor. Catches Decomposition Absence (attacking a monolithic problem without breaking it into tractable pieces — a city needs to prevent flooding in a river basin. Monolithic approach: "build a dam." One solution. One project. But the flooding is caused by 4 independent factors: upstream deforestation (runoff volume), inadequate storm drainage (urban capacity), riverbed sedimentation (channel depth), and tidal surge from the coast (backflow pressure). A dam addresses upstream volume but ignores urban drainage, sedimentation, and tidal surge. Result: dam costs $200M, flooding continues 3 years later because the real bottleneck was storm drainage at 40% capacity during peak rainfall. Tao approach: decompose into 4 sub-problems with clear interfaces. Sub-problem 1 (hydrology): upstream runoff volume model → feeds dam sizing. Sub-problem 2 (drainage engineering): urban pipe capacity → feeds infrastructure upgrade. Sub-problem 3 (sediment management): river dredging schedule → feeds channel depth. Sub-problem 4 (coastal engineering): tidal barrier design → feeds backflow prevention. Each sub-problem is tractable by a different specialist team. Interfaces are defined. Total cost: $120M (40% less than dam alone) with 95% flood reduction vs dam's 35%), Collaboration Missing (one person/team solving a multi-domain problem alone — a pandemic response team designs a contact tracing system. Team: 5 epidemiologists. They design a mathematically elegant exposure model. Problem: no logistics expert. The model requires testing 50,000 people per day. Current lab capacity: 8,000 tests/day. No supply chain plan for test kits. No behavioral scientist — the model assumes 90% compliance with quarantine, actual: 42%. The epidemiological model is perfect. The implementation is impossible. Tao approach: the Polymath Project succeeds because it incorporates perspectives that no single mathematician possesses. The epidemiologists needed: logistics (lab capacity, supply chain), behavioral science (compliance rates), public health communication (multilingual outreach), and IT (data infrastructure). Rule: if your solution requires expertise you do not have in the room, you are designing a theoretical success and a practical failure), Domain Isolation (staying within one field when the solution requires cross-domain synthesis — a bridge engineer designs a bridge over a river estuary. Structural analysis: flawless. Steel grade, load calculations, wind resistance — all verified. But no geological survey was conducted. Pier 3 is sited on an alluvial clay deposit. 18 months after construction: Pier 3 sinks 30cm. Bridge deck cracks. Repair cost: $45M (60% of original construction cost). The structural engineering was correct. But the problem was not purely structural — it was geological + structural + hydrological (tidal erosion of the clay). Tao's Green-Tao theorem: number theory ALONE could not solve it. He borrowed techniques from harmonic analysis AND combinatorics. Three fields. One theorem. No single field was sufficient. Rule: if your solution only uses techniques from one domain, ask: which adjacent domain could invalidate my assumptions?), Progress Opacity (black-box reasoning without intermediate checkpoints — an archaeological excavation team announces: "We found a Bronze Age settlement." Report: 3 pages. No stratigraphy documentation. No artifact catalog by layer. No photographs of in-situ positions. No rejected hypotheses documented. Peer reviewer: "How do you know it is Bronze Age and not Iron Age?" Team: "We analyzed the pottery." But the pottery analysis is not documented. The conclusion may be correct — but it is unverifiable. Tao writes 300+ blog posts showing work-in-progress — including wrong turns, failed approaches, and reasoning dead-ends. When he publishes a result: the reasoning path is reconstructable by any peer. Rule: if your conclusion cannot be independently verified by reviewing intermediate steps, it is an assertion, not a proof), and Rigor Abandoned (claims without verifiable evidence — a hospital claims: "Our new surgical scheduling protocol reduces wait times." How much? "Significantly." Measured how? "Staff reported improvement." Sample size? "Several departments." Time period? "Recent months." This is not evidence — it is opinion. Rigorous version: "Surgical wait times measured across 4 departments (orthopedics, cardiac, general, neuro) for 1,247 procedures over 6 months. Mean wait: 14.2 days → 9.8 days (−31%). p < 0.001. 95% CI: −28% to −34%. Controlled for: seasonal variation, staffing changes, case complexity (ASA score). Replication: protocol applied to 2 additional hospitals — similar reduction (−27%, −33%)." Every claim has a number. Every number has a source. Every source is independently verifiable. Tao: Fields Medal standard — every step in every proof is verifiable by any qualified mathematician). Call once per complex problem, strategic decision, or multi-faceted analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tao Decomposition Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We need to migrate our credentialing from paper-based to digital. Let us do a complete overhaul in one cycle — I will handle it myself since this is purely an administrative problem. Trust me, digital-first is clearly the right choice. It should work fine."

**🤖 AI Agent:**
> DECOMPOSITION_ABSENT — Five failures in one sentence. 'Complete overhaul in one cycle' — monolith. Tao decomposed the Green-Tao theorem into 3 sub-problems. Where are YOUR sub-problems? Verification standards, migration strategy, intake procedure redesign — at minimum 3 pieces with clear interfaces. 'I will handle it myself' — where is the legal advisor for compliance? The operations lead for field rollout? The training coordinator for staff readiness? The records manager for archival policy? 'Purely an administrative problem' — credentialing touches field operations (verification procedures), client communications (new submission requirements), regulatory compliance (data retention rules), training (staff adoption). 'Trust me, clearly the right choice' — show your reasoning. What about hybrid approaches? Phased rollout? What alternatives did you evaluate? 'Should work' — is this a Fields Medal proof or a guess?

---

**👤 You:**
> "We broke the credential migration into 3 parts: (1) define verification standards, (2) run paper and digital in parallel for 2 weeks with feature flags, (3) redesign intake forms piloted at 5% of offices. Standards first, then migration, then intake. Collaboration: legal reviewed retention (7-year archive), records reviewed indexing, client services designed guided forms, field team caught duplicate risk. Blind spot found: multilingual communications — added to plan. Domains: credentialing, legal, client services, field ops, communications, compliance. Borrowed phased rollout from field ops. Progress: evaluated full digital vs hybrid vs phased. Chose phased (12 comparable cases vs hybrid's 2). First plan reverted after legal flagged retention gaps. Duplicate risk resolved via unique references. Rigor: 247 verification tests, 34 integration tests, 10K concurrent stress test, compliance audit passed. Gap: duplicate detection only tested with 3 offices, not 10+."

**🤖 AI Agent:**
> DECOMPOSITION_PROVEN — Tao Method complete. Decomposition: 3 tractable sub-problems (standards → migration → intake) with clear interfaces, dependency ordering, and feature flags for each. Collaboration: 4 teams contributed (legal: retention rules, records: indexing, client services: guided forms, field: duplicate detection) — blind spot found (multilingual rollout) and resolved. Domains: 6 domains crossed (administration, legal, client services, field operations, communications, compliance) with phased rollout pattern borrowed from field operations. Progress: 4 reasoning steps documented, 2 alternatives rejected with specific reasons (full digital risk, hybrid maintenance burden), 1 failure documented (immediate rollout reverted), 1 open question acknowledged (archival format). Rigor: 281 tests, stress test, compliance audit report, independently verifiable, gap acknowledged (10+ concurrent office testing). This is methodical, collaborative problem-solving.

---

**👤 You:**
> "Decomposition: 3 sub-problems. Collaboration: I will handle it myself — no need to involve others, I already know the answer. Cross-domain: this is purely an administrative problem, the field operations do not matter."

**🤖 AI Agent:**
> COLLABORATION_MISSING — Decomposition passes: 3 sub-problems identified. But collaboration fails: 'I will handle it myself,' 'no need to involve others,' 'I already know the answer.' Tao has 70+ co-authors. Polymath1 solved a theorem in 6 weeks with DOZENS of contributors. Whose legal expertise do you have? Who validates your compliance strategy? Who tests the field integration? What blind spots do you have that you literally cannot see? Additionally: 'purely an administrative problem, field operations do not matter' — domain boundaries uncrossed. Credentialing migration ALWAYS touches field operations (where verification happens), client communications (how submissions are guided), compliance (what records must be retained), and training (how staff adopt the new process).


## ❓ FAQ

**Q: Is this only for complex organizational migrations?**
No. Tao's method applies to any problem with multiple interacting parts — product development (decompose into research + design + prototype + validation), incident resolution (decompose into reproduce + isolate + fix + verify), strategic decisions (decompose into requirements + capabilities + timeline + risk), even project planning (decompose into milestones with dependencies). The key insight: if the problem takes more than one person-week or touches more than one domain, decompose it.

**Q: What if the problem is too small for decomposition?**
If the problem can be solved by one person in one domain in under 4 hours, decomposition adds overhead without value. The engine recognizes this: small, single-domain tasks should be solved directly. The engine is designed for problems that resist direct attack — multi-department transitions, cross-team initiatives, complex incident resolution, strategic decisions. If you can hold the entire problem in your head, you do not need decomposition. If you cannot, you need Tao.

**Q: How does it differ from the Archimedes First Principles Prover?**
Archimedes validates analytical DECOMPOSITION from AXIOMS — recursive reduction to fundamental truths, mathematical proof, leverage identification. It asks 'can you prove this from first principles?' Tao validates collaborative DECOMPOSITION into TRACTABLE PIECES — sub-problems, cross-domain synthesis, collaboration, visible progress, rigor. It asks 'can you break this into solvable pieces and prove each one?' Archimedes decomposes to AXIOMS. Tao decomposes to SOLVABLE SUB-PROBLEMS. Use Archimedes when you need to reach bedrock truth. Use Tao when you need to organize a complex, multi-faceted effort.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tao-decomposition-prover](https://vinkius.com/mcp/tao-decomposition-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tao Decomposition Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tao-decomposition-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tao Decomposition Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tao-decomposition-prover": {
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
