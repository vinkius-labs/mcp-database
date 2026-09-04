# European Subsidy Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/european-subsidy-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate potential EU regional subsidies, conditionality costs, and net economic benefits.

## Description
This MCP server provides tools to navigate the complexities of European Union regional subsidies. It allows users to determine maximum support through `calculate_potential_subsidy`, estimate the economic impact of compliance using `estimate_conditionality_costs`, and calculate the final economic gain with `calculate_net_benefit`. Additionally, it ensures regulatory safety by using `validate_state_aid_compliance` to check if proposed aid adheres to EU State Aid rules.


## Available Tools (4)
- **calculate_net_benefit**: Determines the final economic value of the subsidy after all obligations are considered
- **calculate_potential_subsidy**: Determines the maximum amount of subsidy a company can theoretically claim
- **validate_state_aid_compliance**: Checks if a proposed subsidy amount exceeds the legal limits set by EU State Aid rules
- **estimate_conditionality_costs**: Calculates the cost of meeting the requirements attached to a subsidy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **European Subsidy Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much subsidy can a tech company in Germany claim for a 1,000,000 Euro investment?"

**🤖 AI Agent:**
> Based on the investment and sector, the potential subsidy value is 250,000 Euros with a maximum aid intensity of 25%.

---

**👤 You:**
> "If my potential subsidy is 500,000 Euros and my conditionality costs are 50,000 Euros, what is my net benefit?"

**🤖 AI Agent:**
> The net benefit is 450,000 Euros, with a subsidy efficiency of 90%.

---

**👤 You:**
> "Is a 300,000 Euro subsidy compliant for a 1,000,000 Euro investment in the Manufacturing sector?"

**🤖 AI Agent:**
> No, the maximum allowed amount for this sector and investment is 200,000 Euros. The proposed amount exceeds the limit by 100,000 Euros.


## ❓ FAQ

**Q: How does the tool account for EU regulations?**
The `validate_state_aid_compliance` tool specifically checks proposed amounts against maximum aid intensity limits defined by EU State Aid rules for specific sectors.

**Q: What is included in the conditionality cost?**
Conditionality costs include the economic value of maintaining required headcount and any mandatory additional investments needed to remain compliant with the subsidy terms.

**Q: Can I calculate the actual profit from a subsidy?**
Yes, by using `calculate_net_benefit`, you can find the net economic gain after subtracting all conditionality costs from the potential subsidy value.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/european-subsidy-calculator](https://vinkius.com/ai-agent-connect/european-subsidy-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **European Subsidy Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `european-subsidy-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **European Subsidy Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "european-subsidy-calculator": {
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
