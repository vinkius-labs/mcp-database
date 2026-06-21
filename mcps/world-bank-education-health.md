# World Bank Education & Health MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/world-bank-education-health)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Retrieve global life expectancy, infant mortality, literacy rates, and social welfare statistics without any authentication.

## Description
Empower your agent with critical humanitarian, health, and educational data from the World Bank.

### What you can do
- **Health Outcomes** — Access life expectancy and mortality rates.
- **Education Standards** — Evaluate adult literacy rates globally.
- **Government Spending** — Measure health and education expenditures as a percentage of GDP.

### How it works
1. Subscribe to the server in one click.
2. It requires zero authentication details.
3. Turn your AI into a global health analyst.

### Who is this for?
Public health analysts, educators, policy makers, and humanitarian organizations.


## Available Tools
- **get_life_expectancy**: Get life expectancy at birth
- **get_infant_mortality**: Get infant mortality rate
- **get_health_expenditure**: Get current health expenditure (% of GDP)
- **get_literacy_rate**: Get adult literacy rate
- **get_edu_health_indicator**: Get any World Bank education/health indicator by code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **World Bank Education & Health** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare life expectancy in Japan versus the global average."

**🤖 AI Agent:**
> 🌍 **Life Expectancy: Japan vs World**

Japan leads globally with a life expectancy of approximately 84 years, well above the worldwide average of ~73 years. This gap reflects Japan's world-class healthcare system and lifestyle factors.

---

**👤 You:**
> "How has infant mortality improved in India over the last 30 years?"

**🤖 AI Agent:**
> 🌍 **Infant Mortality: India (1994–2024)**

India has achieved remarkable progress, reducing infant mortality from over 80 per 1,000 live births in the mid-1990s to approximately 25 today — a nearly 70% reduction driven by expanded healthcare access.

---

**👤 You:**
> "Which countries spend the most on education as a percentage of GDP?"

**🤖 AI Agent:**
> 🌍 **Education Spending Leaders**

Nordic countries consistently lead: Norway, Sweden, and Denmark each allocate around 6–8% of GDP to education, compared to a global average of approximately 4.3%.


## ❓ FAQ

**Q: How do I get started?**
Our World Bank Open Data servers require absolutely zero authentication. You do not need to register, get an API key, or setup webhooks. Just instantly connect and your AI agent can begin querying decades of global data.

**Q: Can it analyze government spending on healthcare?**
Yes, your AI agent can retrieve health expenditure as a % of GDP to correlate spending with life expectancy outcomes over multiple years.

**Q: Can I query literacy improvements over decades?**
Absolutely. Ask your agent to pull education indicators spanning back decades to demonstrate clear upward trends in global literacy.

**Q: What is the scale of the data I can access?**
You have direct access to 64 years of historical data covering 196+ sovereign states and global regional aggregates, powered directly by the World Bank's robust open data initiatives.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/world-bank-education-health](https://vinkius.com/mcp/world-bank-education-health)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **World Bank Education & Health** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `world-bank-education-health` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **World Bank Education & Health** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "world-bank-education-health": {
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
