# Hallucination Detector Prover MCP Server

LLMs present fabricated information as fact. This tool forces epistemic rigor: cite verifiable sources for every claim, quantify confidence per assertion, separate facts from opinions, declare knowledge boundaries, and cross-reference for internal contradictions.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hallucination-detector-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

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


## Installation & Usage

To install and use the **Hallucination Detector Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hallucination-detector-prover](https://vinkius.com/mcp/hallucination-detector-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
