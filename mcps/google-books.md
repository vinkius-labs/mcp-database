# Google Books MCP Server

Search and explore millions of books on Google Books — find titles, authors, reviews, previews and full text from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/google-books)

## Overview
**Category:** industry-titans
**Tools Count:** 8

## Description
Connect to **Google Books** and explore the world's largest searchable book index through natural conversation.

### What you can do

- **Book Search** — Search millions of books by title, author, publisher, ISBN, subject or keyword with advanced query operators
- **Book Details** — Get comprehensive info including authors, publisher, publication date, page count, categories, ratings and preview links
- **Public Bookshelves** — Browse curated reading lists and collections from other users
- **My Library** — Access your personal bookshelves (favorites, purchased, reviewed) with OAuth authentication
- **Filtering** — Filter by free ebooks, paid ebooks, language, newest first and print type

### How it works

1. Subscribe to this server
2. Enter your Google Books API Key
3. Start exploring millions of books from Claude, Cursor, or any MCP-compatible client

No more navigating the Google Books website to find book details or reading lists. Your AI acts as a dedicated literary research assistant.

### Who is this for?

- **Readers** — quickly find books by title or author, check descriptions and ratings before purchasing
- **Researchers** — search academic books by subject, publisher or ISBN with precise query operators
- **Book Clubs** — browse public bookshelves for curated reading recommendations
- **Students** — find textbooks, check page counts and discover free ebook editions


## Available Tools
- **get_book**: Requires the Google Books volume ID (found from search results).

Get detailed info for a specific book by volume ID
- **get_bookshelf**: Returns the shelf title, description, volume count, accessibility and self-link. Shelf IDs are numeric (e.g. "0", "1", "2") or named (e.g. "favorites", "purchased").

Get a specific public bookshelf
- **get_my_bookshelf_volumes**: Each volume includes title, authors, publisher, description and image links. Requires an OAuth 2.0 token. Optionally set maxResults (1-40).

List books in the authenticated user's bookshelf
- **get_my_bookshelves**: Each bookshelf includes its ID, title, volume count and accessibility. Requires an OAuth 2.0 token (the API key alone is not sufficient for private shelves).

List the authenticated user's bookshelves
- **get_volume_by_isbn**: Returns the book details including title, authors, publisher, description, page count and image links. Useful for quickly finding a specific edition when you have the ISBN. This is equivalent to using search_books with the isbn: operator but returns a single result directly.

Look up a book by its ISBN number
- **list_bookshelf_volumes**: Each volume includes title, authors, publisher, description, page count, categories and image links. Useful for browsing curated reading lists. Optionally set maxResults (1-40).

List books in a public bookshelf
- **list_bookshelves**: Each bookshelf includes its ID, title, volume count, accessibility (public/private) and description. Useful for discovering reading lists and curated collections.

List public bookshelves for a Google Books user
- **search_books**: Supports powerful search operators: intitle: (search in title only), inauthor: (search by author), inpublisher:, subject:, isbn:, lccn:, oclc:. Use quotes for exact phrase matching ("the great gatsby") and - to exclude terms. Optionally set maxResults (1-40), startIndex for pagination, filter (free-ebooks, paid-ebooks), language restriction, order by (relevance, newest) and print type (books, magazines).

Search for books on Google Books


## Installation & Usage

To install and use the **Google Books** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-books](https://vinkius.com/mcp/google-books)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
