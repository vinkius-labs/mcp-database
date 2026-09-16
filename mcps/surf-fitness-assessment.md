# Surf Fitness Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-fitness-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Evaluate surf-specific physical readiness using discipline-based metrics.

## Description
This MCP server provides a specialized assessment engine for surfers. It analyzes paddle endurance, pop-up speed, and flexibility to calculate a fitness score tailored to specific disciplines like longboard, shortboard, or big wave. Use `analyze_fitness_profile` to get a complete readiness report, `compare_to_discipline_norms` to see how you stack up against professional standards, and `get_training_recommendations` for targeted exercise advice.


## Available Tools (4)
- **analyze_fitness_profile**: Calculates a comprehensive assessment based on raw physical metrics and the selected surf discipline
- **compare_to_discipline_norms**: Determines how a user's specific metrics stack up against professional standards for their discipline
- **get_training_recommendations**: Provides specific training focus areas based on identified weaknesses
- **validate_metric_integrity**: Checks if a set of metrics is physically plausible and logically consistent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Fitness Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze my fitness for shortboarding. I have 15 minutes of paddle endurance, a 1.5 second pop-up, and a flexibility score of 85."

**🤖 AI Agent:**
> Your overall fitness score for shortboarding is 92. Your primary strength is pop-up speed, and your training priorities should focus on increasing paddle endurance.

---

**👤 You:**
> "How do my metrics compare to professional big wave standards? Endurance: 45 mins, Pop-up: 2.5s, Flexibility: 70."

**🤖 AI Agent:**
> Your endurance rating is Elite, your speed rating is Average, and your flexibility rating is Average. Your readiness status is High for big wave surfing.

---

**👤 You:**
> "I need training recommendations for flexibility in longboarding."

**🤖 AI Agent:**
> To improve flexibility for longboarding, focus on postural stability and hip mobility through controlled yoga flows and dynamic stretching.


## ❓ FAQ

**Q: How do I calculate my overall fitness score?**
You can use the `analyze_fitness_profile` tool by providing your paddle endurance, pop-up speed, and flexibility score along with your surfing discipline.

**Q: Can I get specific exercises for my weaknesses?**
Yes, the `get_training_recommendations` tool provides actionable training advice based on your identified weaknesses and chosen discipline.

**Q: How does the assessment handle different surfing styles?**
The engine uses discipline-specific benchmarks. For example, `compare_to_discipline_norms` adjusts its evaluation based on whether you select longboard, shortboard, or big wave.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-fitness-assessment](https://vinkius.com/en/ai-agent-connect/surf-fitness-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Fitness Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-fitness-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Fitness Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-fitness-assessment": {
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
