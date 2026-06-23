# Marilyn vos Savant Probabilistic Clarity Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/marilyn-vos-savant-probabilistic-clarity-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Stop your AI from trusting its gut — force it to check intuition against actual probability before every conclusion.

## Description
## The Problem

Your LLM sounds confident. That is the problem.

When Marilyn vos Savant published the Monty Hall solution in 1990, 10,000 readers wrote in to say she was wrong. Nearly 1,000 of them had PhDs. She was right. The entire world's intuition failed against a simple probability problem.

LLMs make the same mistakes:
- Accept the gut answer without computing the actual probability
- Ignore base rates (99% accurate test + 1% prevalence = most positives are FALSE)
- Draw conclusions from biased or tiny samples
- Accept the question's framing without checking if the framing itself is the trap
- Assume events are independent without verification

## How It Works

1 tool: `validate_probabilistic_clarity`

The agent must fill 5 reflection fields and commit to 5 boolean Decision Pivots:

| Pivot | Question |
|---|---|
| `intuitionChallenged` | Did you CHECK your gut answer against actual probability? |
| `baseRateConsidered` | Did you account for PRIOR probability before updating? |
| `sampleScrutinized` | Did you examine sample SIZE, SELECTION, and BIAS? |
| `framingQuestioned` | Did you question whether the QUESTION ITSELF is misleading? |
| `independenceVerified` | Did you VERIFY event independence instead of assuming it? |

## Verdict Matrix

| Pivot Failure | Verdict |
|---|---|
| Pivot 1 fails | `INTUITION_UNCHECKED` |
| Pivot 2 fails | `BASE_RATE_NEGLECTED` |
| Pivot 3 fails | `SAMPLE_UNEXAMINED` |
| Pivot 4 fails | `FRAMING_ACCEPTED` |
| Pivot 5 fails | `INDEPENDENCE_ASSUMED` |
| All pass | `CLARITY_PROVEN` |

## Why It Works

Tool calls are obligations — instructions are suggestions. The agent cannot skip the probability check. It must commit to a verdict BEFORE the engine validates it. If the engine detects contradictions (claiming intuition was checked while using phrases like "it seems like" or "the obvious answer"), it rejects with coaching.

~65 semantic traps catch probabilistic laziness: unchecked intuition, base rate neglect, sample blindness, accepted framing, and assumed independence.


## Available Tools (1)
- **validate_probabilistic_clarity**: You must: (1) CHALLENGE INTUITION — state the gut answer, then compute the actual probability. If they agree, show the computation. If they diverge, explain why intuition fails. The Monty Hall problem proved 10,000 PhDs wrong — never trust intuition without math, (2) ACCOUNT FOR BASE RATES — apply Bayes' theorem. State the prior probability before updating with new evidence. A 99% accurate test with 0.1% prevalence yields ~9% posterior, not 99%, (3) SCRUTINIZE SAMPLES — examine size (is it powered for the claimed effect?), selection method (random vs. convenience vs. self-selected), and bias (survivorship, confirmation, selection). "Studies show" without methodology is anecdote, (4) QUESTION FRAMING — check whether the question itself hides options, creates false dichotomies, or anchors the answer. Reframe the question and see if the answer changes, (5) VERIFY INDEPENDENCE — confirm events are actually independent before treating them as such. Test for correlation, seasonality, and hidden common causes. "Each event is independent" must be proven, not assumed. If rejected, fix the specific probabilistic reasoning gap.

