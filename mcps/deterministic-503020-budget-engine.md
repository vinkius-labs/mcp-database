# Deterministic 50/30/20 Budget Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deterministic-503020-budget-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transform your AI into a hyper-precise financial controller. Mathematically enforce the 50/30/20 budgeting rule on pre-categorized expense pipelines to detect exact capital deviations.

## Description
Asking an LLM to calculate personal or corporate finances is dangerous. AI models frequently miscalculate decimals, drop expenses from large arrays, or hallucinate total percentages. The Budget Engine MCP solves this by offloading strict financial auditing to a hyper-precise V8 mathematical engine.

### The Superpowers
- **Strict 50/30/20 Algorithmic Enforcement:** You map the expenses, and the engine mathematically enforces the golden rule of finance (50% Needs, 30% Wants, 20% Savings/Debt), calculating the exact target capital for your given income.
- **Micro-Precision Deviations:** Generates exact dollar and fractional percentage deviations. It instantly tells you if your 'Wants' category is $250.45 over budget, preventing LLM math hallucinations and allowing immediate tactical corrections.
- **Deficit & Surplus Diagnostics:** Automatically calculates the final monthly surplus or deficit, triggering strict structural alerts ('Deficit' vs 'Healthy') accompanied by algorithmic recommendations.
- **Zero-Dependency Execution:** Operates entirely natively within the V8 runtime, guaranteeing extreme speed and deterministic precision without relying on fragile external financial APIs.


## Available Tools (1)
- **analyze_budget**: You must provide the exact monthly income and a stringified JSON array of categorized expenses.

Instantly applies the 50/30/20 financial rule to an income and expenses list, returning strict algorithmic deviations, percentages, and surplus/deficit health checks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deterministic 50/30/20 Budget Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Here is my mapped list of expenses and $5000 income. Am I over budget on wants?"

**🤖 AI Agent:**
> Using the analyze_budget tool: Yes, the diagnostic shows your 'Wants' category is $200 over budget (`isOverBudget: true`, `deviation: 200`), consuming 34% of your income instead of the required 30%.

---

**👤 You:**
> "Calculate my monthly surplus and health status."

**🤖 AI Agent:**
> Using the analyze_budget tool: Your total income is $4000, and expenses are $3200. You have a monthly surplus of $800, and your budget is structurally 'Healthy'.

---

**👤 You:**
> "Based on my $6000 income, exactly how much is my 20% savings target?"

**🤖 AI Agent:**
> Using the analyze_budget tool: The mathematical 50/30/20 algorithm confirms your target for the 'saving' category is exactly $1200.00.


## ❓ FAQ

**Q: Does the engine automatically guess the category of an expense?**
No. The AI agent calling the tool is responsible for tagging each expense as 'need', 'want', or 'saving'. The MCP acts as an infallible mathematical referee, receiving the categorized list and computing the exact metrics and deviations.

**Q: Why use an MCP instead of having the LLM do the math?**
Because LLMs hallucinate math. If you give an AI 45 different expenses to sum up, it will almost certainly miscalculate the total or botch the exact percentage deviation. The V8 engine calculates numbers deterministically with 100% precision.

**Q: What happens if I spend more than my income?**
The engine perfectly calculates a negative surplus (deficit) and strictly alters the 'healthStatus' to 'Deficit', triggering a warning recommendation that instructs your agent to look at the deviations to cut costs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deterministic-503020-budget-engine](https://vinkius.com/mcp/deterministic-503020-budget-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deterministic 50/30/20 Budget Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deterministic-503020-budget-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deterministic 50/30/20 Budget Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deterministic-503020-budget-engine": {
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
