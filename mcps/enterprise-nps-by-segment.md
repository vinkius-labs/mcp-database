# Enterprise NPS by Segment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-nps-by-segment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Analyze Net Promoter Score (NPS) across enterprise customer segments to identify performance gaps.

## Description
This MCP server provides advanced analytics for Net Promoter Score (NPS) within enterprise customer segments. It allows AI agents to calculate specific NPS metrics using `calculate_segment_nps`, compare performance across different segments with `compare_segments`, and identify critical areas for action via `identify_improvement_priorities`. Additionally, `get_segment_health_summary` provides a qualitative health check and reliability score based on response rates. It is designed to help management pinpoint which segments require immediate attention based on dissatisfaction levels and segment size.


## Available Tools (4)
- **calculate_segment_nps**: Calculates the primary NPS metric for a specific enterprise segment
- **compare_segments**: Analyzes the performance gap between two or more enterprise segments
- **get_segment_health_summary**: Provides a high-level health check combining NPS reliability and customer sentiment
- **identify_improvement_priorities**: Suggests which segments management should focus on based on dissatisfaction levels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise NPS by Segment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the NPS for the Finance segment?"

**🤖 AI Agent:**
> The NPS for the Finance segment is 45, with 60% Promoters, 25% Passives, and 15% Detractors.

---

**👤 You:**
> "Which segments should we prioritize for improvement?"

**🤖 AI Agent:**
> The Mid-Market segment is a high priority due to an NPS of 12 and a high volume of Detractors.

---

**👤 You:**
> "How healthy is the Healthcare segment?"

**🤖 AI Agent:**
> The Healthcare segment is currently rated as Healthy with a high reliability score.


## ❓ FAQ

**Q: How is the NPS score calculated?**
The NPS score is calculated by subtracting the percentage of Detractors from the percentage of Promoters.

**Q: What does the reliability score represent?**
The reliability score is a function of the response rate; a low response rate results in a lower reliability score, indicating the NPS may not be statistically representative.

**Q: Can I compare multiple segments at once?**
Yes, you can use the `compare_segments` tool to analyze the performance gap between two or more enterprise segments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-nps-by-segment](https://vinkius.com/ai-agent-connect/enterprise-nps-by-segment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise NPS by Segment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-nps-by-segment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise NPS by Segment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-nps-by-segment": {
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
