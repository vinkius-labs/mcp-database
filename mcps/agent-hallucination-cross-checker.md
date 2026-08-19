# Agent Hallucination Cross-Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-hallucination-cross-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audit](../categories/audit.md)

A deterministic engine to audit agent outputs by measuring consensus, source validity, and semantic contradictions.

## Description
This MCP server provides a deterministic verification engine designed to audit multiple agent outputs. It identifies hallucinations by measuring consensus, source validity, and semantic contradictions. Using tools like `verify_claim_consensus`, `detect_hallucinations`, and `analyze_agreement_depth`, it calculates fact consistency scores, detects contradictions between high-confidence claims, and determines the probability of hallucinations. It is built to distinguish between total agreement, partial agreement, and outright contradictions to ensure high-fidelity agent interactions.


## Available Tools (3)
- **analyze_agreement_depth**: Breaks down the nature of agent interactions to distinguish between total agreement, partial agreement, and contradictions
- **detect_hallucinations**: Identifies specific claims that are likely to be hallucinations based on probabilistic modeling and contradiction detection
- **verify_claim_consensus**: Calculates the overall reliability of the provided agent outputs through consistency and source metrics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Hallucination Cross-Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these agent outputs for consistency: [{'agentId': 'A', 'claim': 'The sky is blue', 'confidence': 0.9, 'source': 'ref_1'}, {'agentId': 'B', 'claim': 'The sky is blue', 'confidence': 0.8, 'source': 'ref_1'}]"

**🤖 AI Agent:**
> The fact consistency score is 1.0, as both agents provided identical claims with valid sources.

---

**👤 You:**
> "Check for contradictions in these claims: [{'agentId': 'A', 'claim': 'The temperature is rising', 'confidence': 0.9, 'source': 'ref_1'}, {'agentId': 'B', 'claim': 'The temperature is falling', 'confidence': 0.85, 'source': 'ref_1'}]"

**🤖 AI Agent:**
> A contradiction was detected because the claims are semantic opposites and both agents reported confidence above 0.7.

---

**👤 You:**
> "Calculate the consensus for these outputs with a minimum quorum of 2."

**🤖 AI Agent:**
> The consensus report shows that the required quorum has been met for the verified facts.


## ❓ FAQ

**Q: How does the engine detect hallucinations?**
The engine calculates a hallucination probability for each claim by analyzing source validity, cross-agent agreement, and confidence calibration.

**Q: What is a verification quorum?**
A verification quorum is the minimum number of independent agents that must agree on a single fact before it is considered verified.

**Q: Can it distinguish between partial agreement and contradictions?**
Yes, using `analyze_agreement_depth`, the engine can distinguish between total agreement, partial agreement (same entity, different attributes), and semantic contradictions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-hallucination-cross-checker](https://vinkius.com/ai-agent-connect/agent-hallucination-cross-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Hallucination Cross-Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-hallucination-cross-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Hallucination Cross-Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-hallucination-cross-checker": {
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
