# Gutendex MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gutendex)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Search and discover 70,000+ free public domain ebooks from Project Gutenberg — no API key required.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gutendex** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find Pride and Prejudice by Jane Austen."

**🤖 AI Agent:**
> Found 'Pride and Prejudice' by Jane Austen (Gutenberg ID: 1342). Published 1813. Subjects: Love stories, Young women, England, Social classes. Download count: 50,000+. Available formats: HTML, EPUB, Kindle, plain text. Authors: Jane Austen (1775-1817).

---

**👤 You:**
> "Search for science fiction books in Portuguese."

**🤖 AI Agent:**
> Found 200+ books matching 'science fiction' with Portuguese language available. Notable titles include works by Machado de Assis (Brazilian author, 1839-1908), Júlio Verne translations, and classic Brazilian literature. Results sorted by download popularity.

---

**👤 You:**
> "Show me Frankenstein by Mary Shelley."

**🤖 AI Agent:**
> Found 'Frankenstein; Or, The Modern Prometheus' by Mary Wollstonecraft Shelley (Gutenberg ID: 84). Published 1818. Subjects: Science fiction, Gothic fiction, Monsters, Frankenstein's monster. Download count: 35,000+. Available in HTML, EPUB, Kindle, plain text and audio.


## ❓ FAQ

**Q: Do I need an API key?**
No! Gutendex is completely free and requires no authentication. Just subscribe and start searching. There's no sign-up or registration needed.

**Q: What books are available?**
Gutendex indexes 70,000+ ebooks from Project Gutenberg, the world's oldest digital library. This includes classics like Pride and Prejudice, Frankenstein, Moby Dick, Romeo and Juliet, Alice's Adventures in Wonderland and thousands of other public domain works in many languages.

**Q: Can I filter by language?**
Yes! Use the languages parameter with ISO 2-letter codes: "en" for English, "pt" for Portuguese, "fr" for French, "es" for Spanish, "de" for German, etc. You can also combine multiple languages: "en,fr" for English and French books.

**Q: Can I download the books?**
Yes! Each book includes download URLs in multiple formats: HTML, EPUB, Kindle (MOBI), plain text, PDF and sometimes audio. The download links go directly to Project Gutenberg's servers. All books are in the public domain in the United States.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gutendex](https://vinkius.com/mcp/gutendex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gutendex** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gutendex` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gutendex** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gutendex": {
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
