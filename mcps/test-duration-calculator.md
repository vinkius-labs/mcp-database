# Test Duration Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/test-duration-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [statistics](../categories/statistics.md)

Calculate required A/B test duration, sample sizes, and experiment risk levels.

## Description
The Test Duration Calculator is a specialized tool for researchers to determine the necessary length of A/B experiments. By using `calculate_sample_size`, you can find the required number of users per variant based on your baseline conversion rate and MDE. The `estimate_timeline` tool then converts these sample requirements into days and recommended full weeks to account for seasonality. Finally, use `get_finalization_details` to project end dates and identify potential risks from long-running experiments.


## Available Tools (3)
- **calculate_sample_size**: Calculate required sample size for an experiment
- **estimate_timeline**: Estimate experiment duration
- **get_finalization_details**: Get experiment end date and risk assessment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Test Duration Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a baseline conversion rate of 5%, an MDE of 10%, and 3 variants. How many samples do I need?"

**🤖 AI Agent:**
> To detect a 10% relative lift with a 5% baseline across 3 variants, you will need approximately 48,250 samples per variant, totaling 144,750 users.

---

**👤 You:**
> "If I need 50,000 samples per variant and get 2,000 users per day, how many weeks should the test run?"

**🤖 AI Agent:**
> At 2,000 users per day, you need 25 days. To ensure full weekly cycles and avoid seasonality bias, the recommended duration is 4 weeks.

---

**👤 You:**
> "If my experiment starts on 2024-06-01 and lasts for 5 weeks, when will it end and is there any risk?"

**🤖 AI Agent:**
> The experiment is projected to end on 2024-07-06. Since the duration exceeds 4 weeks, a high alert level is triggered due to potential external interference.


## ❓ FAQ

**Q: How does the tool handle day-of-week bias?**
The tool uses `estimate_timeline` to round up the required duration to the nearest full 7-day cycle, ensuring that weekly seasonality does not bias your results.

**Q: What is considered a high-risk experiment duration?**
Any experiment projected to run longer than 4 weeks is flagged as high risk by `get_finalization_details` due to potential external noise like holidays or marketing changes.

**Q: Can I calculate sample size for multiple variants?**
Yes, by providing the total number of experimental groups to `calculate_sample_size`, the tool will determine the cumulative required samples.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/test-duration-calculator](https://vinkius.com/mcp/test-duration-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Test Duration Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `test-duration-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Test Duration Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "test-duration-calculator": {
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
