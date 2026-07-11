# Job Posting Inclusivity Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/job-posting-inclusivity-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [recruitment](../categories/recruitment.md)

Scan job descriptions for gendered language, unrealistic requirements, and technical jargon.

## Description
The Job Posting Inclusivity Analyzer helps recruiters and hiring managers identify hidden linguistic barriers in job advertisements. By using tools like `analyze_gender_bias`, `analyze_demand_stringency`, and `analyze_text_accessibility`, it evaluates text for masculine or feminine coded language, identifies high-intensity requirement language, and assesses technical jargon density to promote more inclusive hiring practices.


## Available Tools (3)
- **analyze_demand_stringency**: Measures the intensity of candidate requirements and use of hyperbole
- **analyze_gender_bias**: Evaluates the posting for masculine or feminine language influence
- **analyze_text_accessibility**: Determines if the posting is readable for a general audience


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Job Posting Inclusivity Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this job posting for gender bias: 'We are looking for a dominant and competitive software engineer to lead our team.'"

**🤖 AI Agent:**
> The analysis shows a masculine-coded lean with a net bias score indicating higher frequency of masculine terms.

---

**👤 You:**
> "Check this posting for unrealistic demands: 'Must be a coding ninja with 20+ years of experience in every single framework.'"

**🤖 AI Agent:**
> The tool detected extreme demand stringency, specifically identifying the hyperbolic persona 'ninja' and an unrealistic experience threshold.

---

**👤 You:**
> "Is this job description accessible? 'The candidate must understand Kubernetes, Docker, and CI/CD pipelines within a highly complex ecosystem.'"

**🤖 AI Agent:**
> The analysis identified several acronyms (Kubernetes, Docker, CI/CD) and a technical jargon density that may impact readability for general audiences.


## ❓ FAQ

**Q: How does the analyzer detect gender bias?**
The `analyze_gender_bias` tool compares your text against masculine-coded and feminine-coded word lexicons to calculate a net bias score.

**Q: Can it identify unrealistic job requirements?**
Yes, the `analyze_demand_stringency` tool identifies hyperbolic personae like 'ninja' or 'rockstar' and extreme experience thresholds.

**Q: Does it check for technical jargon?**
Yes, `analyze_text_accessibility` measures jargon density and detects acronyms that might act as barriers to qualified candidates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/job-posting-inclusivity-analyzer](https://vinkius.com/mcp/job-posting-inclusivity-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Job Posting Inclusivity Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `job-posting-inclusivity-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Job Posting Inclusivity Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "job-posting-inclusivity-analyzer": {
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
