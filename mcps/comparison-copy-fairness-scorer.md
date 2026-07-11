# Comparison Copy Fairness Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/comparison-copy-fairness-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [compliance](../categories/compliance.md)

Audit marketing copy and comparison tables for claim verifiability, feature balance, and disparagement risk.

## Description
The Comparison Copy Fairness Scorer is an automated auditor designed to ensure marketing materials are verifiable, balanced, and legally safe. It analyzes competitor-comparison copy using `analyze_claim_verifiability` to check the ratio of quantified claims versus unsupported superlatives. The tool also assesses feature parity between products using `calculate_feature_balance`, measures superlative density with `measure_superlative_intensity`, validates visual symmetry in comparison tables via `validate_table_symmetry`, and identifies potential legal liabilities through `audit_disparagement_risk` by flagging negative claims that lack necessary qualifying language.

### Available Tools

`calculate_copy_fairness`


## Available Tools (1)
- **calculate_copy_fairness**: Calculate a fairness score between two text copies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Comparison Copy Fairness Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this marketing text for fairness: 'Our product is the best on the market, while CompetitorX is slow and unreliable.'"

**🤖 AI Agent:**
> Analysis complete. High Disparagement Risk detected: 'is slow and unreliable' lacks qualifying language. Superlative Density is high due to 'the best'.

---

**👤 You:**
> "Check the feature balance between these two lists: My Product (Battery, Screen, Camera) vs Competitor (Battery, Screen)."

**🤖 AI Agent:**
> The `calculate_feature_balance` tool reports a parity gap of 1. The balance score is reduced because your product lists more features than the competitor.

---

**👤 You:**
> "Is this comparison table symmetric? Row 1: Feature A (Check, X), Row 2: Feature B (Check, Check)."

**🤖 AI Agent:**
> The `validate_table_symmetry` tool detected an imbalance. The distribution of checkmarks and x-marks is uneven across the columns.


## ❓ FAQ

**Q: What does the verifiability ratio measure?**
It compares claims supported by specific numbers, dates, or sources against unsupported superlatives like '#1' or 'the best'. Tools available: `calculate_copy_fairness`.

**Q: How is feature balance calculated?**
The `calculate_feature_balance` tool assesses if the number of features highlighted for your product matches those presented for the competitor to prevent intentional skewing.

**Q: Can this tool detect legal risks in advertising?**
Yes, using `audit_disparagement_risk`, the system flags negative statements about competitors that lack qualifying language like 'may' or 'in most cases'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/comparison-copy-fairness-scorer](https://vinkius.com/mcp/comparison-copy-fairness-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Comparison Copy Fairness Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `comparison-copy-fairness-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Comparison Copy Fairness Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "comparison-copy-fairness-scorer": {
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
