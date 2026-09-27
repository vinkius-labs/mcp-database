# Deductible Claim Decision Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/deductible-claim-decision-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Evaluates whether to file an insurance claim or pay for repairs out-of-pocket.

## Description
This MCP server provides decision-support tools to help users navigate insurance repairs. By using `calculate_claim_feasibility`, users can determine if a repair is covered. The `evaluate_financial_impact` tool compares the costs of self-paying versus filing a claim, including potential premium increases. Finally, `generate_decision_worksheet` provides a clear recommendation based on whether the user wants to minimize immediate expenses or long-term costs. It also includes `check_claim_history_constraints` to ensure policy compliance.


## Available Tools (4)
- **calculate_claim_feasibility**: Determines if a specific repair is eligible for coverage based on the provided policy terms and estimate
- **check_claim_history_constraints**: Validates if the user has sufficient "claim headroom" or if a new claim would violate policy terms regarding frequency
- **evaluate_financial_impact**: Compares the financial outcomes of filing a claim versus paying out-of-pocket
- **generate_decision_worksheet**: Produces a finalized recommendation and a list of next actions for the user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deductible Claim Decision Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a repair estimate of $1200, a $500 deductible, and a $2000 policy limit. Is this covered?"

**🤖 AI Agent:**
> Yes, the repair is covered. The potential payout from your insurer would be $700.

---

**👤 You:**
> "Should I pay $800 out-of-pocket or file a claim with a $300 deductible and a $100 premium increase?"

**🤖 AI Agent:**
> Filing a claim is the better option. The total cost of the claim is $400, which is $400 less than paying $800 out-of-pocket.

---

**👤 You:**
> "I've filed 2 claims this year and my limit is 3. Can I file another one?"

**🤖 AI Agent:**
> Yes, you are eligible to file one more claim before reaching your policy limit.


## ❓ FAQ

**Q: How does the engine decide between a claim and self-pay?**
The engine uses `evaluate_financial_impact` to compare the total cost of paying out-of-pocket against the net cost of a claim, which includes the deductible and projected premium increases.

**Q: Can I check if my policy allows another claim?**
Yes, the `check_claim_history_constraints` tool validates your current claim count against the maximum claims allowed by your policy.

**Q: What information do I need to provide?**
You will need your repair estimate, deductible amount, policy limits, and any estimated increases in insurance premiums.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/deductible-claim-decision-engine](https://vinkius.com/en/ai-agent-connect/deductible-claim-decision-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deductible Claim Decision Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deductible-claim-decision-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deductible Claim Decision Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deductible-claim-decision-engine": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
