# Claim Substantiation Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/claim-substantiation-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Scans marketing copy for factual and numeric claims requiring substantiation.

## Description
The Claim Substantiation Checker helps you audit marketing text for regulatory compliance. It uses `unsupported_numerics_check` to find statistics and percentages lacking citations, `comparative_claims_check` to identify superlatives or comparative adjectives that lack a benchmark, and `absolute_statements_check` to flag guarantees missing necessary qualifier language. Finally, the `compliance_scan` tool aggregates all findings to provide an overall substantiation coverage score for your text.


## Available Tools (4)
- **comparative_claims_check**: g., "than...").

Scans text for comparative words without a baseline
- **compliance_scan**: Orchestrates a full compliance scan of the provided text
- **unsupported_numerics_check**: g., "50%" without direction).

Scans text for numeric claims that lack sufficient context or units
- **absolute_statements_check**: g., "typically").

Scans text for absolute statements lacking qualifiers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Claim Substantiation Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check this text: 'Our product is 50% faster and always works.'"

**🤖 AI Agent:**
> The scan found issues: '50%' lacks a citation, 'faster' lacks a benchmark, and 'always' lacks a qualifier.

---

**👤 You:**
> "Is this claim substantiated: '9 out of 10 users prefer us.'"

**🤖 AI Agent:**
> No, the numeric claim '9 out of 10' is missing a source or citation marker.

---

**👤 You:**
> "Analyze this for comparative claims: 'Our software is more efficient than the industry standard.'"

**🤖 AI Agent:**
> The claim 'more efficient' was flagged because it does not specify which industry standard is being used as a benchmark.


## ❓ FAQ

**Q: What does the tool check for?**
It identifies unsupported numeric claims, comparative statements without benchmarks, and absolute promises lacking qualifiers using tools like `unsupported_numerics_check`.

**Q: How is the compliance score calculated?**
The `compliance_scan` tool aggregates findings from all scanning tools to provide a percentage of claims that were properly substantiated.

**Q: Can I use this for social media advertisements?**
Yes, you can paste any marketing text into the tool to check for compliance issues across various platforms.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/claim-substantiation-checker](https://vinkius.com/mcp/claim-substantiation-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Claim Substantiation Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `claim-substantiation-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Claim Substantiation Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "claim-substantiation-checker": {
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
