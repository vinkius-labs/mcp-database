# edX MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/edx)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search and discover online courses from Harvard, MIT, Berkeley and 160+ top institutions on edX.

## Description
Connect to **edX** and explore the world's largest online learning platform through natural conversation — no API key needed.

### What you can do

- **Course Search** — Search thousands of courses by topic, university, level and language
- **Course Details** — Get full course info including descriptions, prerequisites and effort estimates
- **Course Runs** — Find upcoming and current course offerings with start dates and enrollment links
- **Programs** — Browse MicroMasters, Professional Certificates, XSeries and Bootcamps
- **Organizations** — Explore all partner universities and institutions (Harvard, MIT, Google, IBM)
- **Subjects** — Discover all subject categories available on the platform

### How it works

1. Subscribe to this server
2. No API key needed — start searching immediately
3. Discover online courses from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Students** — find courses by topic, compare offerings from different universities and discover programs
- **Lifelong Learners** — explore subjects, discover MicroMasters and Professional Certificates
- **Educators** — research what courses are available, compare institutions and find learning paths


## Available Tools
- **get_course**: Returns title, description, organization, level, subjects, pacing, estimated effort, prerequisites and available course runs.

Get detailed info for a specific edX course
- **get_course_run**: Get details for a specific course run
- **get_course_runs**: Optionally filter by course key and status (upcoming, current, archived).

Get course runs (scheduled offerings) for courses
- **get_organizations**: Returns organization names, descriptions, logos and course counts. Includes Harvard, MIT, Berkeley, Google, IBM and many more.

Get partner organizations that offer courses on edX
- **get_program**: Get details for a specific edX program
- **get_subjects**: Returns subject names, descriptions and course counts. Useful for discovering what topics are covered on the platform.

Get course subject categories
- **search_courses**: Supports free-text search, filtering by organization, level (beginner/intermediate/advanced), language, subject. Returns course titles, descriptions, organizations, levels, subjects and enrollment links.

Search for online courses on edX
- **search_programs**: Includes MicroMasters, Professional Certificates, XSeries and Bootcamps. Returns program titles, descriptions, course counts and type.

Search for edX programs (MicroMasters, Professional Certificates, XSeries)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **edX** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find machine learning courses from Harvard."

**🤖 AI Agent:**
> Found 12 machine learning courses from HarvardX. Notable: 'CS109B Data Science 2: Advanced Topics' (Harvard), 'Machine Learning Fundamentals' (Harvard). Courses include self-paced and instructor-led options.

---

**👤 You:**
> "Show me all MicroMasters programs in Data Science."

**🤖 AI Agent:**
> Found 8 MicroMasters programs in Data Science: MIT's 'Statistics and Data Science' (4 courses, $1,350), Columbia's 'Data Science' (4 courses), Georgia Tech's 'Analytics' (4 courses). Each includes course details and enrollment links.

---

**👤 You:**
> "What organizations offer courses on edX?"

**🤖 AI Agent:**
> edX partners with 160+ institutions including: Harvard, MIT, Berkeley, Google, IBM, Microsoft, Columbia, Cornell, Caltech, University of Sydney, Tsinghua University and many more top universities and companies.


## ❓ FAQ

**Q: Do I need an API key?**
No! edX's Discovery API is completely free and open for public course catalog data. No authentication required.

**Q: Can I search courses by university?**
Yes! Use search_courses with the org parameter to filter by organization (e.g. "HarvardX", "MITx", "BerkeleyX"). You can also search by topic, level, language and subject simultaneously.

**Q: What types of programs are available?**
edX offers MicroMasters (graduate-level), Professional Certificates (industry-recognized), XSeries (multi-course), and Bootcamps (intensive). Use search_programs with type parameter to filter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/edx](https://vinkius.com/mcp/edx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **edX** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `edx` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **edX** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "edx": {
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
