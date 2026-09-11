# Exploration Success Probability Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/exploration-success-probability-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Assess geological exploration risk and discovery likelihood.

## Description
This MCP server provides specialized computational tools for assessing the risk and likelihood of resource discovery within geological exploration programs. It accounts for spatial and geological correlations between multiple prospects to provide accurate risk assessments. Use `calculate_discovery_probability` to determine the cumulative likelihood of finding at least one resource, or `calculate_risked_resource` to estimate the mathematical value of a potential find based on success probability.


## Available Tools (4)
- **calculate_discovery_probability**: Determine the cumulative likelihood of finding at least one resource in the exploration portfolio
- **calculate_expected_value**: Quantify the average number of successful discoveries expected from the current portfolio
- **calculate_risked_resource**: Estimate the risked volume of a resource by applying probability to the total potential volume
- **analyze_correlation_sensitivity**: Understand how sensitive the discovery probability is to changes in the geological correlation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Exploration Success Probability Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the probability of finding at least one resource if I have 5 prospects, each with a 20% success chance, and a correlation of 0.3?"

**🤖 AI Agent:**
> The probability of at least one discovery is 64.2%.

---

**👤 You:**
> "Calculate the risked volume for a prospect with a 15% success probability and a total potential volume of 500 million cubic meters across 3 prospects."

**🤖 AI Agent:**
> The risked volume is 225 million cubic meters.

---

**👤 You:**
> "How many successful discoveries should I expect from 10 prospects with a 25% individual success probability?"

**🤖 AI Agent:**
> You can expect 2.5 successful discoveries.


## ❓ FAQ

**Q: How does geological correlation affect my results?**
High correlation means successes are likely to cluster. The `calculate_discovery_probability` tool adjusts the cumulative probability downward as correlation increases, reflecting that successes are not independent events.

**Q: What is a risked resource estimate?**
A risked resource estimate is a volume-based metric where the theoretical total resource is adjusted by the probability of success. You can calculate this using `calculate_risked_resource`.

**Q: Can I analyze how sensitive my model is to correlation assumptions?**
Yes, you can use the `analyze_correlation_sensitivity` tool to see how the probability of at least one success shifts when the correlation coefficient is adjusted.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/exploration-success-probability-engine](https://vinkius.com/en/ai-agent-connect/exploration-success-probability-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Exploration Success Probability Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `exploration-success-probability-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Exploration Success Probability Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "exploration-success-probability-engine": {
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