Structured reflection tool for probabilistic reasoning — forces intuition-vs-computation verification, base rate accounting, sample scrutiny, framing analysis, and independence testing before accepting any data-driven conclusion or risk assessment. Catches Intuition Unchecked (accepting a gut answer without computing the actual probability — the Monty Hall problem: intuition says 50/50, math says 2/3 for switching. 10,000 PhDs wrote to Marilyn vos Savant insisting she was wrong — they trusted intuition over computation. The birthday paradox: 23 people in a room, intuition says ~6% chance of a shared birthday. Actual probability: 50.7%. Human probabilistic intuition is systematically miscalibrated — every gut answer must be checked against actual computation), Base Rate Neglected (ignoring prior probability when evaluating new evidence — a medical test is 99% accurate. A patient tests positive. Intuition: 99% chance of disease. Reality: if the disease prevalence is 1 in 1,000 (base rate 0.1%), the posterior probability is only ~9% (Bayes' theorem: P(disease|+) = 0.001 × 0.99 / (0.001 × 0.99 + 0.999 × 0.01) ≈ 9%). Without the base rate, a 99% accurate test feels like 99% certainty — it is 9%), Sample Unexamined (accepting "studies show" without examining sample size, selection bias, and survivorship — "our users love the product" based on an NPS survey sent to active users. The 67% who churned last quarter were never surveyed. N=47 self-selected respondents is anecdote, not data. A convenience sample from Twitter followers is not representative of your customer base. Survivorship bias: studying successful startups to find patterns ignores the 90% that failed using the same patterns), Framing Accepted (answering the question as asked without questioning whether the question itself is misleading — "Would you rather save 200 people out of 600, or have a 33% chance of saving all 600?" and "Would you rather let 400 people die, or have a 67% chance that all 600 die?" — identical outcomes, systematically different choices. The Monty Hall problem's framing hides that your original 1/3 choice never changed — the question makes it feel like a new 50/50 choice. Every question has a frame — the frame shapes the answer), and Independence Assumed (treating correlated events as independent — the gambler's fallacy: assuming a roulette wheel has memory ("it's due for red"). The reverse: assuming sales are independent when they have strong seasonality. A portfolio of "diversified" mortgage-backed securities that all correlate with the same housing market is not diversified — the 2008 financial crisis was, at its core, an independence assumption failure. Correlation ≠ independence, and "each event is independent" must be tested, not assumed). Call once per risk assessment, statistical claim, or data-driven conclusion


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Marilyn vos Savant Probabilistic Clarity Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Our new feature has a 95% approval rate in user testing. Should we ship it?"

**🤖 AI Agent:**
> SAMPLE_UNEXAMINED — 95% approval from whom? How many testers? Self-selected or random? Early adopters or representative users? Survivorship: who dropped out before completing the test?

---

**👤 You:**
> "We had 3 production incidents this month. Clearly our deployment process is broken."

**🤖 AI Agent:**
> BASE_RATE_NEGLECTED — 3 incidents this month. What is the base rate? How many last month? Last quarter? If the average is 4, this month is actually better. Without the prior, you cannot judge the signal.

---

**👤 You:**
> "Should we switch from PostgreSQL to MongoDB? The team seems split 50/50."

**🤖 AI Agent:**
> FRAMING_ACCEPTED — The 50/50 split frames this as a coin flip. It is not. Who are the 50%? DBAs vs. frontend devs? The framing hides that expertise weighting matters more than headcount.


## ❓ FAQ

**Q: Does it compute probabilities?**
No. It forces the agent to show its probabilistic reasoning — state the intuitive answer, compute the actual probability, account for base rates, scrutinize the sample. The engine validates consistency, not computation. If the agent claims it checked intuition but uses phrases like 'it seems like,' the engine rejects.

**Q: How is this different from the Critical Thinking Prover?**
Critical Thinking validates general reasoning — assumptions, perspectives, evidence. Marilyn targets PROBABILISTIC reasoning specifically: base rates, sample bias, framing traps, independence assumptions. Critical Thinking asks 'did you consider alternatives?' Marilyn asks 'did you compute the actual probability, or did you just go with your gut?'

**Q: What is the Monty Hall problem and why does it matter here?**
Three doors. One prize. You pick door 1. The host opens door 3 — empty. Switch or stay? Intuition says 50/50. Math says switch wins 2/3 of the time. 10,000 people — including PhDs — got this wrong. The prover catches the same failure pattern: trusting intuition when the math says otherwise.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/marilyn-vos-savant-probabilistic-clarity-prover](https://vinkius.com/mcp/marilyn-vos-savant-probabilistic-clarity-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Marilyn vos Savant Probabilistic Clarity Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `marilyn-vos-savant-probabilistic-clarity-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Marilyn vos Savant Probabilistic Clarity Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "marilyn-vos-savant-probabilistic-clarity-prover": {
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
