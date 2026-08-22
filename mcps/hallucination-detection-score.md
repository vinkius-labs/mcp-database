# Hallucination Detection Score MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/hallucination-detection-score)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-safety](../categories/ai-safety.md)

Quantify the reliability of AI agent outputs using deterministic hallucination scoring.

## Description
This MCP server provides a deterministic framework for measuring the accuracy and reliability of AI agent responses. By comparing agent outputs against a verified knowledge base and consensus from other agents, it calculates a precise hallucination probability and confidence score. Use `analyze_claim_accuracy` to get a full risk assessment, `extract_fact_claims` to isolate individual assertions, or `calculate_consensus_metrics` to check agreement with peer outputs.


## Available Tools (3)
- **analyze_claim_accuracy**: Evaluate truthfulness and consensus
- **calculate_consensus_metrics**: Compare claims against peer outputs
- **extract_fact_claims**: Isolate individual assertions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hallucination Detection Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this text for hallucinations: 'The capital of France is Lyon and it is known for its pizza.'"

**🤖 AI Agent:**
> The output has a High Risk level. The claim that Lyon is the capital of France is incorrect; the capital is Paris.

---

**👤 You:**
> "Extract the fact claims from: 'The sun is a star and it provides energy to Earth.'"

**🤖 AI Agent:**
> 1. The sun is a star. 2. The sun provides energy to Earth.

---

**👤 You:**
> "Check the consensus for the claim 'The moon orbits the Earth' against the peer output 'The Earth orbits the Sun'."

**🤖 AI Agent:**
> The agreement ratio is 0.0, as the peer output does not support the specific claim about the moon's orbit.


## ❓ FAQ

**Q: How is the hallucination probability calculated?**
The probability is a weighted metric: 50% for claims verified by the reference knowledge base, 30% for consensus with other agents, and 20% for claims with source attribution.

**Q: What is the difference between verified claims and consensus?**
Verified claims are checked against a provided ground truth (knowledge base), while consensus (cross-agent agreement) measures how much the output aligns with other agents' responses on the same topic.

**Q: Can I use this to check specific assertions?**
Yes, you can use the `extract_fact_claims` tool to break down a text block into individual, testable assertions for granular analysis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/hallucination-detection-score](https://vinkius.com/ai-agent-connect/hallucination-detection-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hallucination Detection Score** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hallucination-detection-score` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hallucination Detection Score** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hallucination-detection-score": {
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
