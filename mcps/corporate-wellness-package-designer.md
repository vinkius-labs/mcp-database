# Corporate Wellness Package Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/corporate-wellness-package-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Design structured corporate wellness programs based on company size, budget, and goals.

## Description
This MCP server provides a specialized toolkit for HR professionals and business leaders to design impactful wellness programs. By using `calculate_package_composition`, you can determine the ideal mix of services for your specific budget and headcount. You can also use `project_outcomes` to estimate improvements in employee engagement and absenteeism, or `analyze_demographic_fit` to ensure your selected services align with your workforce's age and type profile. Finally, `generate_frequency_schedule` creates a monthly calendar to ensure consistent delivery of wellness activities throughout the year.


## Available Tools (4)
- **project_outcomes**: Estimates the qualitative and quantitative benefits of a specific wellness package
- **analyze_demographic_fit**: Evaluates if a proposed package aligns with the specific needs of the employee demographic
- **calculate_package_composition**: Determines the specific wellness services that fit within a company's budget and goals
- **generate_frequency_schedule**: Creates a structured timeline for when services should be delivered


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Corporate Wellness Package Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Design a wellness package for a company of 50 employees with a $10,000 budget focused on reducing burnout."

**🤖 AI Agent:**
> The package includes mental health counseling sessions, stress management workshops, and weekly mindfulness exercises, with a per-employee cost of $200.

---

**👤 You:**
> "What are the expected outcomes for a wellness program with these services: [{"name": "Gym Membership", "category": "PHYSICAL"}] for 100 employees?"

**🤖 AI Agent:**
> The program is projected to increase employee engagement by 15% and reduce absenteeism by 5%.

---

**👤 You:**
> "Create a monthly schedule for a wellness package containing fitness classes and nutrition workshops with a $5,000 budget."

**🤖 AI Agent:**
> The schedule includes bi-weekly fitness classes in January, March, May, July, September, and November, and monthly nutrition workshops throughout the year.


## ❓ FAQ

**Q: How do I determine which wellness services to include?**
You can use the `calculate_package_composition` tool. Provide your company size, total budget, and primary goal to receive a tailored list of services and per-employee costs.

**Q: Can I see the expected impact of my wellness program?**
Yes, the `project_outcomes` tool allows you to estimate improvements in employee engagement, absenteeism reduction, and retention based on your package details.

**Q: How can I ensure the program fits my specific employees?**
Use the `analyze_demographic_fit` tool to evaluate how well your proposed services match the age groups and types within your company.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/corporate-wellness-package-designer](https://vinkius.com/en/ai-agent-connect/corporate-wellness-package-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Corporate Wellness Package Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `corporate-wellness-package-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Corporate Wellness Package Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "corporate-wellness-package-designer": {
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
