# OpenClassrooms MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openclassrooms)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/openclassrooms-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/openclassrooms-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **OpenClassrooms** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openclassrooms](https://vinkius.com/mcp/openclassrooms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
