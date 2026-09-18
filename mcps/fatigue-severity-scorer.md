# Fatigue Severity Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fatigue-severity-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Analyzes Fatigue Severity Scale (FSS) responses to provide clinical scoring and impact assessments.

## Description
This MCP server provides clinical analysis of the Fatigue Severity Scale (FSS). It allows AI agents to process questionnaire responses to determine total fatigue scores, categorize severity, and evaluate functional impact on daily life. Using `calculate_fss_score`, agents can derive fatigue categories and clinical significance. The `assess_functional_impact` tool identifies affected functional domains, while `compare_to_norms` benchmarks results against healthy population data. Finally, `generate_clinical_recommendations` provides prioritized guidance based on the calculated severity and impact levels.


## Available Tools (4)
- **assess_functional_impact**: Evaluates how much the reported fatigue interferes with daily life activities
- **calculate_fss_score**: Calculates the primary numerical score and fatigue category based on raw questionnaire responses
- **compare_to_norms**: Compares the user's score against standard healthy population benchmarks
- **generate_clinical_recommendations**: Provides guidance for next steps based on the severity and impact of the fatigue


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fatigue Severity Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the fatigue score for these responses: [3, 2, 4, 3, 2, 1, 3]"

**🤖 AI Agent:**
> The total FSS score is 18, which indicates Severe Fatigue.

---

**👤 You:**
> "What is the functional impact for a user with these FSS ratings: [1, 0, 1, 1, 0, 1, 0]?"

**🤖 AI Agent:**
> The functional impact is Low, with minimal interference in daily activities.

---

**👤 You:**
> "Compare a total FSS score of 22 to the standard norms."

**🤖 AI Agent:**
> A score of 22 is significantly above average compared to the healthy population norm.


## ❓ FAQ

**Q: What is the Fatigue Severity Scale (FSS)?**
The FSS is a validated clinical tool used to measure how fatigue affects various functional domains in a person's daily life.

**Q: How do I provide the responses for scoring?**
You must provide an array of exactly seven integers, where each integer is a rating between 0 and 4, using the `calculate_fss_score` tool.

**Q: Can this tool provide medical advice?**
No. This tool provides clinical recommendations based on scoring logic. It is intended to support clinical workflows and should not replace professional medical consultation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fatigue-severity-scorer](https://vinkius.com/en/ai-agent-connect/fatigue-severity-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fatigue Severity Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fatigue-severity-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fatigue Severity Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fatigue-severity-scorer": {
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
