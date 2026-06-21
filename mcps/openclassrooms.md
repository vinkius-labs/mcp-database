# OpenClassrooms MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openclassrooms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Monitor student progress on OpenClassrooms — search courses, track diploma paths, review mentoring sessions, and verify certificates from any AI agent.

## Description
Connect your **OpenClassrooms** partner account to any AI agent and get full visibility into courses, student progress, and diploma paths — all through natural conversation.

### What you can do

- **Course Catalog** — List available courses, search by keyword (React, Python, Data Science), and view detailed syllabi with skill competencies
- **Diploma Paths** — Browse career-focused paths with all required courses, projects, and estimated completion times
- **Student Tracking** — List enrolled students under your partner account and check individual progress including project validations and completion percentages
- **Mentoring Sessions** — View past and upcoming mentoring sessions with session dates, mentors, and status
- **Certificates** — Retrieve verified completion certificates for any student with public verification IDs

### How it works

1. Subscribe to this server
2. Enter your OpenClassrooms Partner API Key
3. Start monitoring student progress from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Training managers** — track team upskilling progress across multiple diploma paths without switching to the OpenClassrooms dashboard
- **HR departments** — verify employee certifications and completion rates for compliance reporting
- **EdTech partners** — pull course metadata and student analytics for custom dashboards and integration workflows


## Available Tools (9)
- **lister_cours**: Lister les cours disponibles sur OpenClassrooms (Pagination active)
- **consulter_cours**: Consulter le détail profond d'un cours spécifique
- **rechercher_cours**: Rechercher des cours OpenClassrooms dynamiquement par mots-clés
- **lister_parcours**: Lister l'intégralité des parcours diplômants OpenClassrooms
- **consulter_parcours**: Consulter la taxonomie détaillée d'un parcours diplômant spécifique
- **lister_etudiants**: Lister les étudiants inscrits sous cette clé d'API (Partenaires)
- **progression_etudiant**: Consulter la progression précise d'un étudiant métier
- **sessions_mentorat**: Lister les sessions de mentorat vidéo programmées
- **certificats_etudiant**: Consulter les certificats de réussite obtenus par un étudiant


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenClassrooms** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for courses about Python data analysis."

**🤖 AI Agent:**
> Found 8 courses matching 'Python data analysis'. Top results: 1) 'Analyze Your Data with Python' (Beginner, ~10h). 2) 'Use Python Libraries for Data Science' (Intermediate, ~15h). 3) 'Clean Your Data with Python' (Beginner, ~8h). Want me to open the full syllabus for any of these?

---

**👤 You:**
> "How is Maria Silva progressing in her diploma path?"

**🤖 AI Agent:**
> Maria Silva — Path: 'Web Developer' (12 courses total). Progress: 75% complete (9/12 courses finished). Currently on: 'Build a Responsive Website with HTML & CSS'. 2 projects validated, 1 project pending review. Next mentoring session: April 3 at 14:00. She's on track to finish by May 15.

---

**👤 You:**
> "Which students have earned certificates this month?"

**🤖 AI Agent:**
> 3 students earned certificates in March. Alex Chen — 'Data Analyst' path completed (Cert ID: OC-2024-8834). Julia Martinez — 'Product Manager' path completed (Cert ID: OC-2024-8901). Tom Nguyen — 'Front-End Developer' path completed (Cert ID: OC-2024-8955). All certificates are publicly verifiable.


## ❓ FAQ

**Q: Can I track completion rates across my entire team at once?**
Yes. List all students associated with your partner API key, then ask your agent to summarize each student's completion percentage and pending projects. Get a full team progress report in a single conversation — no spreadsheets, no manual exports from the OpenClassrooms dashboard.

**Q: What data do I get about mentoring sessions?**
The agent pulls session date, time, mentor name, session status (completed, scheduled, or missed), and the student linked to each session. This is useful for auditing mentorship quality and identifying students who are missing their scheduled sessions.

**Q: Is this API available to everyone or only to OpenClassrooms partners?**
The OpenClassrooms API is restricted to approved partners. You need an active partnership agreement with OpenClassrooms to obtain production API credentials. If you're already a partner, your account manager can provide the API key. This integration is designed for organizations using OpenClassrooms for team training.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openclassrooms](https://vinkius.com/mcp/openclassrooms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenClassrooms** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `openclassrooms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenClassrooms** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openclassrooms": {
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
