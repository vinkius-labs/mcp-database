# HDB BTO Ballot Probability Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/hdb-bto-ballot-probability-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate your relative chances of securing an HDB BTO flat based on applicant type, project maturity, and ethnic quotas.

## Description
This MCP server provides deterministic tools to evaluate the likelihood of a successful HDB Build-To-Order (BTO) application. By analyzing the intersection of applicant status and estate characteristics, users can determine their relative standing in the ballot pool. Use `calculate_priority_weight` to establish a baseline score, `apply_ethnic_adjustment` to account for ethnic quota constraints, and `evaluate_ballot_chance` to derive the final relative probability and success category.


## Available Tools (3)
- **apply_ethnic_adjustment**: Calculates the penalty factor applied to the priority weight based on the current ethnic quota status
- **calculate_priority_weight**: Determines the base priority weight of an applicant based on their type and the project's maturity
- **evaluate_ballot_chance**: Computes the final relative ballot chance and assigns a qualitative success category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HDB BTO Ballot Probability Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are my chances if I am a First-timer applying for a Non-mature project that is within its ethnic quota?"

**🤖 AI Agent:**
> Your priority weight is 2.0, the adjustment factor is 1.0, and your relative ballot chance is 2.0, which falls into the High success category.

---

**👤 You:**
> "I am a Second-timer looking at a Mature estate that has reached its ethnic quota. What is my relative chance?"

**🤖 AI Agent:**
> Your priority weight is 1.0, the adjustment factor is significantly reduced due to the quota limit, resulting in a Low success category.

---

**👤 You:**
> "Calculate the chance for a First-timer in a Mature project with no ethnic quota issues."

**🤖 AI Agent:**
> Your priority weight is 3.0, the adjustment factor is 1.0, and your relative ballot chance is 3.0, which is a High success category.


## ❓ FAQ

**Q: How is my priority weight determined?**
The `calculate_priority_weight` tool determines your weight based on whether you are a First-timer or Second-timer and if the project is in a Mature or Non-mature estate.

**Q: What does the ethnic adjustment factor do?**
The `apply_ethnic_adjustment` tool calculates a multiplier that reduces your priority weight if the estate's ethnic quota is near its limit or already at the limit.

**Q: How do I know if my chances are high or low?**
After using `evaluate_ballot_chance`, you will receive a success category of High, Medium, or Low based on your relative ballot chance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/hdb-bto-ballot-probability-calculator](https://vinkius.com/ai-agent-connect/hdb-bto-ballot-probability-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HDB BTO Ballot Probability Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hdb-bto-ballot-probability-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HDB BTO Ballot Probability Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hdb-bto-ballot-probability-calculator": {
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
