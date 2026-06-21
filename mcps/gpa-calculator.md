# GPA Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gpa-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Calculate weighted GPA for US (4.0) and Brazilian (10.0) scales, including honors classification.

## Description
The GPA Calculator MCP provides a specialized engine for determining weighted Grade Point Averaged across different academic grading systems. It allows users to calculate the single-period weighted average using `compute_weighted_gpa`, evaluate performance trends between semesters with `compare_semesters`, and normalize grades between scales via `convert_grade_scale`. Perfect for students and educators managing US 4.0 and Brazilian 10.0 academic records.


## Available Tools
- **compare_semesters**: Evaluates the performance trend between two different academic periods
- **compute_weighted_gpa**: Returns weighted GPA, honors status, and total credits.

Calculates the single-period weighted average and determines if the student qualifies for academic honors
- **convert_grade_scale**: A utility to normalize a grade from one academic system to another


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GPA Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my GPA for this semester: Math (Grade 4.0, 3 credits) and History (Grade 3.0, 2 credits) on the US scale."

**🤖 AI Agent:**
> Your weighted GPA is 3.6, which qualifies you for Cum Laude honors.

---

**👤 You:**
> "Compare my performance: Current semester (Grade 8.0, 4 credits) vs Previous semester (Grade 7.0, 4 credits) on the BR scale."

**🤖 AI Agent:**
> Your GPA increased by 1.0, showing an Improved performance trend.

---

**👤 You:**
> "Convert a grade of 8.5 from the Brazilian scale to the US scale."

**🤖 AI Agent:**
> A grade of 8.5 on the Brazilian scale is equivalent to 3.4 on the US scale.


## ❓ FAQ

**Q: How does the weighted GPA calculation work?**
The tool multiplies each subject's grade by its credit value, sums these products, and then divides the total by the sum of all credits. You can use `compute_weighted_gpa` to perform this calculation.

**Q: Can I convert grades from the Brazilian scale to the US scale?**
Yes, you can use the `convert_grade_scale` tool to normalize grades from the 10.0 Brazilian scale to the 4.0 US scale using linear scaling.

**Q: How are academic honors determined?**
Honors like Summa Cum Laude, Magna Cum Laude, and Cum Laude are determined based on the US 4.0 scale thresholds (3.9+, 3.7+, and 3.5+ respectively) when using `compute_weighted_gpa`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gpa-calculator](https://vinkius.com/mcp/gpa-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GPA Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gpa-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GPA Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gpa-calculator": {
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
