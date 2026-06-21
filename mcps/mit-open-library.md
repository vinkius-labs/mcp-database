# MIT Open Library MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mit-open-library)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mit-open-library-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mit-open-library-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access millions of books, read them online, and explore the world largest open catalog of bibliographic data for every title.

## Description
Connect to the **Open Library API** — the Internet Archive's open catalog of over 20 million books.

### What you can do

- **Book Search** — Full-text search across 20M+ books with sorting and pagination
- **ISBN Lookup** — Find any book by its ISBN-10 or ISBN-13
- **Author Profiles** — Biographies, bibliographies, and author photos
- **Subject Browsing** — Explore books by topic (Computer Science, Physics, Mathematics)
- **Full-Text Access** — Filter for books with freely readable full text on the Internet Archive
- **Edition Discovery** — Find all editions, translations, and formats of any book
- **Publisher Search** — Browse catalogs from MIT Press, O'Reilly, Cambridge University Press
- **Language Filter** — Search books by publication language
- **Cover Images** — Access book cover art in multiple sizes

### Who is this for?

- **Students** — find textbooks, references, and freely readable editions
- **Researchers** — discover comprehensive bibliographies and related works
- **Librarians** — catalog management and edition tracking
- **Book Lovers** — explore the world's largest open book catalog


## Available Tools
- **get_author**: The key format is "OL33421A" (found in Open Library URLs).

Get author profile by Open Library key
- **get_author_works**: Returns all works with titles, covers, and subjects.

Get all works by a specific author
- **get_edition**: Returns title, publisher, publication date, ISBNs, page count, physical format, languages, and cover images.

Get edition details by Open Library edition key
- **get_work**: g. "OL45883W" for The Lord of the Rings). Returns title, description, subjects, covers, and publication history.

Get book details by Open Library work key
- **get_work_editions**: Essential for finding specific translations or editions.

Get all editions of a specific book
- **search_authors**: Returns author names, birth/death dates, top works, total work counts, and main subjects. Open Library has profiles for hundreds of thousands of authors.

Search book authors on Open Library
- **search_books**: Returns titles, authors, publication years, edition counts, subjects, ISBNs, covers, and full-text availability. Sort options: "new", "old", "editions", "rating".

Search 20M+ books on Open Library
- **search_by_author**: Returns a complete bibliography with editions and publication details.

Search books by author name
- **search_by_isbn**: Returns title, publisher, publication date, page count, and cover images.

Look up a book by ISBN
- **search_by_language**: Use ISO 639-1 codes: "eng" (English), "fre" (French), "spa" (Spanish), "por" (Portuguese), "ger" (German), "jpn" (Japanese), "chi" (Chinese), "ara" (Arabic).

Search books by language
- **search_by_publisher**: Examples: "MIT Press", "Oxford University Press", "Cambridge University Press", "O'Reilly Media", "Springer".

Search books by publisher
- **search_by_subject**: Examples: "science_fiction", "artificial_intelligence", "quantum_physics", "mathematics", "computer_science", "philosophy", "history".

Browse books by subject category
- **search_by_title**: More precise than general search when you know the exact book title.

Search books by exact title
- **search_full_text**: Essential for finding freely readable books.

Search for books with full text available
- **search_recent**: Useful for discovering new additions to the catalog.

Browse recently added books
- **search_trending_subjects**: Browse popular books in a subject


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MIT Open Library** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find books about quantum computing published by MIT Press"

**🤖 AI Agent:**
> I've found MIT Press books on quantum computing, including textbooks on quantum algorithms, quantum information theory, and quantum error correction.

---

**👤 You:**
> "Look up all books by Richard Feynman"

**🤖 AI Agent:**
> I've retrieved Richard Feynman's complete bibliography from Open Library, including The Feynman Lectures on Physics, Surely You're Joking, and QED.

---

**👤 You:**
> "Find freely readable books on machine learning"

**🤖 AI Agent:**
> I've filtered for machine learning books with full-text availability on the Internet Archive. These editions can be borrowed or read online for free.


## Installation & Usage

To install and use the **MIT Open Library** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mit-open-library](https://vinkius.com/mcp/mit-open-library)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
