# FBI Crime Data Explorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fbi-crime-data-explorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access official FBI crime statistics, including national estimates, state-level summaries, and agency-specific data via AI.

## Description
Connect to the **FBI Crime Data Explorer (CDE)** to retrieve comprehensive law enforcement statistics directly through natural language. This server provides access to the Uniform Crime Reporting (UCR) program's extensive datasets.

### What you can do

- **National Estimates** — Retrieve estimated crime totals for the entire United States across specific year ranges.
- **State Summaries** — Fetch detailed offense data (violent crime, property crime, etc.) for any specific US state.
- **Agency-Level Data** — Query statistics reported by specific local, county, or state law enforcement agencies using their unique ORI identifier.
- **Victim Demographics** — Analyze NIBRS data to see breakdowns of victims by age, race, and sex for various offenses.

### How it works

1. Subscribe to this server
2. Enter your FBI CDE API Key
3. Start querying public safety data from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Analysts & Researchers** — quickly pull structured crime data for academic or professional reports.
- **Journalists** — verify crime statistics and trends for specific regions or agencies instantly.
- **Policy Makers** — evaluate the impact of safety initiatives using official historical data.


## Available Tools (4)
- **get_national_estimates**: Retrieve national crime estimates
- **get_nibrs_victim_demographics**: Retrieve NIBRS victim demographic data
- **get_state_summarized**: Retrieve crime statistics for a specific state
- **get_agency_summarized**: Retrieve crime data for a specific law enforcement agency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FBI Crime Data Explorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me national crime estimates from 2015 to 2020."

**🤖 AI Agent:**
> I've retrieved the national estimates. From 2015 to 2020, violent crime saw a peak in 2016 with approximately 1.28 million incidents, followed by a gradual decline until 2019. Would you like a breakdown by specific offense type?

---

**👤 You:**
> "Get summarized burglary data for California (CA) between 2018 and 2022."

**🤖 AI Agent:**
> Accessing California state data... For the period 2018-2022, burglary rates showed a downward trend, starting at X incidents in 2018 and reaching Y in 2022. Do you want to see how this compares to the national average?

---

**👤 You:**
> "What is the age breakdown of robbery victims in New York?"

**🤖 AI Agent:**
> Querying NIBRS demographics for New York... The data shows that the largest group of robbery victims falls within the 25-34 age range, accounting for approximately 28% of reported incidents. Would you like to see the breakdown by race or sex instead?


## ❓ FAQ

**Q: How do I find data for a specific local police department?**
You can use the `get_agency_summarized` tool. You will need the agency's 9-character ORI (Originating Agency Identifier) to retrieve their specific reported statistics.

**Q: What kind of demographic information is available for crime victims?**
The `get_nibrs_victim_demographics` tool allows you to filter victim data by age, race, or sex for specific offenses in states that support NIBRS reporting.

**Q: Can I compare crime trends over multiple years?**
Yes. Tools like `get_national_estimates` and `get_state_summarized` accept `start_year` and `end_year` parameters to provide data across a historical range.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fbi-crime-data-explorer](https://vinkius.com/mcp/fbi-crime-data-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FBI Crime Data Explorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fbi-crime-data-explorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FBI Crime Data Explorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fbi-crime-data-explorer": {
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
