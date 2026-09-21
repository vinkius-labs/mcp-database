# Flexibility Assessment Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/flexibility-assessment-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Evaluates physical flexibility by comparing range-of-motion measurements against normative data.

## Description
This MCP server provides a specialized engine for analyzing physical mobility. It uses tools like `calculate_flexibility_score` to generate composite profiles, `get_normative_reference` to benchmark against age and gender-specific data, `detect_imbalances` to identify lateral asymmetries, and `identify_training_priorities` to pinpoint areas for improvement. It is designed to help identify injury risks and guide training focus through precise range-of-motion analysis.


## Available Tools (4)
- **calculate_flexibility_score**: Calculates the overall flexibility profile for a user based on multiple movement tests
- **detect_imbalances**: Specifically isolates and describes the severity of lateral asymmetries
- **get_normative_reference**: Retrieves the expected range or threshold for a specific flexibility metric
- **identify_training_priorities**: Generates a list of focus areas based on deficit analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flexibility Assessment Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my flexibility profile with a sit-and-reach of 25cm, shoulder flexibility of 30cm, and hip rotation of 45 degrees on both sides."

**🤖 AI Agent:**
> Your flexibility score is 75, placing you in the 65th percentile for your demographic.

---

**👤 You:**
> "Check for imbalances if my left hip rotation is 30 degrees and my right hip rotation is 50 degrees."

**🤖 AI Agent:**
> A significant asymmetry was detected between the left and right hip rotation.

---

**👤 You:**
> "What are my training priorities based on a low sit-and-reach score and a detected hip asymmetry?"

**🤖 AI Agent:**
> Your priority areas are hamstring flexibility and hip mobility, with a high level of urgency due to the detected asymmetry.


## ❓ FAQ

**Q: How does the scoring work?**
The engine compares your measurements, such as sit-and-reach or hip rotation, against standardized normative data to calculate a score and percentile.

**Q: Can it detect muscle imbalances?**
Yes, by using `detect_imbalances`, the server identifies significant discrepancies between left and right side measurements.

**Q: What measurements are required?**
You can provide sit-and-reach distance, shoulder flexibility, and hip rotation for both left and right sides.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/flexibility-assessment-scorer](https://vinkius.com/en/ai-agent-connect/flexibility-assessment-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flexibility Assessment Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flexibility-assessment-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flexibility Assessment Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flexibility-assessment-scorer": {
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
