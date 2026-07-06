# ProUni Eligibility Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/prouni-eligibility-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Instantly calculate scholarship eligibility (Full or Partial) for ProUni by inputting family income, household size, and ENEM scores.

## Description
**Are you considering higher education but unsure about scholarship eligibility?** Many students face the challenge of matching their financial background and academic performance against complex, shifting institutional criteria. Trying to calculate eligibility manually using minimum wage multipliers and specific score cutoffs is time-consuming and prone to error.


## Available Tools (4)
- **identify_eligible_courses**: Public school students receive a score bonus. Lower scholarship tiers restrict available courses.

Identify eligible courses based on ENEM scores, public school status, and scholarship tier
- **calculate_per_capita_income**: Calculate per capita income from gross family income and number of members
- **query_university_locations**: Query universities participating in ProUni by city
- **determine_eligibility_tier**: Determine scholarship eligibility tier based on per capita income


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ProUni Eligibility Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My family's gross income is 60,000 and there are 4 members. I scored well in Science."

**🤖 AI Agent:**
> First, we calculate your per capita income using `calculate_per_capita_income`. Based on that result and your ENEM scores, I can then run the `identify_eligible_courses` tool to suggest majors you qualify for.

---

**👤 You:**
> "I want to know which universities are in São Paulo that offer ProUni programs."

**🤖 AI Agent:**
> I will use the `query_university_locations` tool with 'São Paulo' as the city. This provides a list of available universities and campuses for your planning.

---

**👤 You:**
> "My per capita income is 1800, and I attended a public school. What tier am I in?"

**🤖 AI Agent:**
> The `determine_eligibility_tier` tool will analyze your income against the 1.5x and 3x minimum wage thresholds to provide a definitive scholarship tier, which is crucial for all subsequent checks.


## ❓ FAQ

**Q: What is the first step to check my financial eligibility?**
You must first use the `calculate_per_capita_income` tool, providing your gross family income and number of household members. This result is then passed to the `determine_eligibility_tier` tool to classify your status (Full/Partial Scholarship).

**Q: How do I check if my academic scores are high enough?**
After determining your financial tier, use the `identify_eligible_courses` tool. This function takes your ENEM scores and whether you attended a public school to suggest qualified courses, considering both your academic achievement and scholarship restrictions.

**Q: Where can I find participating universities near me?**
To get a list of potential institutions, use the `query_university_locations` tool. Simply provide your preferred city to receive hardcoded results of universities participating in ProUni programs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prouni-eligibility-calculator](https://vinkius.com/mcp/prouni-eligibility-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ProUni Eligibility Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `prouni-eligibility-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ProUni Eligibility Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "prouni-eligibility-calculator": {
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
