# Insurance Deductible Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/insurance-deductible-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare insurance policy costs by evaluating premiums, deductibles, and risk scenarios.

## Description
This MCP server provides tools to evaluate the financial impact of different insurance policy structures. Users can use `compare_policy_scenarios` to see the cost difference between no-claim and claim scenarios, `evaluate_risk_exposure` to calculate expected annual costs based on claim probability, and `find_optimal_policy` to identify the most cost-effective option among multiple choices. It also includes `calculate_coverage_gap` to determine if a policy's limit is sufficient for an expected loss.


## Available Tools (4)
- **compare_policy_scenarios**: 
- **evaluate_risk_exposure**: 
- **find_optimal_policy**: 
- **calculate_coverage_gap**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Insurance Deductible Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare a policy with a $500 premium, $200 deductible, $5000 limit, and an expected loss of $1000."

**🤖 AI Agent:**
> The no-claim cost is $500 and the claim cost is $700.

---

**👤 You:**
> "Which policy is better: Policy A ($100 premium, $500 deductible) or Policy B ($200 premium, $100 deductible), assuming a 10% claim probability and $1000 expected loss?"

**🤖 AI Agent:**
> Policy A is the better choice with an expected annual cost of $140.

---

**👤 You:**
> "If my coverage limit is $2000 and the expected loss is $2500, how much is the gap?"

**🤖 AI Agent:**
> The coverage gap is $500.


## ❓ FAQ

**Q: How does the tool calculate the cost of a claim?**
The claim cost is the sum of the annual premium and the policyholder's responsibility, which is the lesser of the deductible or the actual claim size.

**Q: Can I compare multiple policies at once?**
Yes, you can use `find_optimal_policy` to compare a list of different policy configurations and identify the one with the lowest expected annual cost.

**Q: What is a coverage gap?**
A coverage gap occurs when the expected loss exceeds the insurance coverage limit. You can use `calculate_coverage_gap` to find this specific amount.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/insurance-deductible-comparator](https://vinkius.com/en/ai-agent-connect/insurance-deductible-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Insurance Deductible Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `insurance-deductible-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Insurance Deductible Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "insurance-deductible-comparator": {
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
