# Indeed MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/indeed)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search for job listings on Indeed — find roles by keyword, location, and job type directly from any AI agent.

## Description
Connect your AI agent to **Indeed**, the world's #1 job site, to streamline your recruitment or job-seeking workflows through natural conversation.

### What you can do

- **Job Search** — Query millions of job listings using keywords, titles, or company names
- **Location Filtering** — Narrow down results to specific cities, states, or zip codes with adjustable search radii
- **Advanced Filters** — Filter by job type (full-time, part-time, contract, internship, or temporary) and sort by relevance or date
- **Pagination Support** — Browse through large sets of results efficiently using start and limit parameters

### How it works

1. Subscribe to this server
2. Enter your Indeed Publisher ID
3. Start searching for jobs from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters** — quickly find market benchmarks and active listings for specific roles
- **Job Seekers** — automate the search for new opportunities without leaving your workspace
- **HR Tech Developers** — integrate live job data into your AI-driven workflows


## Available Tools
- **search_jobs**: Search for jobs on Indeed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Indeed** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Software Engineer' jobs in 'New York'."

**🤖 AI Agent:**
> I found several Software Engineer positions in New York. The top results include roles at TechCorp and Innovate Solutions. Would you like to see more details for any of these?

---

**👤 You:**
> "Find part-time 'Graphic Designer' roles within 25 miles of Austin."

**🤖 AI Agent:**
> I've located 3 part-time Graphic Designer roles within 25 miles of Austin. They range from boutique agencies to larger firms. Should I list the specific requirements for the most recent one?

---

**👤 You:**
> "Get the latest 'Data Scientist' job listings sorted by date."

**🤖 AI Agent:**
> Here are the most recent Data Scientist listings, sorted by date. The newest post was added just 2 hours ago. Do you want to filter these by a specific job type?


## ❓ FAQ

**Q: Can I filter by job type like 'full-time' or 'contract'?**
Yes! Use the `search_jobs` tool with the `jt` parameter. You can specify 'fulltime', 'parttime', 'contract', 'internship', or 'temporary' to narrow down your results.

**Q: How do I sort the results to see the newest jobs first?**
Simply set the `sort` parameter to 'date' when calling the `search_jobs` tool. By default, results are sorted by relevance.

**Q: Is it possible to search within a specific radius of a city?**
Yes, you can use the `radius` parameter to define the distance in miles from your target location (provided in the `l` parameter).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/indeed](https://vinkius.com/mcp/indeed)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Indeed** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `indeed` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Indeed** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "indeed": {
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
