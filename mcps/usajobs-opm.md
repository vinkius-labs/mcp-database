# USAJOBS (OPM) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/usajobs-opm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search and analyze federal job opportunities directly from USAJOBS. Access active listings, historic data, and detailed job requirements.

## Description
Connect to the official **USAJOBS** (Office of Personnel Management) database to explore federal career opportunities through your AI agent. This server provides comprehensive access to the federal hiring ecosystem.

### What you can do

- **Active Job Search** — Query live job announcements using keywords, locations, salary ranges, and hiring paths (e.g., Veterans, Students, Public).
- **Historic Data Retrieval** — Access bulk data for current and past job opportunity announcements (JOAs) for trend analysis or research.
- **Detailed Job Analysis** — Fetch full text for specific announcements, including detailed summaries, duties, and qualification requirements.
- **Reference Data** — Retrieve valid codes for occupational series, agency subelements, pay plans, and more to refine your searches.

### How it works

1. Subscribe to this server
2. Enter your USAJOBS API Key and User Agent (email address)
3. Start searching for federal roles directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Job Seekers** — Find specific federal roles that match your skills and location without navigating complex search filters manually.
- **Career Counselors** — Help clients identify federal career paths and understand specific qualification requirements.
- **Data Analysts** — Analyze federal hiring trends using historic JOA data and occupational series codes.


## Available Tools (4)
- **get_announcement_text**: for historic JOAs.

Retrieve long text fields for current and past job postings
- **get_code_list**: No auth required.

Retrieve valid values and codes for filtering search results
- **get_historic_joas**: Supports pagination via continuationtoken.

Retrieve bulk data for current and past job postings
- **search_jobs**: You can filter by keyword, location, job category, and more.

Search for currently open job announcements on USAJOBS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **USAJOBS (OPM)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for active Software Engineer jobs in Washington, DC with a minimum salary of $100,000."

**🤖 AI Agent:**
> I found 12 active Software Engineer positions in Washington, DC meeting your criteria. Notable listings include a Lead Developer role at the Department of State and a Senior Engineer position at NASA. Would you like the details for any of these?

---

**👤 You:**
> "Get the full duties and qualifications for announcement number 784521900."

**🤖 AI Agent:**
> Retrieving announcement text... For JOA 784521900, the primary duties involve managing cloud infrastructure and ensuring cybersecurity compliance. Qualifications require at least one year of specialized experience at the GS-12 level. Shall I summarize the full text for you?

---

**👤 You:**
> "List the occupational series codes for Information Technology positions."

**🤖 AI Agent:**
> I've fetched the code list. For Information Technology, the primary series is 2210. Other related codes include 1550 (Computer Science) and 0854 (Computer Engineering).


## ❓ FAQ

**Q: How can I filter jobs by a specific location and salary range?**
Use the `search_jobs` tool. You can provide parameters like `LocationName` (e.g., 'Washington, DC') and `RemunerationMinimumAmount` to narrow down the results to your specific needs.

**Q: Where can I find the full description of duties for a job posting?**
The `get_announcement_text` tool is designed specifically for this. By providing the announcement number, the agent will retrieve the full text for Summary, Duties, and Qualifications.

**Q: How do I know which codes to use for occupational series like IT or Engineering?**
You can use the `get_code_list` tool with the endpoint 'occupationalseries'. This will return a list of all valid codes and their corresponding titles (e.g., 2210 for Information Technology).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/usajobs-opm](https://vinkius.com/mcp/usajobs-opm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **USAJOBS (OPM)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `usajobs-opm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **USAJOBS (OPM)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "usajobs-opm": {
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
