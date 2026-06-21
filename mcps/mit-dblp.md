# MIT DBLP MCP Server

Search millions of computer science publications, find author profiles, and explore academic citation networks across conferences.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mit-dblp)

## Overview
**Category:** knowledge-management
**Tools Count:** 16

## Description
Connect to the **DBLP Computer Science Bibliography** — the most comprehensive index of CS research, maintained by Schloss Dagstuhl.

### What you can do

- **Full-Text Search** — Search 6M+ CS publications across all venues
- **Author Profiles** — Explore researcher profiles and publication histories
- **Venue Browsing** — Search conferences (NeurIPS, ICML, SIGMOD, OSDI) and journals (JACM, TOCS)
- **Co-Author Networks** — Discover collaboration patterns between researchers
- **AI/ML Papers** — Dedicated search for NeurIPS, ICML, ICLR, and AAAI papers
- **Systems Papers** — Dedicated search for OSDI, SOSP, SIGCOMM, NSDI papers
- **Theory Papers** — Dedicated search for STOC, FOCS, SODA papers
- **Database Papers** — Dedicated search for SIGMOD, VLDB, ICDE papers
- **Author Statistics** — Publication counts, venue distribution, and year-over-year trends

### Who is this for?

- **CS Researchers** — literature reviews and related work discovery
- **PhD Students** — find the latest papers in your area
- **Faculty** — track research output and collaboration networks
- **Hiring Committees** — evaluate candidate publication records


## Available Tools
- **get_author**: The PID can be found in DBLP URLs (e.g. for "https://dblp.org/pid/b/YoshuaBengio" the PID is "b/YoshuaBengio").

Get author profile by DBLP PID
- **get_author_publications**: Returns up to 40 most recent publications with full metadata. Use the author name as it appears on DBLP.

Get all publications by a specific author
- **get_author_stats**: Essential for evaluating research productivity and impact.

Get publication statistics for an author
- **get_coauthors**: Returns a ranked list of collaborators ordered by number of joint publications. Essential for understanding research collaboration patterns.

Get co-author network of a researcher
- **get_publication**: g. "journals/cacm/Knuth74", "conf/nips/VaswaniSPUJGKP17"). The key uniquely identifies every record in DBLP.

Get publication details by DBLP key
- **get_venue**: Use conference abbreviations (ICML, NeurIPS, SIGMOD) or full journal names.

Get venue details (conference or journal)
- **get_venue_publications**: Essential for exploring what was published at a particular conference edition (e.g. NeurIPS 2024).

Get papers published at a specific venue
- **search_ai_papers**: These are the premier conferences for artificial intelligence and machine learning research.

Search AI and machine learning papers at top venues
- **search_authors**: Returns author names, DBLP profile URLs, and disambiguation notes. DBLP meticulously disambiguates authors with the same name.

Search computer science authors on DBLP
- **search_by_year**: Useful for tracking research trends over time or finding papers from a specific conference edition.

Search publications filtered by year
- **search_database_papers**: Search database papers at top venues
- **search_in_venue**: Combine a venue name with an optional topic query to find relevant papers at a particular venue.

Search for papers within a specific venue
- **search_publications**: Covers all major conferences (NeurIPS, ICML, SIGMOD, VLDB, OSDI) and journals (JACM, TOCS, VLDBJ). Returns titles, authors, venues, years, DOIs, and DBLP keys.

Search 6M+ computer science publications on DBLP
- **search_systems_papers**: Search systems papers at top venues
- **search_theory_papers**: Search theoretical CS papers at top venues
- **search_venues**: Returns venue names, DBLP URLs, and types.

Search CS conferences and journals


## Installation & Usage

To install and use the **MIT DBLP** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mit-dblp](https://vinkius.com/mcp/mit-dblp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
