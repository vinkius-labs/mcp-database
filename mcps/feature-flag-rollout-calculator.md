# Feature Flag Rollout Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/feature-flag-rollout-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Calculate deterministic user assignment, rollout projections, and statistical sample sizes for feature flags.

## Description
This MCP server provides mathematical utilities for managing gradual feature rollouts. Use `get_user_assignment` to verify if a specific user falls within a rollout percentage using consistent hashing. Plan your deployment with `project_rollout_impact` to see how many users are added at each stage. Ensure experiment validity with `calculate_statistical_thresholds` to determine the required sample size for detecting regressions, and use `analyze_cohort_overlap` to estimate the intersection of multiple concurrent flags.


## Available Tools (4)
- **analyze_cohort_overlap**: Estimates the potential intersection of two different feature flag populations
- **calculate_statistical_thresholds**: Determines the required number of users needed in a treatment group to detect a metric regression
- **get_user_assignment**: Determines whether a specific user is included in a feature flag's current rollout percentage
- **project_rollout_impact**: Predicts the number of users affected at each stage of a predefined deployment schedule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Feature Flag Rollout Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is user 'user_123' enabled for feature 'new_ui' at a 25% rollout?"

**🤖 AI Agent:**
> The user 'user_12<0xA0>3' is currently enabled for the 'new_ui' feature.

---

**👤 You:**
> "What is the minimum and maximum overlap if Flag A is at 30% and Flag B is at 45%?"

**🤖 AI Agent:**
> The potential overlap between the two flags ranges from a minimum of 0% to a maximum of 30%.

---

**👤 You:**
> "How many users do I need for an experiment with a 5% baseline conversion, 1% MDE, and 95% confidence?"

**🤖 AI Agent:**
> To detect a 1% absolute drop from a 5% baseline with 95% confidence, you require a treatment sample size of approximately 16,450 users.


## ❓ FAQ

**Q: How does the user assignment work?**
The `get_user_assignment` tool uses consistent hashing of the User ID and Feature Key to ensure that a user's assignment remains deterministic at any given rollout percentage.

**Q: Can I use this for A/B testing?**
Yes. You can use `calculate_statistical_thresholds` to determine the necessary sample size to detect a specific Minimum Detectable Effect (MDE) with your desired confidence level.

**Q: How do I estimate the impact of a multi-stage rollout?**
Use `project_rollout_impact` by providing your total population size and a schedule of percentages to see both active and incremental user counts at each stage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/feature-flag-rollout-calculator](https://vinkius.com/mcp/feature-flag-rollout-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Feature Flag Rollout Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `feature-flag-rollout-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Feature Flag Rollout Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "feature-flag-rollout-calculator": {
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
