# Deep Analyst Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deep-analyst-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

AI gives surface analysis — restates the question, misses hidden assumptions, uses single-lens thinking. This tool forces multi-model depth: First Principles decomposition, Second-Order cascades (3 levels), Steelmanning (Ideological Turing Test), Inversion, and Premortem risk mapping....

## Description
AI models give surface-level analysis. They restate the question instead of decomposing it, miss hidden assumptions, use single-lens thinking, fail to stress-test from the opponent's view, see only first-order effects, and produce generic conclusions that could apply to any problem.

### The Problem

AI analysis fails on seven axes:

- **Surface analysis** — restates "how should we price?" as "pricing is important" without decomposing into sub-problems.
- **Hidden assumptions** — doesn't surface the beliefs that, if wrong, invalidate the entire analysis.
- **Single-model thinking** — applies one lens when 3+ mental models would reveal completely different insights.
- **No opposition** — doesn't steelman the opposing view. Strawman ("some might say") is not steelman.
- **Cascade blindness** — sees immediate effects but misses Level 2 and Level 3 consequences.
- **No risk mapping** — skips premortem analysis that makes risks 30% more identifiable (Klein, 2007).
- **Generic conclusion** — summary instead of synthesis. Repeats what was said instead of combining models into a novel insight.

### How It Works

6 Decision Pivots force genuine intellectual depth:

1. **decomposed** — Problem broken into 3-5 atomic sub-problems? Not just restated?
2. **assumptionsExplicit** — 3-5 load-bearing assumptions listed with "if wrong" consequences?
3. **multiModelApplied** — 3+ mental models stacked? First Principles + Second-Order + Inversion minimum?
4. **oppositionSteelmanned** — STRONGEST case against your conclusion? Ideological Turing Test?
5. **cascadesIdentified** — "And then what?" 3 levels deep? L1 → L2 → L3?
6. **risksPremortem** — "It failed spectacularly. Why?" 3+ specific failure paths?


## Available Tools (1)
- **validate_deep_analysis**: The goal is to produce analysis that a domain expert would find genuinely insightful, not a structured restatement of the question. You must: (1) DECOMPOSE — break the problem into 3-5 atomic sub-problems using First Principles. Strip convention: "we do it this way because everyone does" is not an answer. Each sub-problem must be independently analyzable, (2) SURFACE ASSUMPTIONS — list 3-5 load-bearing beliefs with consequences if wrong. "If this assumption is wrong, EVERYTHING collapses." Focus on: stability assumptions (what will not change?), motivation assumptions (how will people behave?), prediction assumptions (what will happen?), (3) MULTI-MODEL — apply 3+ named mental models: First Principles, Second-Order, Inversion, Opportunity Cost, Circle of Competence. Where models DISAGREE is where the real insight lives. Single-lens analysis is systematic blindness (Munger), (4) STEELMAN — make the STRONGEST case for the opposing view. Ideological Turing Test: could the opponent read your steelman and say "yes, that IS my argument"? Not "some might argue..." — that is a strawman, (5) CASCADE — "and then what?" 3 levels. L1 immediate → L2 what does L1 cause → L3 systemic. 10/10/10 (Welch): what happens in 10 minutes, 10 months, 10 years? Most stop at L1. See L3, (6) PREMORTEM — "It is 12 months later. It failed spectacularly. Why?" (Klein 2007). 3+ specific, plausible, non-obvious failure paths. Prospective hindsight makes risks 30% more identifiable, (7) SYNTHESIZE — combine ALL models into a NOVEL insight that could not emerge from any single model. Synthesis ≠ summary. If your conclusion could apply to any problem, it is not a conclusion. If rejected, your analysis is surface-level.

