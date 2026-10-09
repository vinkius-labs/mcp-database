# School Grade Average Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/school-grade-average-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate weighted and unweighted academic averages with precision.

## Description
This MCP server provides a specialized calculation engine for academic performance. It allows AI agents to compute precise weighted and unweighted averages, verify weight distributions, and validate that grades fall within specific academic bounds. Use `calculate_average` to find the mean score, `verify_weight_distribution` to check weight totals, `validate_grade_bounds` to ensure scores are within range, and `get_grade_contribution` to analyze the impact of a specific assessment.


## Available Tools (4)
- **calculate_average**: Calculates the final average grade for a given set of assessments
- **get_grade_contribution**: Determines the individual impact of a single grade on the total weighted average
- **validate_grade_bounds**: Ensures all submitted grades fall within a valid academic range
- **verify_weight_distribution**: Checks if the provided weights follow a specific distribution or sum to a specific target


## 💬 Prompt Examples

Here are some examples of how you can interact with the **School Grade Average Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the average of grades 80, 90, and 70?"

**🤖 AI Agent:**
> The average grade is 80.

---

**👤 You:**
> "Calculate the weighted average for grades 90 and 80 with weights 0.7 and 0.3."

**🤖 AI Agent:**
> The weighted average is 87.0, with a total weight of 1.0.

---

**👤 You:**
> "Are the grades [95, 105, 85] valid for a range of 0 to 100?"

**🤖 AI Agent:**
> No, the grade 105 is out of bounds.


## ❓ FAQ

**Q: How do I calculate a weighted average?**
Provide the list of grades and a corresponding list of weights to the `calculate_average` tool.

**Q: Can I check if my grades are within a valid range?**
Yes, use the `validate_grade_bounds` tool to ensure all scores fall between your specified minimum and maximum values.

**Q: What happens if I don't provide weights?**
If no weights are provided, the `calculate_average` tool treats every grade as having an equal weight of one.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/school-grade-average-engine](https://vinkius.com/en/ai-agent-connect/school-grade-average-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **School Grade Average Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `school-grade-average-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **School Grade Average Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "school-grade-average-engine": {
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
