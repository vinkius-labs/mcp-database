# GPA Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gpa-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Convert academic grades between different scales and calculate weighted averages.

## Description
This MCP server provides specialized tools for academic grade conversion. Use `convert_grade` to transform a numerical grade from one scale (e.g., 4.0) to another (e.g., 10.0). You can also use `calculate_weighted_average` to compute your cumulative GPA by providing course grades and credits, or `get_grade_category` to determine if a specific score falls into high achievement, satisfactory, or unsatisfactory tiers.


## Available Tools
- **calculate_weighted_average**: Calculates the weighted average of grades based on course credits
- **convert_grade**: Converts a grade from one scale to another
- **get_grade_category**: Classifies a grade into performance tiers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GPA Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert a grade of 3.5 from a 4.0 scale to a 10.0 scale."

**🤖 AI Agent:**
> The `convert_grade` tool would return a converted value of 8.75, representing an 87.5% achievement level.

---

**👤 You:**
> "Calculate my weighted average for these courses: Grade 4.0 with 3 credits, and Grade 3.0 with 2 credits."

**🤖 AI Agent:**
> The `calculate_weighted_average` tool would return a final GPA of 3.6 and a total of 5 credits.

---

**👤 You:**
> "What category is an 8.0 on a 10.0 scale?"

**🤖 AI Agent:**
> The `get_grade_category` tool would identify this as part of the satisfactory performance tier.


## ❓ FAQ

**Q: How do I convert my GPA to a different scale?**
Use the `convert_grade` tool. You need to provide your current grade, the maximum value of your original scale, and the maximum value of the target scale.

**Q: Can I calculate my total GPA for a semester?**
Yes, use the `calculate_weighted_average` tool. Provide a JSON array of objects, where each object contains the grade and the number of credits for each course.

**Q: How does the tool determine my performance tier?**
The `get_grade_category` tool evaluates your grade against predefined percentage thresholds for the specified scale to identify if you are in the high, middle, or low achievement tier.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gpa-converter](https://vinkius.com/mcp/gpa-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GPA Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gpa-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GPA Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gpa-converter": {
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