Structured reflection tool for deep, multi-model intellectual analysis — writing, strategy, decisions, research, brainstorming. Stacks 5+ mental models (Munger, Kahneman, Klein) against the same problem: First Principles decomposition, explicit assumptions, Second-Order cascades (3 levels deep), Steelmanning (Ideological Turing Test standard), and Premortem risk mapping. Catches Surface Analysis (restating the question as the answer — "the key challenge is the challenge" without decomposition into atomic sub-problems that can be independently analyzed), Hidden Assumptions (load-bearing beliefs never made explicit — "users want speed" when the real bottleneck is trust, but the speed assumption was never questioned because it felt obvious), Single-Model Thinking (analyzing through one lens only — "economically optimal" without considering behavioral, political, ethical, or temporal dimensions. Single-lens = systematic blindness), Strawman Opposition ("some might argue..." — presenting a weak version of the counterargument. Steelman: the STRONGEST case against your position, to Ideological Turing Test standard), Cascade Blindness (seeing only L1 consequences — "this will increase efficiency" without tracing L2 "which team gets cut?" and L3 "what institutional knowledge is lost forever?"), and Generic Conclusions (a synthesis that could apply to any problem is not a synthesis — "we should be thoughtful and move carefully" says nothing). Call once per complex analysis, strategic decision, or research synthesis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deep Analyst Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Should we expand our SaaS product into the enterprise market?"

**🤖 AI Agent:**
> Verdict: SURFACE_ANALYSIS. The question is restated, not decomposed. First Principles decomposition: (1) What does 'enterprise' actually mean for our product? (compliance, SSO, audit logs, SLAs). (2) What's our cost structure and how does enterprise change it? (longer sales cycles, dedicated support, SOC2). (3) Willingness to pay? (enterprise pays 5-10x but demands 50x more support). (4) Opportunity cost? (every engineer on enterprise is NOT building SMB features). Decompose into ...

---

**👤 You:**
> "Pricing analysis. Decomposed: (1) cost floor ($12/user), (2) competitor range ($29-$99/user), (3) WTP survey: 68% chose $39, (4) strategic position: premium. Assumptions: market grows 15% YoY (if wrong: smaller TAM). Applied: first principles (cost + margin), second-order (price increase → churn → revenue net effect), inversion (guarantee failure: underprice and attract low-value users). Steelman against premium: 'Freemium captures 10x market share, converts 3-5%, builds network e..."

**🤖 AI Agent:**
> Verdict: ANALYSIS_PROVEN. Decomposed into 4 sub-problems (cost, competitors, WTP, strategy). Assumptions explicit with consequences. Multi-model: first principles + second-order + inversion. Steelman passes Ideological Turing Test (freemium argument is genuinely compelling). Cascades mapped 3 levels (price → base → data disadvantage). Premortem: 3 specific, plausible failure paths. This analysis will withstand scrutiny.

---

**👤 You:**
> "We should hire more engineers to move faster. The best companies hire aggressively. Our competitors are growing their teams. We need to keep up."

**🤖 AI Agent:**
> Verdict: SINGLE_MODEL. Three failures: (1) Reasoning by ANALOGY ('best companies do it', 'competitors do it') instead of First Principles. Strip convention: does more engineers = more speed? Brooks's Law says no — adding people to a late project makes it later. (2) No second-order: hire → onboarding burden → existing team slows → net velocity DROPS for 3-6 months. (3) No inversion: how to guarantee failure? Hire 10 people without clear ownership, duplicate work, communication over...


## ❓ FAQ

**Q: What types of problems is this for?**
ANY complex problem where you need depth beyond surface-level AI output: writing professional reports, making strategic decisions, evaluating business opportunities, synthesizing multi-document research, brainstorming solutions to hard problems, stress-testing proposals, analyzing competitive threats, planning career moves. If the AI's answer to your question could apply to any company or any person, you need this tool.

**Q: What is the Ideological Turing Test?**
When you steelman the opposing view, the test is: could someone who actually holds that opposing view read your steelman and say 'Yes, that's my actual argument'? If they would say 'No, that's a caricature of my position,' you've strawmanned, not steelmanned. True steelmanning requires you to present the opposition's case SO well that you genuinely feel the pull of their argument. This forces intellectual honesty and prevents confirmation bias.

**Q: Why premortem instead of risk analysis?**
Gary Klein's 2007 research showed that prospective hindsight — imagining a future failure and working backward — makes people 30% better at identifying risks compared to traditional forward-looking risk analysis. Traditional risk analysis asks 'what could go wrong?' which triggers defensive thinking. Premortem says 'it already failed — why?' which bypasses ego defenses and unlocks honest assessment of vulnerabilities that people otherwise suppress.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deep-analyst-prover](https://vinkius.com/mcp/deep-analyst-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deep Analyst Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deep-analyst-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deep Analyst Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deep-analyst-prover": {
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
