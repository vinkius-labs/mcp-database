# Degreed MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/degreed)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to discover learning content, track skills, and monitor user completions via the Degreed API.

## Description
Integrate **Degreed**, the leading upskilling and learning experience platform (LXP), directly into your AI workflow. Discover available learning content, monitor employee skill profiles, and track progress across pathways and plans using natural language.

### What you can do

- **Content Discovery** — Search the entire Degreed catalog for courses, articles, and videos matching specific keywords.
- **Skill Intelligence** — List and review the defined skills taxonomy and individual user skill profiles.
- **Learning Oversight** — Monitor user completions, active learning plans, and curated pathways.
- **User Research** — Retrieve detailed metadata and activity summaries for learners in your organization.

### How it works

1. Connect the Degreed integration to your AI assistant.
2. Authorize using your Degreed Client ID and Client Secret (found in your API settings).
3. Orchestrate your organization's learning and development through intuitive conversation.

### Who is this for?

- **L&D Managers** — Quickly check learner progress and content availability on the go.
- **Talent Partners** — Research employee skill sets and identify talent gaps via chat.
- **Team Leads** — Monitor team learning goals and pathway completions during planning.


## Available Tools (10)
- **get_content_details**: Resolves detailed descriptions, associated skill tags, and duration metadata.

Get detailed metadata for a specific learning item
- **get_user_profile**: Resolves assigned skill ratings, learning progress, and active pathways within the Degreed ecosystem.

Get full profile and skill data for a specific user
- **list_active_learners**: Identifies users with recent completion activity within the Degreed workspace.

List users who have completed learning recently
- **list_learning_content**: Returns content metadata including titles, providers, content types (e.g., article, video, course), and external URLs.

List all available learning content in the Degreed catalog
- **list_learning_pathways**: Returns pathway metadata including objectives, total duration, and completion requirements.

List curated learning pathways available to users
- **list_learning_plans**: Returns active learning plans, including target completion dates and linked competencies.

List learning plans and goals configured in the system
- **list_defined_skills**: Returns the standardized list of skills and competencies defined by the organization for talent mapping.

List the skills taxonomy defined in your organization
- **list_user_completions**: Returns a history of all learned items with completion timestamps and earned skill points.

List all learning content completed by a specific user
- **list_degreed_users**: Returns a list of users with metadata including system IDs, professional titles, and organizational affiliations.

List all users registered in your Degreed organization
- **search_learning_catalog**: Matches terms against titles, descriptions, and skill tags to return a ranked list of relevant learning materials.

Search for learning content by keyword or term


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Degreed** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for courses related to 'Data Science with Python'."

**🤖 AI Agent:**
> I've found several courses on 'Data Science with Python', including 'Intro to Pandas' and 'Machine Learning Basics'. Would you like to see the duration and provider for these items?

---

**👤 You:**
> "List all learning plans for user 'Alice Johnson'."

**🤖 AI Agent:**
> Alice Johnson has 2 active learning plans: 'Leadership Foundations' and 'Advanced SQL'. She has completed 65% of the leadership plan. Should I list the next steps in her 'Advanced SQL' goal?

---

**👤 You:**
> "What skills are most common in the 'Engineering' team?"

**🤖 AI Agent:**
> In the Engineering team, the top skills identified are 'React.js', 'Node.js', and 'System Architecture'. 80% of members have a 'Proficient' rating in React. Would you like a breakdown of skill gaps for this team?


## ❓ FAQ

**Q: How do I get Degreed API credentials?**
Log in to your Degreed admin account, navigate to the API settings section, and create a new application to retrieve your Client ID and Client Secret for OAuth 2.0 authentication.

**Q: Can the agent assign learning content?**
This integration currently focuses on discovering content and monitoring progress. Assigning content to specific users is managed via the Degreed dashboard or mobile app.

**Q: Are skill ratings included?**
Yes, when retrieving user profiles, the agent can provide information on skills associated with the user and their current proficiency levels where available.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/degreed](https://vinkius.com/mcp/degreed)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Degreed** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `degreed` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Degreed** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "degreed": {
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
