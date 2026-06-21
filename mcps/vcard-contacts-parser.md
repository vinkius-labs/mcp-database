# vCard Contacts Parser MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vcard-contacts-parser)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vcard-contacts-parser-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vcard-contacts-parser-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Instantly convert massive iPhone and Android `.vcf` contact exports into structured JSON. Turn your AI into a hyper-intelligent local address book.

## Description
When you export your phone's address book, you get a massive `.vcf` file containing hundreds of contacts formatted in the legacy `BEGIN:VCARD` structure, often bloated with base64-encoded profile pictures. If you ask an LLM to read this raw file, it will exhaust its context window and hallucinate phone numbers and emails.

This MCP is a dedicated contact intelligence engine. It runs 100% local on your machine, instantly stripping away the binary noise and converting the raw vCard format into a beautiful, easily queryable JSON array. The AI sees exactly what it needs: First Name, Last Name, Organization, Phone, and Email.

### The Superpowers

- **100% Air-Gapped Privacy:** Your personal phonebook never leaves your local machine.
- **Zero Hallucination:** Perfect extraction of country codes, emails, and company roles.
- **Massive File Support:** Can instantly process a VCF file containing 5,000+ contacts.
- **Assistant Ready:** Ask your AI: 'Find the phone number for the CTO of Vinkius in my contacts.'


## Available Tools
- **parse_kindle_clippings**: Paste the raw text content from the "My Clippings.txt" file found on a Kindle device.

Parse Amazon Kindle "My Clippings.txt" exports into structured JSON. Extracts highlights, notes, and bookmarks grouped by book


## 💬 Prompt Examples

Here are some examples of how you can interact with the **vCard Contacts Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my contacts.vcf and give me a list of everyone who works at 'Vinkius'."

**🤖 AI Agent:**
> I found 3 contacts working at Vinkius: John Silva (DevOps), Sarah Connor (Design), and Mike Ross (Legal).

---

**👤 You:**
> "Extract all the email addresses from this vCard export and format them as a CSV."

**🤖 AI Agent:**
> Name,Email
Alice Smith,alice@example.com
Bob Jones,bob@example.org

---

**👤 You:**
> "Look through my contacts and find the phone number for 'Plumber'."

**🤖 AI Agent:**
> The phone number saved under 'Plumber' is +1 (555) 019-8372.


## Installation & Usage

To install and use the **vCard Contacts Parser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vcard-contacts-parser](https://vinkius.com/mcp/vcard-contacts-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
