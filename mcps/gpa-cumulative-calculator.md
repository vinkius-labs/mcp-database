# GPA Cumulative Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gpa-cumulative-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Calculate and track semester and cumulative GPA using various grading scales.

## Description
This MCP server allows for precise academic performance tracking. Use `calculate_semester_performance` to compute term GPAs and `update_cumulative_record` to maintain a running total across your entire academic history. It supports 4.0, 4.3, 5.0, and 100-point scales.


## Available Tools (4)
- **calculate_semester_performance**: Compute performance metrics for a single academic term
- **get_grade_weight**: s. "A", "B+") and a grading scale (standard_4.0, advanced_4.3, weighted_5.0, or percentage_100) and returns its weight.

Determine the numeric value of a grade based on a scale
- **update_cumulative_record**: Update the cumulative academic record
- **validate_academic_input**: Validate and sanitize course input


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GPA Cumulative Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my GPA for this semester if I got an A in Math (3 credits) and a B in English (2 credits) on a 4.0 scale?"

**🤖 AI Agent:**
> Your semester GPA is 3.6.

---

**👤 You:**
> "Calculate the weight for an A+ on a 4.3 scale."

**🤖 AI Agent:**
> The numeric weight for an A+ on the 4.3 scale is 4.3.

---

**👤 You:**
> "How many total credits did I earn if I had 15 previous credits and just finished a semester with 18 credits?"

**🤖 AI Agent:**
> You have earned a total of 33 credits.


## ❓ FAQ

**Q: How do I calculate my semester GPA?**
Use the `calculate_semester_performance` tool by providing your course list and grading scale.

**Q: Does it support weighted grades?**
Yes, using the 5.0 scale allows you to include weights for AP or Honors courses.

**Q: Can I track multiple semesters?**
Yes, use `update_cumulative_record` to add new semester data to your existing totals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gpa-cumulative-calculator](https://vinkius.com/mcp/gpa-cumulative-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GPA Cumulative Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gpa-cumulative-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GPA Cumulative Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gpa-cumulative-calculator": {
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
