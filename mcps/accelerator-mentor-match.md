# Accelerator Mentor Match MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-mentor-match)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business](../categories/business.md)

Evaluates mentor-startup matching effectiveness using expertise, capacity, and stage alignment.

## Description
This MCP server provides a specialized matching engine for accelerator programs. It analyzes how effectively mentors are paired with startups by evaluating expertise alignment, stage compatibility, and capacity constraints. Use `analyze_match_coverage` to see if the mentor pool meets cohort needs, `calculate_utilization_rate` to monitor mentor workload, and `evaluate_match_quality` to get granular scores on specific pairings.


## Available Tools (3)
- **calculate_utilization_rate**: Measures the efficiency of mentor hour allocation to ensure workload balance
- **evaluate_match_quality**: Provides a granular assessment of how good the specific pairings are based on expertise and stage
- **analyze_match_coverage**: Determines how effectively the available mentors cover the total skill requirements of the startup cohort


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Mentor Match** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How well does our current mentor pool cover the skills needed by our startups?"

**🤖 AI Agent:**
> The current match coverage is 85%, with 12 total needs met and 2 unaddressed needs in specialized technical areas.

---

**👤 You:**
> "Are our mentors being utilized efficiently?"

**🤖 AI Agent:**
> The current mentor utilization rate is 72%, with 144 hours used out of 200 total available hours.

---

**👤 You:**
> "What is the quality of the pairing between Mentor A and Startup B?"

**🤖 AI Agent:**
> The match quality score for this pairing is 0.92, indicating a very strong alignment in both expertise and development stage.


## ❓ FAQ

**Q: How is match coverage calculated?**
The `analyze_match_coverage` tool calculates coverage by comparing the unique skill requirements of all startups against the skills provided by assigned mentors.

**Q: Can I check if a mentor is over-leveraged?**
Yes, use the `calculate_utilization_rate` tool to measure mentor hour allocation and ensure workload balance across the cohort.

**Q: What factors influence the match quality score?**
The `evaluate_match_quality` tool determines the score based on the intersection of mentor expertise with startup needs and the alignment of the mentor's experience with the startup's current stage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-mentor-match](https://vinkius.com/ai-agent-connect/accelerator-mentor-match)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Mentor Match** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-mentor-match` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Mentor Match** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-mentor-match": {
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
