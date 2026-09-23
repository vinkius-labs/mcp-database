# Burnout Risk Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/burnout-risk-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantifies occupational burnout risk using Maslach Burnout Inventory principles.

## Description
This MCP server provides tools to assess burnout risk by mapping work environmental factors to psychological burnout domains. It uses the Maslach Burnout Inventory methodology to evaluate how workload, autonomy, recognition, and recovery time impact emotional exhaustion, depersonalization, and personal accomplishment. Use `calculate_burnout_risk` for a full assessment, `analyze_recovery_efficiency` to check rest adequacy, or `identify_mbi_domain_alignment` to map stressors to specific psychological domains.


## Available Tools (4)
- **analyze_recovery_efficiency**: Evaluates if the amount of recovery time is sufficient given the workload and hours worked
- **get_risk_thresholds**: Informs the user of the specific score ranges used to categorize risk levels
- **identify_mbi_domain_alignment**: Maps specific occupational stressors to the three Maslach Burnout Inventory domains
- **calculate_burnout_risk**: Provides a comprehensive assessment of an individual's burnout risk based on their current work environment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Burnout Risk Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my burnout risk. I work 50 hours a week, have an autonomy level of 3, recognition level of 4, workload intensity of 8, and 10 hours of recovery."

**🤖 AI Agent:**
> Your burnout risk score is 8.5, which is categorized as Critical. The primary risk factors are high workload and low autonomy.

---

**👤 You:**
> "Is my recovery time sufficient? I work 40 hours, have 15 hours of recovery, and a workload intensity of 5."

**🤖 AI Agent:**
> Your recovery status is Sufficient. Your recovery ratio is well-balanced for your current workload intensity.

---

**👤 You:**
> "How do my stressors map to burnout domains? Autonomy is 2, recognition is 5, and workload is 9."

**🤖 AI Agent:**
> Your profile shows high risk for Emotional Exhaustion due to low autonomy and high workload, and risk for Reduced Personal Accomplishment due to low recognition.


## ❓ FAQ

**Q: How is the burnout risk calculated?**
The risk is determined by evaluating the imbalance between stressors like workload and low autonomy against protective factors like recovery time.

**Q: What are the Maslach Burnout Inventory domains?**
The tool maps stressors to Emotional Exhaustion, Depersonalization, and Reduced Personal Accomplishment.

**Q: Can I check if my rest time is enough?**
Yes, you can use `analyze_recovery_efficiency` to evaluate if your recovery hours are sufficient relative to your workload intensity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/burnout-risk-assessment](https://vinkius.com/en/ai-agent-connect/burnout-risk-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Burnout Risk Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `burnout-risk-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Burnout Risk Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "burnout-risk-assessment": {
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
