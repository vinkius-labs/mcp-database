# Gutendex MCP Server

Search and discover 70,000+ free public domain ebooks from Project Gutenberg — no API key required.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gutendex)

## Overview
**Category:** knowledge-management
**Tools Count:** 3

## Description
Connect to **Gutendex** and explore the world's largest collection of free public domain ebooks through natural conversation — no API key needed.

### What you can do

- **Book Search** — Search 70,000+ ebooks by title, author, subject or language
- **Book Details** — Get complete info including authors, subjects, download formats (HTML, EPUB, Kindle, PDF) and download counts
- **Language Filter** — Filter books by language (English, Portuguese, French, Spanish, German, etc.)
- **Author Filter** — Filter by author birth/death year ranges
- **Copyright Filter** — Filter by public domain or in-copyright status
- **Format Filter** — Filter by available formats (PDF, EPUB, HTML, plain text, audiobook)
- **Direct Access** — Look up books directly by Gutenberg URL or ID

### How it works

1. Subscribe to this server
2. No API key needed — start searching immediately
3. Discover free ebooks from Claude, Cursor, or any MCP-compatible client

No API key required — completely free, no registration.

### Who is this for?

- **Readers** — discover free classics like Pride and Prejudice, Frankenstein, Moby Dick and thousands more
- **Students** — find public domain books for research with language and subject filters
- **Researchers** — explore book metadata, download statistics and subject classifications
- **Book Clubs** — search by topic, author or language to find reading recommendations


## Available Tools
- **get_book**: Returns the title, authors (with birth/death years), subjects, bookshelves, languages, summary, download counts and all available formats/URLs (HTML, EPUB, Kindle, PDF, plain text). Common IDs: 1342 (Pride and Prejudice), 84 (Frankenstein), 4300 (Ulysses), 2701 (Moby Dick), 1727 (Romeo and Juliet).

Get detailed info for a specific Gutenberg book
- **get_books_by_url**: org URL and returns the book details. Accepts URLs like "https://www.gutenberg.org/ebooks/1342" or "https://www.gutenberg.org/files/1342/".

Get book info from a Gutenberg URL
- **list_books**: Supports powerful filters: search by title/author, topic/subject, language (ISO 2-letter codes like "en", "fr", "pt"), copyright status, MIME type (e.g. "application/pdf" for PDFs), author birth/death year ranges, and specific Gutenberg IDs. Results sorted by popularity (download count) by default. Returns book titles, authors, subjects, languages, download URLs and download counts. Supports pagination.

Search Project Gutenberg ebooks via Gutendex


## Installation & Usage

To install and use the **Gutendex** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gutendex](https://vinkius.com/mcp/gutendex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
