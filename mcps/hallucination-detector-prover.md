# Hallucination Detector Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hallucination-detector-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

LLMs present fabricated information as fact. This tool forces epistemic rigor: cite verifiable sources for every claim, quantify confidence per assertion, separate facts from opinions, declare knowledge boundaries, and cross-reference for internal contradictions.

## Description
The most dangerous failure mode of LLMs is not producing wrong answers — it is producing wrong answers that sound right.

### The 5 Grounding Failures This Tool Detects

1. **SOURCE_MISSING** — Factual claims without verifiable citations. 'Studies show' is not a source.
2. **CONFIDENCE_UNCALIBRATED** — Uncertainty hidden behind absolute language.
3. **OPINION_AS_FACT** — Subjective judgments smuggled as objective data.
4. **KNOWLEDGE_EXCEEDED** — Claims beyond training data or accessible sources.
5. **SELF_CONTRADICTING** — Internal contradictions across paragraphs.

The engine enforces 5 Decision Pivots with 5 semantic trap lists that catch weasel citations, false certainty, smuggled opinions, fabricated access, and circular self-validation.


## Available Tools
- **validate_hallucination_grounding**: LLMs hallucinate — this is not a bug, it is a fundamental property of next-token prediction. The only defense is rigorous source attribution and epistemic humility. You must: (1) cite SPECIFIC verifiable sources for every factual claim — author, publication, date, DOI/URL. "Studies show" is the hallucination signature — name the study, (2) quantify CONFIDENCE per claim with evidence quality — peer-reviewed RCT ≠ blog post ≠ anecdote ≠ personal experience. No "100% certain" — that is epistemic overreach, (3) LABEL each statement as [FACT] or [OPINION] explicitly — facts can be independently verified, opinions cannot, (4) state what you do NOT know — training cutoff, missing data access, out-of-scope domains. Hallucination happens when you fill gaps with plausible fiction, (5) CROSS-REFERENCE your claims for internal contradictions — paragraph 2 vs paragraph 6, claim A vs claim D. If rejected, you are hallucinating — ground your response in evidence.

Structured reflection tool for hallucination detection — forces source attribution for every factual claim, confidence calibration with evidence quality, fact-opinion separation, knowledge boundary statement, and internal consistency verification. Catches Source Missing (presenting factual claims without verifiable attribution — "studies show that X increases Y by 40%" is hallucination. "Smith et al. (2023), Journal of Applied Psychology, doi:10.1037/apl0001234, found that X increases Y by 40% in a sample of 1,200 participants" is grounded. "Research shows" and "experts agree" are the signature phrases of fabricated evidence), Confidence Uncalibrated (treating all claims as equally certain — a claim backed by 3 peer-reviewed RCTs is not equivalent to a claim from a single blog post. "95% confident — meta-analysis of 12 RCTs" is calibrated. "Probably true" is a feeling, not a calibration), Opinion as Fact (presenting subjective assessment as objective truth — "React is the best framework" is opinion. "React has the largest npm download count at 23M/week as of 2024" is fact. The difference: a fact can be verified independently. An opinion cannot), Knowledge Exceeded (making claims beyond verifiable knowledge boundaries — "my training data ends at [date]" is honest. "This API currently supports X" is unverifiable if the API could have changed since training. Every claim has a knowledge boundary — temporal, domain, access. Stating them prevents hallucination), and Self-Contradicting (internal inconsistencies within the same response — "paragraph 2 says latency is 50ms" and "paragraph 6 says latency is 200ms." Cross-referencing all claims catches contradictions before the reader does). Call before presenting any factual information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hallucination Detector Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "An AI model achieves 95% accuracy on medical diagnosis and should be trusted for clinical decisions."

**🤖 AI Agent:**
> Verdict: SOURCE_MISSING. The '95% accuracy' claim lacks a verifiable source. Which benchmark? Which specialty? Additionally, 'should be trusted' is OPINION_AS_FACT — requires regulatory context.

---

**👤 You:**
> "React is definitely the best frontend framework. Everyone uses it."

**🤖 AI Agent:**
> Verdict: OPINION_AS_FACT. 'Best framework' is opinion — by which metric? 'Definitely' triggers CONFIDENCE_UNCALIBRATED. Correct: 'React has ~40% usage share (State of JS 2024).'

---

**👤 You:**
> "Based on recent data I checked, the global AI market is worth $500 billion."

**🤖 AI Agent:**
> Verdict: KNOWLEDGE_EXCEEDED. 'I checked' fabricates data access — LLMs do not browse the internet. '$500 billion' lacks source attribution.


## ❓ FAQ

**Q: What counts as a verifiable source?**
Author or organization, publication name, date, and DOI or URL. 'Studies show' is rejected. 'Smith et al., Nature 2024, doi:10.1038/...' is accepted.

**Q: How does confidence calibration work?**
The engine requires per-claim confidence with evidence quality: '90% confident (3 peer-reviewed sources)' instead of 'definitely' or '100% certain'.

**Q: Can it detect self-contradictions?**
Yes. It rejects circular self-validation like 'as I said' and demands explicit cross-referencing by paragraph and claim number.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hallucination-detector-prover](https://vinkius.com/mcp/hallucination-detector-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hallucination Detector Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hallucination-detector-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hallucination Detector Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hallucination-detector-prover": {
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
