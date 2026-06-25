# Recovery Readiness Score MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/recovery-readiness-score)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Evaluate training readiness and optimal intensity based on sleep, soreness, stress, and motivation.

## Description
The Recovery Readiness Score engine provides a data-driven approach to training optimization. By synthesizing physiological markers like sleep duration and DOMS (Delayed Onset Muscle Soreness) with psychological indicators such as stress and motivation, the system calculates a comprehensive readiness score. Use `calculate_readiness_score` to determine your recommended training intensity--ranging from Heavy to Active Rest--and estimate when you will be fully recovered. You can also use `get_soreness_impact_analysis` to identify which specific muscle groups are currently limiting your performance, or `validate_recovery_metrics` to ensure your input data is within valid physiological bounds.


## Available Tools (3)
- **calculate_readiness_score**: Calculate training readiness score and intensity
- **get_soreness_impact_analysis**: Analyze muscle group soreness impact
- **validate_recovery_metrics**: Validate recovery metrics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recovery Readiness Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I slept 7 hours with good quality, but my legs and chest are very sore (8/10). My stress is low (2) and motivation is high (9). I had a heavy session 2 days ago. How should I train today?"

**🤖 AI Agent:**
> Based on your metrics, your recovery score is approximately 65. Due to high soreness in your legs and chest and the recent heavy session, your recommended training intensity for today is 'Light'.

---

**👤 You:**
> "Check if my recovery metrics are valid: sleep 8 hours, quality 9, stress 5, motivation 7."

**🤖 AI Agent:**
> Yes, all provided metrics are within the valid physiological and psychological ranges.

---

**👤 You:**
> "Analyze this soreness: {'Legs': 9, 'Back': 2, 'Chest': 1}."

**🤖 AI Agent:**
> The critical muscle group identified is Legs. The high soreness level suggests localized fatigue that may limit your training intensity.


## ❓ FAQ

**Q: How is my training intensity determined?**
The intensity is determined by analyzing your sleep quality, muscle soreness (DOMS), stress levels, and motivation. If high soreness or recent heavy sessions are detected via `calculate_readiness_score`, the system may recommend a lighter session like 'Light' or 'Active Rest'.

**Q: Can I check which muscle groups are preventing me from training hard?**
Yes, you can use the `get_soreness_impact_analysis` tool. By providing your current DOMS levels, it will identify 'critical groups' that are currently limiting your overall readiness score.

**Q: What should I do if my metrics are invalid?**
You can use `validate_recovery_metrics` to check your inputs. It will return a list of specific errors if any value (like stress or motivation) is outside the required 0-10 range.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/recovery-readiness-score](https://vinkius.com/mcp/recovery-readiness-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recovery Readiness Score** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recovery-readiness-score` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recovery Readiness Score** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recovery-readiness-score": {
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
