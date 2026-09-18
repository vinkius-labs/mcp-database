# Insomnia Severity Index (ISI) Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/insomnia-severity-index-isi-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Clinical assessment tool to calculate Insomnia Severity Index scores and sleep profiles.

## Description
This MCP server provides clinical-grade tools to assess insomnia using the validated Insomnia Severity Index (ISI). It allows AI agents to calculate total severity scores, perform subdomain analysis (distinguishing between sleep onset and maintenance issues), provide clinical guidance, and evaluate sleep quality profiles. By using `get_isi_score`, agents can categorize insomnia severity, while `get_subdomain_analysis` helps identify specific sleep disruption patterns.


## Available Tools (4)
- **get_clinical_guidance**: 
- **get_isi_score**: 
- **get_sleep_quality_profile**: 
- **get_subdomain_analysis**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Insomnia Severity Index (ISI) Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my ISI score with these responses: [2, 3, 1, 0, 2, 1, 2]"

**🤖 AI Agent:**
> Your total Insomnia Severity Index score is 11, which falls into the moderate insomnia category.

---

**👤 You:**
> "Analyze my sleep profile using these responses: [1, 1, 0, 0, 1, 1, 1]"

**🤖 AI Agent:**
> Your sleep profile shows minimal interference with daily life and a high perceived quality of sleep.

---

**👤 You:**
> "What clinical guidance is recommended for a total ISI score of 25?"

**🤖 AI Agent:**
> For a score of 25, immediate professional medical intervention is recommended due to severe insomnia symptoms.


## ❓ FAQ

**Q: How do I use the ISI tools?**
Provide the 7 integer responses from the ISI questionnaire (ranging from 0 to 4) to tools like `get_isi_score` or `get_subdomain_analysis` to receive your assessment.

**Q: What is the difference between onset and maintenance analysis?**
The `get_subdomain_analysis` tool breaks down responses to show if your primary issue is difficulty falling asleep (onset) or staying asleep (maintenance).

**Q: Can this tool provide medical advice?**
The tool provides clinical guidance based on validated scoring, but it is not a substitute for professional medical diagnosis or treatment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/insomnia-severity-index-isi-analyzer](https://vinkius.com/en/ai-agent-connect/insomnia-severity-index-isi-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Insomnia Severity Index (ISI) Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `insomnia-severity-index-isi-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Insomnia Severity Index (ISI) Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "insomnia-severity-index-isi-analyzer": {
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
